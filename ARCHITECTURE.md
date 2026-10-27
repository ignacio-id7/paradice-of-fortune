[Español](ARQUITECTURA.md) · **English**

# Architecture

ParaDice of Fortune is built in Godot 4 with statically typed GDScript. This page summarises how it is organised and the design decisions behind it; the code itself is not published.

## Four layers

1. **Pure core.** The rules, the game, the score sheet, the players, the economy, the missions and the AI are plain objects with no scene nodes. Every action (roll, hold a die, score) is validated there: an illegal action is rejected and reported, never half-applied. A game in progress is saved as the list of the player's actions and, when resumed, those actions are replayed through the same validations.
2. **Services.** Audio, options, saving and the catalogue of pieces live as global services. The profile is versioned, migrated between versions and written atomically, so a crash never leaves it half-written.
3. **Content as data.** Pieces, worlds, sounds, missions, prices and AI settings are resources, not constants in the code: a world is added or tuned without touching the logic.
4. **Presentation.** The scene, the camera, the cup and the dice, the score sheet and the interface. A single controller orchestrates the flow and asks the core whether each action is legal.

## The pieces system

The table is assembled from interchangeable **slots**: dice, cup, tray, buttons, table, score sheet, ambience, music and cursor. Each piece brings looks and sound, **never physics**: the collision bodies are the same in every world, so changing worlds never changes the odds. Each sound belongs to the piece that makes it, and finishes change a piece's colours or materials without creating a new piece.

On top of the pieces sit the **table objects** (a skull, a lava lamp, empanadas) placed in «Decorate the table», and the **table spaces**: one complete table per world, switched in the middle of a game.

## Dice physics

- Real physics at 120 steps per second, with the cup moved by code so the dice inherit its motion.
- Dice enter the cup with a uniformly random rotation; the cup has invisible collision shaped like its visible walls, a lid while shaking and a pivot at the mouth when it tips over.
- A die reads its value from the face pointing up. A die that ends up stacked or tilted counts the face that shows the most, and stays where it fell.
- A die that has already shown its face is held still until the roll resolves: dice at rest are never re-thrown or nudged.

## Measured fairness

The fairness of the dice is a test, not a promise. The suite throws the dice thousands of times through the real mouse path and checks the distribution of faces with a chi-squared test, along with throw times and the absence of jumps after a die comes to rest. Each new set of dice can be put through the same test.

## The AI

Three levels. The easy one is a sensible player: it keeps the most repeated value and scores the box worth the most. The medium and hard ones compute the exact value of the round: every possible hand, every hold and their transitions, with zero, one and two rolls remaining. The hard level also weighs the upper bonus while it is still within reach. The AI plays through the same interface as a person, with real physics and readable pauses.

## Touch

On the phone, a touch mode replaces the mouse: drag from the cup to roll, two fingers to zoom and look around, side buttons to hold and score, and a «contemplate» mode to just look at the table. Sizes are expressed in millimetres on the screen, so they hold up whatever the resolution.

## Tests

More than ninety automated tests, unit and integration, run before every delivery. The runner treats any error, warning or memory leak as a failure, and can check that each test really fails when an assertion is forced.

---

[Back to the start](README.en.md)
