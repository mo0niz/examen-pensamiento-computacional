# examen-pensamiento-computacional
# Galaxia Interactiva

## Información del proyecto

**Nombre del proyecto:** Galaxia Interactiva

**Autor:** Isidora Muñoz

### Descripción general

Galaxia Interactiva es una experiencia interactiva desarrollada en p5.js que integra la cámara web para convertir al usuario en parte de un universo digital. A través de partículas dinámicas y la interacción mediante el mouse, el proyecto busca generar una experiencia visual inmersiva donde el usuario modifica constantemente el comportamiento del sistema.



# Descripción objetiva

## ¿Qué es el proyecto?

Es una experiencia de programación creativa donde el usuario interactúa con un universo de partículas generado en tiempo real sobre la imagen capturada por la cámara web.



## ¿Qué se ve en pantalla?

El proyecto está dividido en tres estados:

- Pantalla de inicio con el título del proyecto y un botón para comenzar.
- Experiencia interactiva donde la cámara muestra al usuario y aparecen partículas sobre la imagen.
- Pantalla final con un mensaje que indica el término de la experiencia y permite reiniciarla.



## ¿Qué elementos visuales aparecen?

- Cámara web en tiempo real.
- Partículas circulares.
- Fondo oscuro con estética espacial.
- Tipografía LEDLIGHT.
- Botón de inicio.
- Mensajes de inicio y final.



## ¿Qué inputs utiliza?

- Cámara web.
- Movimiento horizontal del mouse.
- Movimiento vertical del mouse.
- Click del mouse.
- Tecla R.



## ¿Qué outputs genera?

- Imagen en vivo del usuario.
- Aparición continua de partículas.
- Cambios de tamaño según la posición del mouse.
- Cambios de color según la posición del mouse.
- Cambio de estado de la experiencia.



# Descripción conceptual

## Idea central

El proyecto busca que el usuario deje de ser un simple observador y pase a formar parte de una galaxia digital. Mediante la cámara y la interacción con el mouse, el sistema responde en tiempo real, creando una experiencia donde el usuario influye directamente en el comportamiento visual del entorno.



## Corriente o referente de diseño

La propuesta se inspira en el arte generativo y el diseño interactivo, donde las imágenes son creadas mediante algoritmos y responden a la participación del usuario.



## Referentes visuales, históricos o teóricos

- Arte generativo.
- Programación creativa con p5.js.
- Instalaciones inmersivas de teamLab.
- Obras digitales de Refik Anadol.
- Imágenes astronómicas del espacio profundo.



## Principio de diseño explorado

El proyecto explora principalmente el principio de **interactividad**, ya que el usuario modifica constantemente el comportamiento del sistema mediante sus acciones.

También se trabajan principios como:

- Movimiento.
- Ritmo.
- Contraste.
- Jerarquía visual.
- Profundidad.



# Sistema computacional

## Inputs

- Cámara web.
- Mouse X.
- Mouse Y.
- Click del mouse.
- Tecla R.



## Procesos

El sistema recibe información del usuario y la procesa mediante funciones propias de p5.js.

La posición horizontal del mouse modifica el tamaño de las partículas utilizando `map()`.

La posición vertical modifica el color de las partículas.

Las partículas son distribuidas aleatoriamente mediante `random()`.

El tiempo controla automáticamente el cambio de estado utilizando `millis()`.



## Estados

### Estado 1

Pantalla de inicio.

### Estado 2

Experiencia interactiva.

### Estado 3

Pantalla final.



## Eventos

- `mousePressed()`
- `keyPressed()`



## Outputs

- Cámara en tiempo real.
- Partículas.
- Cambios de tamaño.
- Cambios de color.
- Cambio automático de estado.
- Mensajes visuales.



# Explicación de la interacción

## ¿Qué datos entran al sistema?

- Imagen capturada por la cámara.
- Posición horizontal del mouse.
- Posición vertical del mouse.
- Click del usuario.
- Presión de la tecla R.



## ¿Cómo se procesan?

El programa interpreta la información mediante variables, condicionales y funciones.

La posición del mouse es convertida mediante `map()` para controlar el tamaño y el color de las partículas.

Las partículas son generadas continuamente mediante un bucle `for`.



## ¿Cómo se transforman?

Los datos ingresados por el usuario son transformados en cambios visuales.

