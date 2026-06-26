# Examen-Pensamiento-Computacional-

# Información del proyecto

[link](https://editor.p5js.org/dannyy/sketches/Xp2ickMO2)

[link](https://editor.p5js.org/dannyy/full/Xp2ickMO2)




## Nombre del proyecto 
**Percepción Cinética: Sistema Interactivo de Figuras Generativas**

## Autora 
Daniela muñoz

## Descripción general 
Este proyecto es una experiencia digital interactiva desarrollada en p5.js que explora cómo la percepción del movimiento puede generarse a partir de figuras estáticas. A través de la interacción del usuario (mouse y teclado), una serie de composiciones geométricas se transforman dinámicamente, creando la sensación de movimiento, variación y respuesta visual en tiempo real.

El sistema está organizado en tres estados (inicio, experiencia y final), los cuales estructuran la navegación y la evolución de la experiencia visual.

# Descripcion objetiva 

## ¿Qué es el proyecto?
Es una instalación digital interactiva basada en código generativo que utiliza grillas de figuras geométricas para construir una experiencia visual dinámica. Estas figuras cambian según la interacción del usuario, generando un sistema visual reactivo.

## ¿Qué se ve en pantalla? 
El proyecto está dividido en tres pantallas:

- Pantalla de inicio: fondo negro con una grilla de círculos estáticos que funciona como introducción visual, acompañada de texto explicativo.
- Pantalla de experiencia: una grilla completa de figuras geométricas (círculos, cuadrados o rectángulos) que cambian en tiempo real según la interacción del usuario.
-  Pantalla final: una composición similar a la inicial, pero con menor densidad visual, acompañada de texto de cierre.

## ¿Qué elementos visuales aparecen?

- Círculos 
- Cuadrados
- Rectángulos
- Texto tipográfico explicativo e instructivo
- Grillas 
- Variaciones aleatorias en tamaño y forma

## ¿Qué inputs utiliza?
El sistema responde a múltiples entradas del usuario:

**Mouse**
- Movimiento horizontal (mouseX): controla el tamaño general de las figuras
- Movimiento vertical (mouseY): modifica la variación del tamaño
- Clic: alterna entre fondo claro y oscuro

**Teclado**
- ENTER: cambia entre pantallas (inicio - experiencia - final)
- ESPACIO: finaliza la experiencia
- Teclas 1, 2, 3 : cambian el tipo de figura

## ¿Qué outputs genera?
El sistema genera respuestas visuales y sonoras en tiempo real:

- Cambio dinámico de figuras geométricas
- Transformación del tamaño de los elementos
- Inversión de colores de fondo y figura
- Generación de variaciones aleatorias en cada figura
- Reproducción de sonido al cambiar el tipo de figura

# Descripción conceptual

## Idea central
La idea principal del proyecto es explorar cómo la interacción del usuario puede generar la percepción de movimiento a partir de elementos visuales estáticos. Aunque las figuras no se mueven físicamente, sus cambios constantes de tamaño, forma y distribución generan una ilusión cinética.


## Corriente o referente de diseño
Este proyecto se basa en el arte cinético, una corriente artística que busca generar la sensación de movimiento a través de elementos visuales estáticos o en movimiento real. En este caso, el movimiento no ocurre físicamente en los objetos, sino que se construye a partir de variaciones constantes en la composición visual, el ritmo y la repetición. El arte cinético se caracteriza por involucrar activamente la percepción del espectador, haciendo que el movimiento dependa de cómo el ojo interpreta los cambios visuales, principio que este proyecto replica mediante la interacción en tiempo real del usuario con la grilla de figuras.


## Principio de diseño explorado

- Repetición (grillas estructuradas)
- Variación (cambios aleatorios en tamaño)
- Contraste (blanco/negro)
- Interacción usuario-sistema
- Transformación en tiempo real

# Sistema computacional

## Inputs
El sistema recibe datos del usuario:

- Posición del mouse (mouseX, mouseY)
- Interacciones del mouse (clic)
- Teclas del teclado (ENTER, espacio, 1, 2, 3)

## Procesos
El sistema procesa la información mediante:

- Control de estados (estado) para cambiar pantallas
- Generación de grillas con bucles for
- Conversión de datos del mouse en parámetros visuales (map)
- Variación aleatoria de tamaño (random)
- Condiciones que determinan el tipo de figura (if / else)

## Estados
El proyecto funciona con tres estados principales:

- Estado 0: Pantalla de inicio
- Estado 1: Pantalla de experiencia interactiva
- Estado 2: Pantalla final

## Eventos
El sistema responde a eventos específicos:

- keyPressed(): controla navegación y cambios de figura
- mousePressed(): cambia esquema de color

## Outputs

- Imágenes generadas en tiempo real
- Composición visual dinámica
- Cambios de color y forma
- Reproducción de sonido

# Explicación de la interacción

## ¿Qué datos entran al sistema?
El sistema recibe información del usuario en forma de:

- coordenadas del mouse
- teclas presionadas
- clics del mouse

## ¿Cómo se procesan?
Estos datos se transforman en variables internas que modifican:

- tamaño de las figuras
- tipo de forma geométrica
- color del sistema
- estado de la experiencia


## ¿Cómo se transforman?
Los datos de entrada no se muestran directamente, sino que se convierten en parámetros visuales:

- posición del mouse: escala visual
- teclado: cambio de estructura
- clic: inversión cromática
- interacción: activación de sonido

## ¿Qué respuestas producen?
El sistema responde generando:

- cambios visuales inmediatos
- transformación de la composición
- sensación de movimiento continuo
- retroalimentación sonora

# Recursos multimedia utilizados

## Tipo de recurso utilizado

- Archivo de audio (.mp3)

## Función que cumple dentro del proyecto
El sonido funciona como retroalimentación interactiva. Se activa cada vez que el usuario cambia el tipo de figura, reforzando la relación entre acción y respuesta del sistema.

# Registro visual
El proyecto se inspira en sistemas visuales basados en:

- patrones geométricos repetitivos
- arte cinético y óptico
- diseño generativo digital

 Referentes 

 ![imagen](https://www.cinconoticias.com/wp-content/uploads/obras-de-arte-cinetico.jpg)
 ![imagen](https://tk-arte-cinetico.weebly.com/uploads/3/7/1/2/37126569/7082873.jpg?412)


  
# Reflexión final

Este proyecto fue un proceso de exploración donde fue importante organizar bien la lógica del sistema para que las distintas partes funcionaran de manera coherente. Uno de los principales desafíos fue coordinar los estados de la aplicación junto con la interacción del mouse y el teclado, ya que todo ocurre al mismo tiempo y debe mantenerse equilibrado para que la experiencia sea clara.

También fue interesante observar cómo pequeñas variables como la posición del mouse o el uso de valores aleatorios pueden modificar completamente la percepción visual del sistema. Esto hizo necesario probar varias configuraciones hasta lograr un resultado estable y consistente. La integración del sonido también requirió ajustes, especialmente para controlar cuándo debía activarse sin interrumpir la interacción visual.

En general, el proyecto permitió profundizar en la relación entre código, interacción y percepción visual, entendiendo cómo el usuario puede influir directamente en la construcción de la experiencia. Más allá de lo técnico, fue un ejercicio para seguir explorando cómo el diseño puede generar sistemas dinámicos que responden en tiempo real.

# Diagrama de flujo 



