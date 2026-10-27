**Español** · [English](EVOLUTION.md)

# Evolución

Cómo creció ParaDice of Fortune, fase por fase. Cada fase termina con la batería de tests automáticos en verde, el juego jugable de principio a fin y la revisión del dueño.

## Fase 0: Auditoría y dirección visual

*2026-09-26 · Cerrada*

El punto de partida fue un prototipo heredado: jugable, pero frágil y sin identidad. Se revisó entero, se acordó un remake completo y se probaron tres direcciones visuales con maquetas dentro del motor: una posada fantástica a la luz de las velas, la tablilla de un tabernero y una piel Frutiger Aero. Ganó la posada, con la luz de luna y los dados de boj de la segunda.

![El prototipo heredado, antes del remake.](media/fase-0/prototipo.webp)

*El prototipo heredado, antes del remake.*

![Maqueta A: la Posada del Roble, la dirección elegida.](media/fase-0/maqueta-a-posada.webp)

*Maqueta A: la Posada del Roble, la dirección elegida.*

![Maqueta B: la tablilla del tabernero, con luz de luna.](media/fase-0/maqueta-b-tablilla.webp)

*Maqueta B: la tablilla del tabernero, con luz de luna.*

![Maqueta C: la primera idea de Frutiger Aero.](media/fase-0/maqueta-c-aero.webp)

*Maqueta C: la primera idea de Frutiger Aero.*

![Las tres propuestas, lado a lado.](media/fase-0/propuestas.webp)

*Las tres propuestas, lado a lado.*

---

## Fase 1: Cimientos

*2026-09-26 · Cerrada*

Las reglas pasaron a un núcleo puro, separado de lo que se ve en pantalla, y se probaron con miles de partidas simuladas. Los tests automáticos fallan ante cualquier error, advertencia o fuga de memoria. El perfil se guarda de forma atómica y el juego habla español e inglés desde el primer día.

![La mesa sobre el núcleo nuevo, todavía con el arte heredado.](media/fase-1/inicio.webp)

*La mesa sobre el núcleo nuevo, todavía con el arte heredado.*

![La tabla de puntaje, ahora una vista pura de la partida.](media/fase-1/cartola.webp)

*La tabla de puntaje, ahora una vista pura de la partida.*

![Fin de partida con el récord guardado en el perfil.](media/fase-1/fin.webp)

*Fin de partida con el récord guardado en el perfil.*

![La misma partida en inglés.](media/fase-1/ingles.webp)

*La misma partida en inglés.*

---

## Fase 2: Núcleo jugable

*2026-09-26 · Cerrada*

El vaso y los dados se rehicieron con física real: se toma el vaso, se agita y se suelta. Cada dado se lee por su cara de arriba, los que quedan montados o inclinados valen la cara que más se ve, y la justicia de las tiradas se mide con miles de lanzamientos reales.

![El vaso se vuelca y los dados ruedan.](media/fase-2/rodando.webp)

*El vaso se vuelca y los dados ruedan.*

![Dados guardados en el pedestal antes de volver a tirar.](media/fase-2/retenidos.webp)

*Dados guardados en el pedestal antes de volver a tirar.*

![A mitad de la partida.](media/fase-2/cartola.webp)

*A mitad de la partida.*

![Una tirada completa, del vaso al reposo.](media/fase-2/tirada.gif)

*Una tirada completa, del vaso al reposo.*

---

## Fase 3: La Posada del Roble e interfaz

*2026-09-26 / 2026-09-27 · Cerrada*

Llegó la primera ambientación completa: una taberna cálida con velas, madera y un tapete azul noche. La interfaz se construyó sobre pergamino, con la tabla que se enrolla y se desenrolla, menú principal, pausa, opciones y créditos.

![La mesa de la posada con su tabla de pergamino.](media/fase-3/mesa.webp)

*La mesa de la posada con su tabla de pergamino.*

![La tabla enrollada deja ver la mesa entera.](media/fase-3/enrollada.webp)

*La tabla enrollada deja ver la mesa entera.*

![El primer menú principal.](media/fase-3/menu.webp)

*El primer menú principal.*

![El fin de partida sobre pergamino.](media/fase-3/fin.webp)

*El fin de partida sobre pergamino.*

![Anotar, sellar y enrollar la tabla.](media/fase-3/cartola.gif)

