Sopa de Letras en C

Este programa genera una sopa de letras en la que los jugadores pueden buscar palabras ocultas. A continuación, se describen las características, instrucciones de uso y detalles técnicos del programa.

Características

Tamaño Personalizable de la Matriz:

El usuario puede elegir el tamaño de la sopa de letras, con un límite entre 10x10 y 35x35.

Cantidad de Palabras a Esconder:

Se permite esconder entre N/2 y 2N palabras, donde N es el tamaño de la matriz.

Validación de Entrada:

Las palabras deben tener entre 2 y N caracteres.

Se permite únicamente el uso de caracteres alfabéticos.

Orientaciones de Palabras:

Las palabras pueden aparecer en las siguientes orientaciones:

Vertical (arriba hacia abajo o abajo hacia arriba).

Horizontal (izquierda a derecha o derecha a izquierda).

Interfaz de Juego:

Los jugadores ingresan palabras encontradas.

El programa valida las palabras ingresadas y proporciona retroalimentación sobre si son correctas.

Se informa la ubicación y orientación de las palabras encontradas.

Sistema de Puntuación:

Los jugadores tienen 3 vidas.

Se reduce una vida por cada palabra incorrecta ingresada.

El juego termina si se encuentran todas las palabras o si se pierden todas las vidas.

Tiempo de Juego:

Se mide y muestra el tiempo que tarda el jugador en completar la partida.

Cómo Usar el Programa

Requisitos

Un compilador de C (como GCC).

Un terminal o entorno de desarrollo que permita la entrada y salida estándar.

Instrucciones

Compilación:
Compile el programa utilizando el siguiente comando:

gcc sopa.c -o sopa_de_letras

Ejecución:
Ejecute el programa:

./sopa_de_letras

Configuración Inicial:

Introduzca el tamaño de la matriz (entre 10 y 35).

Especifique la cantidad de palabras a esconder (entre N/2 y 2N).

Ingrese cada palabra siguiendo las reglas establecidas (alfabéticas y en mayúsculas o minúsculas).

Juego:

Encuentre y escriba las palabras ocultas una por una.

Reciba retroalimentación sobre palabras correctas o incorrectas.

Siga jugando hasta ganar o perder.

Fin del Juego:

El programa muestra un mensaje indicando si ganó o perdió.

Se informa el tiempo total transcurrido durante el juego.

Detalles Técnicos

Generación de Matriz:

Se llena inicialmente con caracteres vacíos (32).

Las palabras se colocan de forma aleatoria siguiendo las reglas de orientación.

Las posiciones vacías se rellenan con letras aleatorias (A-Z).

Validaciones:

Las entradas del usuario son verificadas para evitar caracteres no permitidos.

Las palabras ya encontradas se eliminan para evitar duplicados.

Manejo de Colisiones:

Se realizan hasta 1000 intentos para colocar cada palabra en la matriz.

Si no se encuentra espacio, la palabra es ignorada.

Control de Tiempo:

El programa mide el tiempo transcurrido desde el inicio hasta el final del juego para proporcionar estadísticas adicionales al jugador.

