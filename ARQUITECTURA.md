**Español** · [English](ARCHITECTURE.md)

# Arquitectura

ParaDice of Fortune está hecho en Godot 4 con GDScript de tipado estático. Esta página resume cómo está organizado y las decisiones de diseño detrás; el código no se publica.

## Cuatro capas

1. **Núcleo puro.** Las reglas, la partida, la tabla de puntaje, los jugadores, la economía, las misiones y la IA son objetos simples, sin nodos de escena. Toda acción (tirar, guardar un dado, anotar) se valida ahí: una acción ilegal se rechaza y se avisa, nunca queda a medias. Una partida en curso se guarda como la lista de acciones del jugador y, al retomarla, esas acciones se reproducen con las mismas validaciones.
2. **Servicios.** El audio, las opciones, el guardado y el catálogo de piezas son servicios globales. El perfil está versionado, se migra entre versiones y se escribe de forma atómica: un cierre inesperado nunca lo deja a medio escribir.
3. **Contenido como datos.** Piezas, mundos, sonidos, misiones, precios y la configuración de la IA son recursos, no constantes en el código: un mundo se agrega o se ajusta sin tocar la lógica.
4. **Presentación.** La escena, la cámara, el vaso y los dados, la tabla y la interfaz. Un único controlador orquesta el flujo y le pregunta al núcleo si cada acción es legal.

## El sistema de piezas

La mesa se arma con **ranuras** intercambiables: dados, vaso, bandeja, botones, mesa, tabla de puntaje, ambiente, música y cursor. Cada pieza aporta aspecto y sonido, **nunca física**: los cuerpos de colisión son los mismos en todos los mundos, así que cambiar de mundo nunca cambia las probabilidades. Cada sonido pertenece a la pieza que lo produce, y los acabados cambian colores o materiales de una pieza sin crear otra.

Sobre las piezas van los **objetos de la mesa** (una calavera, una lámpara de lava, empanadas), que se colocan en «Decorar la mesa», y los **espacios de la mesa**: una mesa completa por mundo, que se cambia en medio de la partida.

## La física de los dados

- Física real a 120 pasos por segundo, con el vaso movido por código para que los dados hereden su movimiento.
- Los dados entran al vaso con una rotación uniformemente aleatoria; el vaso tiene una colisión invisible con la forma de sus paredes, una tapa al agitar y un pivote en la boca al volcarse.
- Un dado vale la cara que apunta hacia arriba. Uno que queda montado o inclinado vale la cara que más se ve, y se queda donde cayó.
- Un dado que ya mostró su cara queda quieto hasta resolver la tirada: los dados en reposo nunca se relanzan ni reciben empujones.

## Justicia medida

La justicia de los dados es un test, no una promesa. La batería lanza los dados miles de veces por el camino real del mouse y comprueba la distribución de las caras con una prueba de chi cuadrado, junto con los tiempos de cada tirada y que ningún dado salte después de quedar en reposo. Cada juego de dados nuevo puede pasar por la misma prueba.

## La IA

Tres niveles. El fácil es un jugador razonable: guarda el valor más repetido y anota la casilla que más vale. El medio y el difícil calculan el valor exacto de la ronda: cada mano posible, cada retención y sus transiciones, con cero, una y dos tiradas por delante. El difícil pesa además el bono superior mientras siga al alcance. La IA juega por la misma interfaz que una persona, con física real y pausas legibles.

## Táctil

En el teléfono, un modo táctil reemplaza al mouse: se tira arrastrando desde el vaso, con dos dedos se acerca y se mira alrededor, unos botones a los costados guardan dados y anotan, y el modo «contemplar» deja solo la mesa para mirarla. Los tamaños se expresan en milímetros de pantalla, así se mantienen con cualquier resolución.

## Tests

Más de noventa tests automáticos, de unidad y de integración, corren antes de cada entrega. El ejecutor trata como fallo cualquier error, advertencia o fuga de memoria, y puede comprobar que cada test falla de verdad cuando se fuerza una aserción.

---

[Volver al inicio](README.md)
