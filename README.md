# Slot Car AR

Slot Car AR · Realidades Extendidas y Experiencias Inmersivas · UGM · 2026

## 1 · Qué es

- Experiencia de realidad aumentada de carreras slot car para fanáticos de estos juegos que no tienen espacio suficiente para armar sus pistas en casa y sientan una experiencia de aceleración y velocidad.

## 2 · Cómo se usa

- Enlace a la escena: https://grezarraumartin-create.github.io/ar-slot-car/
- Dispositivo pensado: Dispositivos Android/PC
- Al entrar: Debes presionar el botón del acelerador para iniciar la carrera, una vez hecho eso, su auto y el del rival empezaran a moverse por la pista

## 3 · Cómo está hecha

- Herramienta: A-Frame, publicado en GitHub Pages.
- Archivos que usé:

  - **activos/auto.glb**: modelo 3D. Origen: lo hice yo
  - **activos/pista.glb**: modelo 3D. Origen: lo hice yo

## 4 · Decisiones

- Qué decidí y por qué
  - La luz vino con el codigo generado, decidi no hacerle cambios ya que la prioridad principal de este prototipo era la jugabilidad y las mecanicas sobre el estilo visual
  - Los materiales de los objetos usados son simples ya que este prototipo no se enfoca en el aspecto visual, sino que en la jugabilidad
  - El audio del motor de los autos es un sintetizador usando GameAudio en donde la frecuencia y el pitch cambian segun la velocidad del auto y se apaga cuando sale de la pista
  - El jugador interactua con un boton para controlar la velocidad del vehiculo, esto se hiso para replicar la experiencia de los controles de los Slot Cars, que normalmente tenian solo un boton
- Qué cambió respecto de lo que propuse en la Solemne 1, y por qué.
  - La mecanica del turbo no se ha implementado aun ya que este prototipo busca presentar la jugabilidad de las carreras principal de la experiencia
  - Cambie la cantidad de vueltas de la pista de 4 a 15, ya que las carreras hubieran sido muy cortas con la velocidad que implemente en el codigo

## 5 · Testing

Video del recorrido: https://youtu.be/Pmt8wgBqABY

### Abrir el enlace en ventana privada
- Resultado: Funciona correctamente

### Dispositivo elegido
- Resultado: En vertical, la camara esta muy cerca y no se ve la pista completa. En horizontal, la pista desaparece y la interfaz cubre la pantalla
- Ajuste que hice: En vertical, voy a alejar la camara para que se vea la pista. En horizontal se esta revisando

### Interacciones, una por una
- Resultado:
  - El usuario revisa las descripciones en la interfaz
  - El usuario presiona el boton "acelerar" y la carrera comienza
  - El usuario llega a la curva final muy rapido y se sale de la pista
  - Con cada vuelta, el usuario aprende el momento exacto para frenar
- Ajuste que hice: Reduci el numero de vueltas a 15, ya que una vez el usuario se acostumbra a las curvas, la carrera se vuelve monotona

### Sonido con audífonos
- Resultado: Funciona correctamente

### Fluidez del recorrido
- Resultado: El usuario empieza la carrera y conforme avanza en ella, se va adaptando a la pista, cuando acelerar y cuando frenar

### Entrar como si fuera la primera vez
- Resultado: El usuario revisa el lugar antes de presionar el boton, donde empieza la carrera. Algunos usuarion presional el boton, y otros usan la barra espaciadora.

## 6 · Uso de IA

- Qué le pedí a la IA (herramienta y para qué).
  - Utilize Claude para crear la base del codigo, implementando las mecanicas, los controladores, el rival, el sintetizador y que ajustara el camino segun las indicaciones que puse en el modelo
- Qué hice yo y qué cambié de lo que me entregó.
  - Yo cree los modelos usados en el prototipo y ajuste los datos como la velocidad, la aceleracion, la friccion y el agarre del auto para que se sintieran como slot cars cuando presionas el boton y lo sueltas, y que pasa cuando vaz muy rapido entrando a una curva

## 7 · Pendientes para el examen

- Lo que falta, en orden de importancia.
  - Mecanica de nitro y la barra de energia
  - Implementacion de realidad aumentada (La pista tiene que aparecer en una superficie plana)
  - Como se siente en dispostivos moviles (Interaz de usuario y controles)
  - Ajuste de los modelos para que queden bajo el presupuesto propuesto y implementacion de los mapas UV para su texturizado
  - Ajuste del estilo de la interfaz de usuario