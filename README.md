**Español** · [English](README.en.md)

# ParaDice of Fortune

Un juego de dados 3D basado en Yacht, el antecesor de dominio público de Yahtzee y la Generala, hecho en Godot 4 con GDScript. Se toma el vaso, se agita y se sueltan los dados sobre una mesa con física real; después se guardan los dados que interesan, se vuelve a tirar hasta tres veces y se anota en la tabla.

Cada mesa pertenece a un **mundo** con aspecto, sonido y vida propios: una posada fantástica a la luz de las velas, una pradera Frutiger Aero bajo una mesa de vidrio, el despacho de un detective de los años 40 y una fonda chilena de Fiestas Patrias.

![Una partida contra la IA](media/hero.gif)

*Una partida contra la IA en la Posada del Roble.*

> Este es un repositorio **de vitrina**: guarda capturas, la evolución del proyecto y su hoja de ruta. El código, las escenas, los modelos, las texturas y el audio del juego no se publican aquí.

## Dónde está

- Solitario, contra la IA (tres dificultades) o dos jugadores en el mismo equipo.
- Dos reglamentos: Yacht clásico con bono superior y Yacht moderno.
- Cuatro mundos terminados, cada uno con sus piezas, objetos de la mesa, sala, ambiente y música.
- Monedas, tienda, misiones diarias y semanales, y tablón de récords.
- Español e inglés.
- Windows (con mouse) y, en curso, una versión personal para Android que se juega con el dedo.

## Fases

| Fase | Título | Fechas | Estado |
|---|---|---|---|
| 0 | [Auditoría y dirección visual](EVOLUCION.md#fase-0-auditoría-y-dirección-visual) | 2026-09-26 | Cerrada |
| 1 | [Cimientos](EVOLUCION.md#fase-1-cimientos) | 2026-09-26 | Cerrada |
| 2 | [Núcleo jugable](EVOLUCION.md#fase-2-núcleo-jugable) | 2026-09-26 | Cerrada |
| 3 | [La Posada del Roble e interfaz](EVOLUCION.md#fase-3-la-posada-del-roble-e-interfaz) | 2026-09-26 / 2026-09-27 | Cerrada |
| 4 | [Audio](EVOLUCION.md#fase-4-audio) | 2026-09-27 | Cerrada |
| 5 | [Arte y sistema de piezas](EVOLUCION.md#fase-5-arte-y-sistema-de-piezas) | 2026-09-27 / 2026-09-28 | Cerrada |
| 6 | [Economía, tienda y segundo mundo](EVOLUCION.md#fase-6-economía-tienda-y-segundo-mundo) | 2026-09-28 / 2026-10-02 | Cerrada |
| 6B | [Tercer mundo: el despacho noir](EVOLUCION.md#fase-6b-tercer-mundo-el-despacho-noir) | 2026-10-02 / 2026-10-04 | Cerrada |
| 6C | [Cuarto mundo: la Fonda El Cacho](EVOLUCION.md#fase-6c-cuarto-mundo-la-fonda-el-cacho) | 2026-10-13 / 2026-10-15 | Cerrada |
| 7A | [Contra la IA y dos jugadores](EVOLUCION.md#fase-7a-contra-la-ia-y-dos-jugadores) | 2026-10-16 / 2026-10-17 | Cerrada |
| M | [Android](EVOLUCION.md#fase-m-android) | 2026-10-17 / 2026-10-29 | En curso |
| 7B | En línea, 1 contra 1 | — | Planificada |
| 7C | De 3 a 4 jugadores | — | Planificada |
| 8 | Progresión y final del juego | — | Planificada |
| 9 | Quinto mundo: la cripta gótica | — | Planificada |

## Mundos

### [La Posada del Roble](worlds/posada.es.md)

[![La Posada del Roble](media/worlds/posada/mesa.webp)](worlds/posada.es.md)

### [Frutiger Aero](worlds/aero.es.md)

[![Frutiger Aero](media/worlds/aero/mesa.webp)](worlds/aero.es.md)

### [Agencia Medianoche (despacho noir)](worlds/noir.es.md)

[![Agencia Medianoche (despacho noir)](media/worlds/noir/mesa.webp)](worlds/noir.es.md)

### [Fonda El Cacho](worlds/fonda.es.md)

[![Fonda El Cacho](media/worlds/fonda/mesa.webp)](worlds/fonda.es.md)

## Más

- [Evolución](EVOLUCION.md): fase por fase, con imágenes.
- [Hoja de ruta](HOJA_DE_RUTA.md): lo que viene.
- [Arquitectura](ARQUITECTURA.md): cómo está organizado el juego.

Última actualización: 2026-10-29.

© 2026 Ignacio Díaz. Todos los derechos reservados: ver [LICENSE](LICENSE).
