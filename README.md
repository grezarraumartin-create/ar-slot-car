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

Video del recorrido: https://...

### Abrir el enlace en ventana privada
- Resultado: ...
- Ajuste que hice: ...

### Dispositivo elegido
- Resultado: ...
- Ajuste que hice: ...

### Interacciones, una por una
- Resultado: ...
- Ajuste que hice: ...

### Sonido con audífonos
- Resultado: ...
- Ajuste que hice: ...

### Fluidez del recorrido
- Resultado: ...
- Ajuste que hice: ...

### Entrar como si fuera la primera vez
- Resultado: ...
- Ajuste que hice: ...

## 6 · Uso de IA

- Qué le pedí a la IA (herramienta y para qué).
  - Utilize Claude para crear la base del codigo, implementando las mecanicas, los controladores, el rival y que ajustara el camino segun las indicaciones que puse en el modelo
- Qué hice yo y qué cambié de lo que me entregó.
  - Yo cree los modelos usados en el prototipo y ajuste los datos como la velocidad, la aceleracion y la friccion para que se sintieran como slot cars cuando presionas el boton de aceleracion

## 7 · Pendientes para el examen

- Lo que falta, en orden de importancia.
  - Mecanica de nitro y la barra de energia
  - Implementacion de realidad aumentada (La pista tiene que aparecer en una superficie plana)
  - Como se siente en dispostivos moviles (Interaz de usuario y controles)
  - Ajuste de los modelos para que queden bajo el presupuesto propuesto y implementacion de los mapas UV para su texturizado
  - Ajuste del estilo de la interfaz de usuario