*Anotar, sellar y enrollar la tabla.*

---

## Fase 4: Audio

*2026-09-27 · Cerrada*

Cada golpe suena según la superficie y la fuerza del choque: paño, madera, otro dado o el vaso, y dentro del vaso el choque entre dados suena apagado. Casi todos los sonidos se sintetizaron para el juego; la música y el ambiente de la taberna siguen sin cortes del menú a la partida. El tapete pasó a ser un paño rugoso, como el de una mesa de pool, en la imagen y en el sonido.

![El paño antes y después: relieve de fibra y brillo de tela.](media/fase-4/pano.webp)

*El paño antes y después: relieve de fibra y brillo de tela.*

![Volumen por canal: efectos, música y ambiente.](media/fase-4/opciones.webp)

*Volumen por canal: efectos, música y ambiente.*

![Los créditos, con la sección de música y sonido.](media/fase-4/creditos.webp)

*Los créditos, con la sección de música y sonido.*

---

## Fase 5: Arte y sistema de piezas

*2026-09-27 / 2026-09-28 · Cerrada*

Modelos y texturas propios para todo lo que está sobre la mesa. El juego se ordenó en piezas intercambiables (dados, vaso, tabla, ambiente, música, cursor) que aportan aspecto y sonido, nunca física, y apareció «Decorar la mesa» para poner objetos alrededor de la bandeja.

![La posada con arte propio y la tabla apoyada sobre la mesa.](media/fase-5/mesa.webp)

*La posada con arte propio y la tabla apoyada sobre la mesa.*

![Dados de boj y de hueso.](media/fase-5/dados.webp)

*Dados de boj y de hueso.*

![«Decorar la mesa»: los objetos se arrastran y se giran.](media/fase-5/decorar.webp)

*«Decorar la mesa»: los objetos se arrastran y se giran.*

![Combinaciones de piezas sobre la misma mesa.](media/fase-5/combinaciones.webp)

*Combinaciones de piezas sobre la misma mesa.*

![El menú principal con la mesa de fondo.](media/fase-5/menu.webp)

*El menú principal con la mesa de fondo.*

![Del menú a la partida en un solo movimiento de cámara.](media/fase-5/transicion.gif)

*Del menú a la partida en un solo movimiento de cámara.*

---

## Fase 6: Economía, tienda y segundo mundo

*2026-09-28 / 2026-10-02 · Cerrada*

Cada partida terminada paga monedas, que se gastan en una tienda con prueba en vivo. Llegaron las misiones diarias y semanales, el tablón de récords por reglamento y el segundo mundo, Frutiger Aero: una pradera bajo una mesa de vidrio, junto a un lago con edificios de cristal, burbujas, peces y auroras.

![La maqueta de Frutiger Aero al aire libre.](media/fase-6/maqueta-aero.webp)

*La maqueta de Frutiger Aero al aire libre.*

![Frutiger Aero producido: mesa de vidrio sobre la pradera.](media/fase-6/aero.webp)

*Frutiger Aero producido: mesa de vidrio sobre la pradera.*

![Dados de resina aguamarina y de hueso.](media/fase-6/dados-aero.webp)

*Dados de resina aguamarina y de hueso.*

![Auroras y edificios reflejados en el agua.](media/fase-6/auroras.webp)

*Auroras y edificios reflejados en el agua.*

![El tablón de récords, con un reglamento por pestaña.](media/fase-6/records.webp)

*El tablón de récords, con un reglamento por pestaña.*

![Burbujas que suben desde el pasto.](media/fase-6/burbujas.gif)

*Burbujas que suben desde el pasto.*

---

## Fase 6B: Tercer mundo: el despacho noir

*2026-10-02 / 2026-10-04 · Cerrada*

«Agencia Medianoche», el despacho de un detective de los años 40: lámpara colgante, persianas, neón, lluvia en la ventana y humo de cigarrillo. La tabla de puntaje es un expediente que se escribe a máquina, golpe a golpe, y una paleta en blanco y negro de cómic convierte la escena en tinta.

![La maqueta, con el neón encendido.](media/fase-6b/maqueta.webp)

*La maqueta, con el neón encendido.*

![El escritorio del detective, listo para tirar.](media/fase-6b/mesa.webp)

*El escritorio del detective, listo para tirar.*

