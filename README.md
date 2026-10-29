# Juego 1

## Descripción del repositorio

En este repositorio se encuentra el archivo `paint.py`, que contiene el código del videojuego Paint, así como el archivo `README.md`, donde 
explicamos las modificaciones realizadas.

Originalmente, el juego permitía dibujar líneas y cuadrados. Durante esta actividad modificamos el código para agregar nuevas figuras, como 
rectángulos y triángulos.

## Modificaciones realizadas

### 1. Completar el rectángulo

Para dibujar el rectángulo, primero agregamos las instrucciones `up()`, `goto()`, `down()` y `begin_fill()`, que permiten levantar el 
lápiz, posicionarlo en el punto inicial, bajarlo y comenzar a definir la figura que se va a rellenar.

Después agregamos cuatro instrucciones `goto()` que utilizan las coordenadas iniciales y finales para formar los cuatro lados 
del rectángulo. Cada instrucción mueve el lápiz hacia una esquina diferente hasta regresar al punto inicial y cerrar la 
figura. Finalmente, utilizamos `end_fill()` para rellenar el rectángulo.

### 2. Completar el triángulo

Para dibujar el triángulo utilizamos las mismas cuatro instrucciones iniciales que en el rectángulo, pero en este caso solo necesitamos 
formar tres lados.

Primero utilizamos `goto(end.x, start.y)` para dibujar la base horizontal. Después, `goto(end.x, end.y)` para formar el lado 
vertical y finalmente `goto(start.x, start.y)` para crear la línea diagonal que regresa al punto inicial.

De esta manera conseguimos formar un triángulo rectángulo y utilizamos `end_fill()` para rellenar.