El movimiento horizontal controla el tamaño.

El movimiento vertical controla el color.

El clic duplica temporalmente el tamaño de las partículas.



## ¿Qué respuestas producen?

El sistema responde mostrando cambios inmediatos en la composición visual.

Cada usuario genera una experiencia distinta dependiendo de cómo interactúe con la cámara y el mouse.



# Recursos multimedia utilizados

## Tipo de recurso utilizado

- Cámara web.
- Tipografía personalizada (.otf).



## Función que cumple dentro del proyecto

La cámara integra al usuario dentro de la composición visual, convirtiéndolo en parte de la galaxia.

La tipografía aporta identidad visual y refuerza la estética tecnológica del proyecto.



# Registro visual

## Referentes

Como inspiración se utilizaron referentes de arte generativo, instalaciones interactivas y visualizaciones digitales del espacio.




## Bocetos

Se realizaron bocetos para definir la estructura de los tres estados y la distribución general de los elementos visuales. Más que solo bocetos en plan dibujos, se escribio previamente la idea e una libreta y de ahi fue siendo modificada. Necesite ayuda tanto de la misma pagina de p5js como de la Ia para entender un par de cosas, como el tener que esconder la camara, problema ocupando los segundos y aprendiendo a ocupar los milis.





## Iteraciones

El proyecto pasó por distintas versiones.

Inicialmente se trabajó con figuras geométricas simples.

Posteriormente se incorporó la cámara como fondo interactivo y finalmente se añadieron partículas dinámicas para reforzar el concepto de galaxia.



# Reflexión final

## Principales decisiones tomadas

La principal decisión fue utilizar la cámara como elemento central para integrar al usuario dentro de la experiencia.

También se decidió utilizar partículas simples para mantener un código ordenado y fácil de comprender, sin perder atractivo visual.

Finalmente, se organizó el programa mediante estados para facilitar la navegación entre las distintas etapas de la experiencia.



## Dificultades encontradas

Durante el desarrollo fue necesario aprender a utilizar la cámara mediante `createCapture()` e integrarla correctamente dentro del canvas.

Otra dificultad fue controlar la duración de la experiencia. Inicialmente se utilizó `second()`, pero posteriormente se reemplazó por `millis()`, ya que entrega una medición continua y evita errores cuando cambia el minuto.

No entendia algunos codigos por lo qu tuve que recurrir a ayuda externa, tanto de la misma pagina de p5js, como de internet (al buscar algunos colores, o para medir los milis) como tambien la ayuda de IA para poder preguntar cosas mas especificas y la ayuda de mis compañeros.

## Aprendizajes obtenidos

Este proyecto permitió comprender la importancia de organizar un programa mediante estados, funciones y eventos.

También reforzó el uso de variables, condicionales, bucles, funciones propias y funciones matemáticas como `map()` y `random()`.

Finalmente, permitió entender cómo la programación puede utilizarse como una herramienta de diseño para crear experiencias visuales donde el usuario participa activamente en la construcción de la obra.
## Imagenes
![Captura del proyecto 1](examen%20pensamiento/IMG_5484.jpg)

![Captura del proyecto 2](examen%20pensamiento/IMG_5485.jpg)

![Captura del proyecto 3](examen%20pensamiento/IMG_5486.jpg)

![Captura del proyecto 4](examen%20pensamiento/IMG_5490.jpg)

![Captura del proyecto 5](examen%20pensamiento/IMG_5492.jpg)

![Captura del proyecto 6](examen%20pensamiento/IMG_5493.jpg)

![Captura del proyecto 7](examen%20pensamiento/IMG_5494.jpg)

![Captura del proyecto 8](examen%20pensamiento/IMG_5496.jpg)

![Captura del proyecto 9](examen%20pensamiento/IMG_5497.jpg)

![Captura del proyecto 10](examen%20pensamiento/IMG_5499.jpg)

---

## 📊 Diagrama de Flujo

[👉 Haz clic aquí para ver o descargar el Diagrama de Flujo (PDF)](examen%20pensamiento/diagrama%20de%20fluje.pdf)


## P5JS

(https://editor.p5js.org/isidora.munoz9/full/LbaF4a2Bl)

https://editor.p5js.org/isidora.munoz9/sketches/LbaF4a2Bl