![La tabla de puntaje como expediente.](media/fase-6b/expediente.webp)

*La tabla de puntaje como expediente.*

![La paleta Tinta: blanco y negro de cómic.](media/fase-6b/tinta.webp)

*La paleta Tinta: blanco y negro de cómic.*

![Mirando alrededor: el despacho a oscuras.](media/fase-6b/sala.webp)

*Mirando alrededor: el despacho a oscuras.*

![Anotar a máquina de escribir.](media/fase-6b/anotar.gif)

*Anotar a máquina de escribir.*

---

## Fase 6C: Cuarto mundo: la Fonda El Cacho

*2026-10-13 / 2026-10-15 · Cerrada*

Una fonda chilena de Fiestas Patrias, de tarde: el cacho de cuero como vaso, una pizarra escrita con tiza, mantel de copihues, guirnaldas, volantines, humo de la parrilla y comida como objetos de la mesa. Un organillero pasa de vez en cuando.

![La mesa de la fonda, con empanadas y anticuchos.](media/fase-6c/mesa.webp)

*La mesa de la fonda, con empanadas y anticuchos.*

![La pizarra como tabla de puntaje.](media/fase-6c/pizarra.webp)

*La pizarra como tabla de puntaje.*

![Los dados sobre el paño rojo.](media/fase-6c/dados.webp)

*Los dados sobre el paño rojo.*

![Los objetos de la mesa: comida, bebida y juegos.](media/fase-6c/objetos.webp)

*Los objetos de la mesa: comida, bebida y juegos.*

![Mirando alrededor: la parrilla y las banderas.](media/fase-6c/sala.webp)

*Mirando alrededor: la parrilla y las banderas.*

![Anotar con tiza en la pizarra.](media/fase-6c/tiza.gif)

*Anotar con tiza en la pizarra.*

---

## Fase 7A: Contra la IA y dos jugadores

*2026-10-16 / 2026-10-17 · Cerrada*

El primer paso del multijugador: contra la IA, en tres dificultades, o dos personas en el mismo equipo. La IA juega con la misma física que el jugador, con pausas legibles, y la de mayor dificultad calcula exactamente el valor de cada retención. La tabla de puntaje tiene una columna por jugador en el estilo de cada mundo; en Frutiger Aero es una conversación de chat.

![Elegir el modo: solitario, contra la IA o de a dos.](media/fase-7a/modos.webp)

*Elegir el modo: solitario, contra la IA o de a dos.*

![Dos columnas en la tabla de la posada.](media/fase-7a/posada-dos.webp)

*Dos columnas en la tabla de la posada.*

![El expediente del noir con dos detectives.](media/fase-7a/noir-dos.webp)

*El expediente del noir con dos detectives.*

![En Frutiger Aero, la partida es una conversación.](media/fase-7a/aero-dos.webp)

*En Frutiger Aero, la partida es una conversación.*

![Cada jugador anota a máquina en su columna.](media/fase-7a/maquina-dos.gif)

*Cada jugador anota a máquina en su columna.*

---

## Fase M: Android

*2026-10-17 / 2026-10-18 · En curso*

El juego completo en un teléfono Android, en horizontal y con el dedo, como una versión personal que no se publica en tiendas. Se tira arrastrando desde el vaso, se acerca y se aleja con dos dedos, y unos botones entran por los costados al terminar cada tirada para guardar dados y anotar. Falta afinar los gráficos y el rendimiento.

![El juego tal cual en el teléfono, antes de adaptarlo.](media/fase-m/tal-cual.webp)

*El juego tal cual en el teléfono, antes de adaptarlo.*

![Botones para guardar y anotar, con una yema de dedo a escala.](media/fase-m/posada.webp)

*Botones para guardar y anotar, con una yema de dedo a escala.*

![Anotar en dos toques: el primero marca la casilla.](media/fase-m/noir.webp)

*Anotar en dos toques: el primero marca la casilla.*

![«Contemplar la mesa»: solo la escena, para mirar.](media/fase-m/contemplar.webp)

*«Contemplar la mesa»: solo la escena, para mirar.*

![Los botones entran y salen por los costados.](media/fase-m/botones.gif)

*Los botones entran y salen por los costados.*

---

[Volver al inicio](README.md) · [Hoja de ruta](HOJA_DE_RUTA.md)
