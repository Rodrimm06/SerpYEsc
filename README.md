Implementación de "Serpientes y Escaleras" en C++ usando programación orientada a objetos.

1.- Soporta a dos jugadores, los cuales podrán interactuar escribiendo la letra C para continuar con su turno, o E para terminar el juego, cualquier otra respuesta será vista como un error.
2.- El juego termina cuando un jugador llega a la casilla final, presiona la letra E o se llega al limite de turnos.
3.- El output que recibe el jugador es <turno, # de jugador, posición anterior, valor del dado, tipo de casilla, posición final>
4.- El tablero tiene un total de 30 casillas, siendo tres de estas serpientes y tres escaleras

Justificación POO

Encapsulamiento: El usuario no tiene acceso directo a los atributos privados, y solo puede interactuar de cierta forma con el programa, pudiendo únicamente iniciar, continuar o terminar un juego.
Single responsibility: Cada clase se encarga de algo en específico, dice solo se encarga de generar un numero aleatorio y la clase MyGame solo se encarga de la lógica del juego.
Abstracción: Se buscó hacerlo de una forma simple, evitando la complejidad innecesaria, además de colocar comentarios para expresar lo que se buscaba hacer, un ejemplo es usar un tablero unidimensional en vez de uno bidimensional.

Especificaciones
Jugadores: 2
Tablero: Arreglo unidimensional de 30 espacios
Límite de turnos: 20
Serpientes: Casilla 6,13 y 24
Escaleras: Casillas 8, 17 y 22

Justificación de diseño
Se opto por un arreglo unidimensional porque este es más fácil de recorrer en cada turno, dado que es lineal.
Se pusieron posiciones fijas de serpientes y escaleras para que no interactúen unas con otras o se "salgan" del tablero.
La clase dice es parte de la clase MyGame para sacar un valor aleatorio, y así cada clase hace algo específico y no una hace todo

Rodrigo Medina Medrano - A00841682
