[Español](EVOLUCION.md) · **English**

# Evolution

How ParaDice of Fortune grew, phase by phase. Each phase ends with the automated test suite passing, the game playable from start to finish and the owner's review.

## Phase 0: Audit and visual direction

*2026-09-26 · Closed*

The starting point was an inherited prototype: playable, but fragile and without an identity. It was reviewed in full, a complete remake was agreed on, and three visual directions were tried as in-engine mock-ups: a fantasy inn lit by candles, a tavern keeper's tally board and a Frutiger Aero skin. The inn won, borrowing the moonlight and boxwood dice of the second one.

![The inherited prototype, before the remake.](media/fase-0/prototipo.webp)

*The inherited prototype, before the remake.*

![Mock-up A: the Oak Inn, the chosen direction.](media/fase-0/maqueta-a-posada.webp)

*Mock-up A: the Oak Inn, the chosen direction.*

![Mock-up B: the tavern keeper's tally board, with moonlight.](media/fase-0/maqueta-b-tablilla.webp)

*Mock-up B: the tavern keeper's tally board, with moonlight.*

![Mock-up C: the first take on Frutiger Aero.](media/fase-0/maqueta-c-aero.webp)

*Mock-up C: the first take on Frutiger Aero.*

![The three proposals, side by side.](media/fase-0/propuestas.webp)

*The three proposals, side by side.*

---

## Phase 1: Foundations

*2026-09-26 · Closed*

The rules moved into a pure core, separate from what is drawn on screen, and were tested with thousands of simulated games. The automated tests fail on any error, warning or memory leak. The profile is saved atomically and the game speaks Spanish and English from day one.

![The table running on the new core, still with the inherited art.](media/fase-1/inicio.webp)

*The table running on the new core, still with the inherited art.*

![The score sheet, now a pure view of the game state.](media/fase-1/cartola.webp)

*The score sheet, now a pure view of the game state.*

![End of game, with the record saved to the profile.](media/fase-1/fin.webp)

*End of game, with the record saved to the profile.*

![The same game in English.](media/fase-1/ingles.webp)

*The same game in English.*

---

## Phase 2: Playable core

*2026-09-26 · Closed*

The cup and the dice were rebuilt with real physics: grab the cup, shake it and let go. Each die is read by its top face, dice that land stacked or tilted count the face that shows the most, and the fairness of the rolls is measured over thousands of real throws.

![The cup tips over and the dice roll.](media/fase-2/rodando.webp)

*The cup tips over and the dice roll.*

![Dice held on the side rack before the next roll.](media/fase-2/retenidos.webp)

*Dice held on the side rack before the next roll.*

![Halfway through a game.](media/fase-2/cartola.webp)

*Halfway through a game.*

![A full roll, from the cup to rest.](media/fase-2/tirada.gif)

*A full roll, from the cup to rest.*

---

## Phase 3: The Oak Inn and the interface

*2026-09-26 / 2026-09-27 · Closed*

The first complete setting arrived: a warm tavern with candles, wood and a midnight-blue cloth. The interface was built on parchment, with a score sheet that rolls and unrolls, a main menu, pause, options and credits.

![The inn's table with its parchment score sheet.](media/fase-3/mesa.webp)

*The inn's table with its parchment score sheet.*

![With the sheet rolled up, the whole table is visible.](media/fase-3/enrollada.webp)

*With the sheet rolled up, the whole table is visible.*

![The first main menu.](media/fase-3/menu.webp)

*The first main menu.*

![The end-of-game screen on parchment.](media/fase-3/fin.webp)

*The end-of-game screen on parchment.*

![Scoring, sealing and rolling up the sheet.](media/fase-3/cartola.gif)

*Scoring, sealing and rolling up the sheet.*

---

## Phase 4: Audio

*2026-09-27 · Closed*

Every hit sounds according to the surface and the strength of the impact: cloth, wood, another die or the cup, and inside the cup dice-on-dice hits sound muffled. Most sounds were synthesised for the game; the music and the tavern ambience carry on without cuts from the menu into the game. The play surface became a rough baize, like a pool table, both in look and in sound.

![The cloth before and after: fibre relief and fabric sheen.](media/fase-4/pano.webp)

*The cloth before and after: fibre relief and fabric sheen.*

![Volume per channel: effects, music and ambience.](media/fase-4/opciones.webp)

*Volume per channel: effects, music and ambience.*

![The credits, with the music and sound section.](media/fase-4/creditos.webp)

*The credits, with the music and sound section.*

---

## Phase 5: Art and the pieces system

*2026-09-27 / 2026-09-28 · Closed*

Original models and textures for everything on the table. The game was organised into interchangeable pieces (dice, cup, score sheet, ambience, music, cursor) that bring looks and sound, never physics, and «Decorate the table» arrived to place objects around the tray.

![The inn with original art and the score sheet resting on the table.](media/fase-5/mesa.webp)

*The inn with original art and the score sheet resting on the table.*

![Boxwood and bone dice.](media/fase-5/dados.webp)

*Boxwood and bone dice.*

![«Decorate the table»: objects are dragged and rotated.](media/fase-5/decorar.webp)

*«Decorate the table»: objects are dragged and rotated.*

![Combinations of pieces on the same table.](media/fase-5/combinaciones.webp)

*Combinations of pieces on the same table.*

![The main menu with the table behind it.](media/fase-5/menu.webp)

*The main menu with the table behind it.*

![From the menu into the game in a single camera move.](media/fase-5/transicion.gif)

*From the menu into the game in a single camera move.*

---

## Phase 6: Economy, shop and a second world

*2026-09-28 / 2026-10-02 · Closed*

Every finished game pays out coins, spent in a shop where items can be tried on live. Daily and weekly missions arrived, along with a records board per rule set and the second world, Frutiger Aero: a meadow under a glass table, next to a lake with glass buildings, bubbles, fish and auroras.

![The open-air Frutiger Aero mock-up.](media/fase-6/maqueta-aero.webp)

*The open-air Frutiger Aero mock-up.*

![Frutiger Aero, finished: a glass table over the meadow.](media/fase-6/aero.webp)

*Frutiger Aero, finished: a glass table over the meadow.*

![Aquamarine resin dice and bone dice.](media/fase-6/dados-aero.webp)

*Aquamarine resin dice and bone dice.*

![Auroras and buildings reflected in the water.](media/fase-6/auroras.webp)

*Auroras and buildings reflected in the water.*

![The records board, one rule set per tab.](media/fase-6/records.webp)

*The records board, one rule set per tab.*

![Bubbles rising from the grass.](media/fase-6/burbujas.gif)

*Bubbles rising from the grass.*

---

## Phase 6B: Third world: the noir office

*2026-10-02 / 2026-10-04 · Closed*

«Midnight Agency», a 1940s detective's office: a hanging lamp, blinds, neon, rain on the window and cigarette smoke. The score sheet is a case file typed out key by key, and a black-and-white comic palette turns the scene into ink.

![The mock-up, with the neon on.](media/fase-6b/maqueta.webp)

*The mock-up, with the neon on.*

![The detective's desk, ready to roll.](media/fase-6b/mesa.webp)

*The detective's desk, ready to roll.*

![The score sheet as a case file.](media/fase-6b/expediente.webp)

*The score sheet as a case file.*

![The Ink palette: black-and-white comic style.](media/fase-6b/tinta.webp)

*The Ink palette: black-and-white comic style.*

![Looking around: the office in the dark.](media/fase-6b/sala.webp)

*Looking around: the office in the dark.*

![Scoring on the typewriter.](media/fase-6b/anotar.gif)

*Scoring on the typewriter.*

---

## Phase 6C: Fourth world: Fonda El Cacho

*2026-10-13 / 2026-10-15 · Closed*

A Chilean Independence Day fonda, in the afternoon: a leather dice cup (the «cacho»), a chalkboard written in chalk, a copihue-flower tablecloth, bunting, kites, smoke from the grill and food as table objects. An organ grinder walks by now and then.

![The fonda's table, with empanadas and anticuchos.](media/fase-6c/mesa.webp)

*The fonda's table, with empanadas and anticuchos.*

![The chalkboard as the score sheet.](media/fase-6c/pizarra.webp)

*The chalkboard as the score sheet.*

![The dice on the red cloth.](media/fase-6c/dados.webp)

*The dice on the red cloth.*

![The table objects: food, drinks and games.](media/fase-6c/objetos.webp)

*The table objects: food, drinks and games.*

![Looking around: the grill and the flags.](media/fase-6c/sala.webp)

*Looking around: the grill and the flags.*

![Scoring in chalk on the board.](media/fase-6c/tiza.gif)

*Scoring in chalk on the board.*

---

## Phase 7A: Versus the AI and two players

*2026-10-16 / 2026-10-17 · Closed*

The first step towards multiplayer: against the AI, at three difficulty levels, or two people on the same computer. The AI plays with the same physics as the player, with readable pauses, and the hardest level computes the exact value of every hold. The score sheet has one column per player in each world's style; in Frutiger Aero it is a chat conversation.

![Choosing the mode: solo, against the AI or two players.](media/fase-7a/modos.webp)

*Choosing the mode: solo, against the AI or two players.*

![Two columns on the inn's score sheet.](media/fase-7a/posada-dos.webp)

*Two columns on the inn's score sheet.*

![The noir case file with two detectives.](media/fase-7a/noir-dos.webp)

*The noir case file with two detectives.*

![In Frutiger Aero, the game is a conversation.](media/fase-7a/aero-dos.webp)

*In Frutiger Aero, the game is a conversation.*

![Each player types into their own column.](media/fase-7a/maquina-dos.gif)

*Each player types into their own column.*

---

## Phase M: Android

*2026-10-17 / 2026-10-29 · In progress*

The full game on an Android phone, in landscape and played with a finger, as a personal build that is not published in any store. Roll by dragging from the cup, zoom with two fingers, and buttons slide in from the sides after each roll to hold dice and score. Graphics have their own phone preset, measured world by world, and in «Decorate the table» objects are dragged with a finger from the list.

![The game as-is on the phone, before adapting it.](media/fase-m/tal-cual.webp)

*The game as-is on the phone, before adapting it.*

![Buttons to hold and score, with a fingertip drawn to scale.](media/fase-m/posada.webp)

*Buttons to hold and score, with a fingertip drawn to scale.*

![Scoring in two taps: the first one marks the box.](media/fase-m/noir.webp)

*Scoring in two taps: the first one marks the box.*

![«Contemplate the table»: just the scene, to look around.](media/fase-m/contemplar.webp)

*«Contemplate the table»: just the scene, to look around.*

![The buttons slide in and out from the sides.](media/fase-m/botones.gif)

*The buttons slide in and out from the sides.*

![From the inventory to the table, dragging with a finger.](media/fase-m/decorar.webp)

*From the inventory to the table, dragging with a finger.*

---

[Back to the start](README.en.md) · [Roadmap](ROADMAP.md)
