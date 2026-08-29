# Roles y responsabilidades

La asignación inicial comprende 16 estudiantes únicos. Algunas personas aparecen en más de un rol porque colaborarán en distintas etapas.

> Los nombres son provisionales y se actualizarán cuando estén disponibles los nombres y apellidos completos.

## Diseño

**Integrantes:** Ian, Nahuel, Tomy, Uma, Mia, Montes y Lauti.

Responsabilidades:

- definir la mecánica exacta y el objetivo del juego;
- diseñar escenas, niveles y progresión;
- acordar controles, feedback y presentación visual;
- definir el mensaje cuando se trabaje con la opción B;
- entregar decisiones claras a Código y Prompt/IA.

## Código

**Integrantes:** Agustin, Ary, Nahuel, Lauti y Montes.

Responsabilidades:

- construir las escenas y scripts en Godot 4;
- dividir el trabajo por subsistemas;
- revisar el GDScript generado con asistencia de IA;
- mantener escenas separadas para reducir conflictos;
- probar cada subsistema antes de integrarlo.

Una persona del grupo será designada **Responsable de Integración** al comenzar cada práctica. No es un rol separado: es una responsabilidad adicional.

## Prompt / IA

**Integrantes:** Sebastian, Agus, Nahuel, Lorax y Valentina.

Responsabilidades:

- ayudar a convertir necesidades concretas en prompts verificables;
- generar borradores de GDScript compatibles con Godot 4;
- producir assets visuales provisionales;
- documentar qué generó la IA y cómo debe probarse;
- revisar junto con Código que cada resultado funcione realmente.

## Test

**Integrantes:** Fran, Godoy, Lorax, Valentina y Dani.

Responsabilidades:

- probar builds parciales desde el minuto 30;
- registrar pasos claros para reproducir cada bug;
- verificar colisiones, layers, controles y límites de pantalla;
- comprobar victoria, derrota, reinicio, vidas, puntaje y temporizadores;
- volver a verificar los bugs corregidos.

## Cast

**Integrantes:** Sebastian, Lorax, Godoy y Tomy.

Responsabilidades:

- preparar desde el inicio la explicación del juego;
- registrar qué mecánica se eligió y por qué;
- reunir capturas, controles y puntos clave de la demostración;
- colaborar con Test mientras se desarrolla el juego;
- ensayar la presentación final.

## Responsable de Integración

Se designa al comenzar la práctica entre las personas de Código.

Responsabilidades:

- definir el orden de integración de subsistemas;
- revisar y fusionar pull requests;
- coordinar cambios sobre escenas compartidas;
- resolver conflictos o pedir ayuda para resolverlos;
- anunciar en Discord el comienzo y final de cada integración;
- mantener `main` en un estado ejecutable.

## Subsistemas sugeridos

| Subsistema | Nodos habituales | Responsabilidad |
|---|---|---|
| Jugador | `CharacterBody2D`, `Area2D`, `Sprite2D` | Movimiento, input y animación básica. |
| Spawner | `Timer`, `Node2D` | Generación de obstáculos, ítems o enemigos. |
| Puntaje / UI | `CanvasLayer`, `Label` | Puntaje, vidas, tiempo y feedback en pantalla. |
| Colisiones / Game Over | señales de `Area2D` | Interacciones, daño, victoria y derrota. |
| Pantalla final | `Control`, `Button` | Resultado y reinicio de la partida. |
