# Examen — Pensamiento computacional

## Información del proyecto:

  * Nombre del proyecto: Nunca es suficiente 
  * Autora: Denisse Delgado  

---

# Descripción objetiva

## ¿Qué es el proyecto?
  * Nunca es suficiente es una visualización interactiva desarrollada en p5.js que busca representar la presión estética y social ejercida sobre el cuerpo femenino. Mediante imágenes, textos, movimiento y transformaciones visuales, el sistema traduce una problemática de género en un comportamiento computacional interactivo.
  * El proyecto propone una experiencia donde la posición horizontal del mouse simboliza distintos niveles de presión social, generando cambios progresivos en el ambiente visual.
---

## ¿Qué se ve en pantalla?

El proyecto se compone de tres estados principales:

Pantalla 1: Inicio
  * Título del proyecto.
  * Breve descripción conceptual.
  * Botón para comenzar la experiencia.

Pantalla 2: Instrucciones
  * Explicación de la interacción.
  * Indicaciones para navegar dentro del sistema.
  * Botón para acceder a la visualización.

Pantalla 3: Interacción
  * Dos figuras femeninas.
  * Una nube compuesta por palabras asociadas a exigencias estéticas.
  * Partículas ambientales.
  * Fondo dinámico.
  * Textos reflexivos.
  * Elementos gráficos decorativos.

  * En la pantalla 3 aparecen dos figuras femeninas, una más grande y otra más pequeña y triste, conectadas mediante una flecha que representa una transformación progresiva. El/La usuari@ puede interactuar moviendo el mouse horizontalmente, lo que modifica el comportamiento visual de los elementos. También aparece una nube compuesta por palabras relacionadas con estándares de belleza y exigencias sociales, además de partículas y elementos gráficos ambientales.

---

## ¿Qué elementos visuales aparecen?

  * Dos imágenes PNG.
  * Textos reflexivos.
  * Array de palabras flotantes.
  * Sistema de partículas.
  * Círculos superpuestos.
  * Líneas y grillas decorativas.
  * Fondo dinámico.
  * Movimiento oscilatorio.
  * Animación continua.

---

# Descripción conceptual

## Idea central del proyecto y relación con el sistema diseñado

  * La idea central del proyecto es representar cómo la presión estética externa puede modificar la percepción corporal y emocional de una persona, lo cúal está dirigido principalmente a mujeres.

  * El sistema utiliza la interacción del mouse como metáfora de la presión social: mientras más avanza el usuario hacia la derecha, mayor es la intensidad visual de las exigencias sociales, por eso cambia de color y distintas figuras se agrandan.

  * La transformación de las figuras, el aumento del ruido visual y el cambio de ambiente simbolizan cómo estas expectativas afectan la autoimagen.

---

## Regla de oro del sistema:

  * “A mayor presión social, mayor distorsión de la percepción corporal.”

Esta regla se traduce visualmente mediante:
- Reducción de una figura femenina
- Crecimiento de la segunda figura
- Intensificación del fondo
- Mayor presencia de palabras y ruido visual

---

## Relación con la problemática de género

  * Históricamente, las mujeres han sido sometidas a estándares estéticos rígidos promovidos por medios de comunicación, redes sociales e industrias culturales. 

  * Las palabras flotantes representan discursos repetitivos asociados a la apariencia física, juventud y perfección.

  * El sistema del proyecto busca evidenciar cómo estas exigencias externas pueden alterar la percepción de la identidad y generar tensión emocional.

---

# Input / Output y sistema

## INPUT

- Los datos de entrada del sistema son:
    * Posición horizontal del mouse (mouseX).
    * Click sobre botones (mousePressed).
    * Presión de la tecla R (keyPressed).
    * Tiempo del sistema (frameCount).
    * Variables internas de p5.js (width y height).

---

## Procesamiento

- El sistema procesa los datos utilizando:
    * Condicionales (`if / else`)
    * Mapeo de valores (`map()`)
    * Funciones matemáticas (`sin()`)
    * Escalado (`scale()`)
    * Rotación (`rotate()`)
    * Traducción (`translate()`)
    * Repetición (For()`)

- El valor de `mouseX` controla:
    * Escala de las imágenes
    * Intensidad del fondo
    * Tamaño del texto
    * Velocidad de rotación
    * Sensación de presión visual

---

## OUTPUT

- La respuesta visual del sistema incluye:
    * Cambio de color del fondo.
    * Modificación del tamaño de las figuras.
    * Movimiento continuo.
    * Rotación de la nube.
    * Aparición de partículas.
    * Variación del tamaño del texto.
    * Cambio de ambiente visual.

---

# Pensamiento computacional

## Reglas del sistema

Descomposición
- La problemática fue dividida en módulos independientes:
    * Pantalla de inicio.
    * Pantalla de instrucciones.
    * Pantalla interactiva.
    * Sistema de partículas.
    * Sistema de botones.
    * Transformación corporal.
    * Sistema de textos.

Reconocimiento de patrones
- Se utilizan estructuras repetitivas mediante ciclos for() para generar:
    * Partículas.
    * Nubes visuales.
    * Palabras.
    * Grillas decorativas.

Abstracción
- El proyecto abstrae la presión social mediante el movimiento horizontal del mouse.
    * Más mouse hacia la derecha = Mayor presión social
    * Esta presión modifica visualmente todo el sistema.

Algoritmos
- El sistema sigue la siguiente secuencia:
    * Cargar imágenes.
    * Crear canvas responsivo.
    * Generar partículas.
    * Mostrar pantalla inicial.
    * Esperar interacción del usuario.
    * Mostrar instrucciones.
    * Esperar segundo click.
    * Iniciar visualización.
    * Interpretar posición del mouse.
    * Actualizar variables visuales.
    * Dibujar todos los elementos.
    * Reiniciar mediante tecla R.

### Input
El usuario interactúa mediante el movimiento del mouse.

### Procesos
El sistema interpreta la posición del mouse y transforma variables visuales usando:
- Condicionales
- Mapeos numéricos
- Funciones 
- Animación en tiempo real

### Output
El sistema genera cambios visuales que representan distintos niveles de presión emocional y estética.

---

## Explicación de la interactividad
Las principales relaciones de interacción son las siguientes:

  * Movimiento del mouse → Nivel de presión: La posición del cursor se transforma mediante la función map() en un valor numérico entre 0 y 1, almacenado en la variable presion.
  * Presión → Cambio del fondo: Dependiendo de la posición del mouse, el fondo cambia gradualmente desde tonos oscuros y calmados hacia tonos rojizos más intensos, simbolizando distintos niveles de tensión emocional.
  * Presión → Transformación corporal: La figura femenina ubicada a la izquierda disminuye progresivamente de tamaño, mientras que la figura de la derecha aumenta su escala, representando la distorsión de la autoimagen provocada por la presión social.
  * Presión → Intensidad de los mensajes externos: Las palabras asociadas a exigencias estéticas ("Sé perfecta", "Más delgada", etc.) incrementan su tamaño conforme aumenta la presión, volviéndose más visibles y dominantes dentro del espacio visual.
  * Movimiento continuo → Dinamismo visual: Tanto las partículas ambientales como la rotación de la nube de pensamientos generan una sensación constante de movimiento, reforzando la idea de un entorno psicológico activo y persistente.
  * Interacción mediante botones: El usuario avanza entre las distintas pantallas del proyecto (inicio, instrucciones e interacción principal) haciendo clic sobre los botones "COMENZAR" y "EXPLORAR".
  * Interacción mediante teclado: La tecla R permite reiniciar completamente la experiencia, devolviendo todas las variables y elementos visuales a su estado inicial.

La interacción principal ocurre en la pantalla 3 con el movimiento horizontal del mouse:

- Hacia la izquierda:
     * Ambiente más calmado
     * Menor presión visual
     * Figura principal más grande

- Hacia la derecha:
     * Fondo más intenso
     * Más ruido visual
     * Figura principal más pequeña
     * Mayor protagonismo de la figura secundaria

- El click del mouse también modifica aleatoriamente el color del fondo.

---

# Referentes

## Referentes visuales

### Barbara Kruger:
- Uso de texto como crítica social y cuestionamiento de los estándares impuestos sobre el cuerpo femenino.

### Jenny Holzer:
- Uso de frases y mensajes como elemento visual y político.

---

## Referentes conceptuales

### Presión estética y género
- El proyecto toma como referencia las problemáticas relacionadas con:
    * Estándares irreales de belleza
    * Autoimagen corporal
    * Influencia de redes sociales
    * Exigencias culturales hacia las mujeres

---

# Diagrama de flujo
<img width="2268" height="1890" alt="Diagrama de flujo" src="https://github.com/user-attachments/assets/b7235afd-3201-4a32-9786-9dc6999b9c5b" />

# Código:
- Link al Sketch en p5.js (con permiso de edición)
(https://editor.p5js.org/denisse.delgado2/sketches/yUF1ghR7g)

```
// ------------------------------------------------------
// VARIABLES

// Imágenes principales del proyecto
let mujerGrande; // Imagen “mujer grande” (Representa estado inicial o más fuerte)
// Funciona como punto de partida de la transformación visual causada por la presión social.
let mujerPequena; // Imagen “mujer pequeña” (Representa el efecto de la presión estética constante)

// Estados de navegación de la experiencia interactiva
// 0 = Pantalla de inicio
// 1 = Pantalla de instrucciones
// 2 = Pantalla principal interactiva
let estado = 0; // Variable que controla qué pantalla se muestra al usuario.

// Variables para controlar la posición y tamaño del botón
let botonX; // Posición horizontal del botón
let botonY; // Posición vertical del botón
let botonAncho = 220; // Ancho del botón
let botonAlto = 60; // Alto del botón

// Palabras dentro de la nube
let palabras = [
  // Lista de frases o palabras que representan discursos sociales internalizados, exigencias estéticas repetitivas que afectan la autoimagen, generando una “voz externa” constante dentro del espacio visual.
  "Sé perfecta",
  "Más delgada",
  "Sin arrugas",
  "Más delicada",
  "Piel perfecta",
  "Cintura pequeña",
  "Simétrica",
  "Más bonita",
  "Más flaca",
  "Nariz perfecta",
  "Siempre joven",
  "Maquillada",
  "Cuerpo perfecto",
];

// Partículas ambientales que se mueven por el canvas
let particulas = []; // Contiene partículas que simulan “ruido visual” o ambiente nostálgico

// Variables propias
let presion = 0; // Nivel de presión (Derivado del mouse)
let colorFondo; // Color del fondo dinámico según interacción con el mouse
let rotacionNube = 0; // Controla la rotación progresiva de la nube de palabras.

// ------------------------------------------------------
//CLASE

// Clase que define el comportamiento de cada partícula
class Particula {
  constructor() {
    // Se ejecuta cada vez que se crea una nueva partícula
    this.x = random(width); // Posición horizontal aleatoria dentro del canvas
    this.y = random(height); // Posición vertical aleatoria dentro del canvas
    this.size = random(1, 4); // Tamaño aleatorio de la partícula
    this.speed = random(0.2, 1); // Velocidad de desplazamiento vertical
    this.alpha = random(20, 120); // Transparencia aleatoria para generar profundidad visual
  }

  mostrar() {
    // Método encargado de dibujar la partícula
    noStroke(); // Elimina el borde de la partícula
    fill(255, this.alpha); // Define el color blanco con transparencia variable
    ellipse(this.x, this.y, this.size); // Dibuja la partícula en sus coordenadas
  }

  mover() {
    // Método encargado del movimiento de la partícula
    this.y += this.speed; // Desplaza la partícula verticalmente

    if (this.y > height) {
      // Si la partícula sale por la parte inferior del canvas
      this.y = 0; // Vuelve a aparecer en la parte superior
      this.x = random(width); // Se le asigna una nueva posición horizontal aleatoria
    }
  }
}

// ------------------------------------------------------
// CARGA DE IMÁGENES

function preload() {
  // Carga de imágenes antes de iniciar el programa
  mujerGrande = loadImage("k1.png"); // Carga la imagen correspondiente al estado corporal inicial
  mujerPequena = loadImage("k2.png"); // Carga la imagen correspondiente al estado corporal desanimado
}

// ------------------------------------------------------
// CONFIGURACIÓN INICIAL

function setup() {
  createCanvas(windowWidth, windowHeight); // Crea un canvas adaptable al tamaño de la ventana

  // Centra imágenes y texto para facilitar composición visual
  imageMode(CENTER);
  textAlign(CENTER, CENTER);

  // Cursor visible
  colorFondo = color(10, 10, 18); // Define el color inicial del fondo

  botonX = width / 2 - botonAncho / 2; // Calcula la posición horizontal del botón para mantenerlo centrado
  botonY = height * 0.75; // Define la posición vertical del botón

  for (let i = 0; i < 100; i++) {
    // Crea 100 partículas y las almacena
    particulas.push(new Particula());
  }
}

// ------------------------------------------------------
// DRAW

function draw() {
  if (estado === 0) {
    // Si el estado es 0, muestra la pantalla de inicio
    pantallaInicio();
  } else if (estado === 1) {
    // Si el estado es 1, muestra la pantalla de instrucciones
    pantallaInstrucciones();
  } else if (estado === 2) {
    // Si el estado es 2, ejecuta la experiencia interactiva
    actualizarPresion(); // Actualiza el nivel de presión según la posición del mouse

    background(colorFondo); // Dibuja el color de fondo correspondiente

    // Dibujo de capas visuales
    dibujarFondo(); // Grilla + ambiente
    dibujarParticulas(); // Partículas flotantes
    dibujarBurbuja(); // Nube/presión social
    dibujarTransformacion(); // Relación visual entre dos estados corporales
    dibujarTexto(); // Mensajes narrativos

    rotacionNube += map(mouseX, 0, width, 0.0005, 0.03); // Rotación progresiva de la nube de presión
  }
}

// ------------------------------------------------------
// PANTALLA INICIO

function pantallaInicio() {
  // Dibuja la pantalla inicial del proyecto
  background(20, 10, 25); // Define el color de fondo
  dibujarParticulas(); // Dibuja las partículas ambientales
  textAlign(CENTER, CENTER); // Centra el texto

  // Configuraciones del título
  fill(255, 120, 140);
  textSize(constrain(width * 0.05, 28, 50)); // Ajusta el tamaño del título de forma responsiva
  text("NUNCA ES SUFICIENTE", width / 2, height * 0.3); // Dibuja el título principal

  // Configuraciones del texto
  fill(255);
  textSize(constrain(width * 0.03, 14, 22)); // Ajusta el tamaño del texto de manera responsiva
  text(
    "Una visualización interactiva acerca de la presión\nsocial ejercida sobre el cuerpo femenino.",
    width / 2,
    height * 0.45
  );

  push();
  textStyle(BOLD); // Aplica estilo negrita al texto del botón
  dibujarBoton("COMENZAR"); // Dibuja el botón de inicio
  pop();
}

// ------------------------------------------------------
// PANTALLA INSTRUCCIONES

function pantallaInstrucciones() {
  // Dibuja la pantalla de instrucciones
  background(20, 10, 25);
  dibujarParticulas();
  textAlign(CENTER, CENTER);

  // Configuraciones del título
  fill(255, 120, 140);
  textSize(constrain(width * 0.05, 24, 40)); // Ajusta el tamaño del título de forma responsiva
  text("INSTRUCCIONES", width / 2, height * 0.3);

  // Configuraciones del texto
  push();
  textAlign(CENTER, TOP); // Alinea el texto hacia la izquierda y el top es la parte superior
  fill(255);
  textSize(constrain(width * 0.027, 14, 22)); // Ajusta el tamaño del texto de manera responsiva
  text(
    "∘ Mueva el mouse hacia la derecha\npara aumentar la presión.\n\n∘ Mueva el mouse hacia la izquierda\npara disminuir la presión.\n\n∘ Presione la tecla R para reiniciar.",
    width / 2,
    height * 0.35
  );
  pop();

  push();
  textStyle(BOLD);
  dibujarBoton("EXPLORAR");
  pop();
}

// ------------------------------------------------------
// BOTÓN

function dibujarBoton(textoBoton) {
  // Dibuja un botón interactivo
  if (
    // Comprueba si el cursor se encuentra sobre el botón
    mouseX > botonX &&
    mouseX < botonX + botonAncho &&
    mouseY > botonY &&
    mouseY < botonY + botonAlto
  ) {
    fill(255, 170, 190); // Cambia el color al pasar el cursor
  } else {
    fill(255, 120, 140); // Mantiene el color original
  }

  noStroke(); // Elimina el borde del botón
  rect(botonX, botonY, botonAncho, botonAlto, 20); // Dibuja el rectángulo del botón

  // Configura el texto del botón
  fill(255);
  textSize(22);

  text(textoBoton, width / 2, botonY + botonAlto / 2); // Dibuja el texto centrado dentro del botón
}

// ------------------------------------------------------
// CLICK BOTONES

function mousePressed() {
  // Se ejecuta automáticamente cuando el usuario hace clic
  if (
    // Comprueba si el clic ocurrió dentro del botón
    mouseX > botonX &&
    mouseX < botonX + botonAncho &&
    mouseY > botonY &&
    mouseY < botonY + botonAlto
  ) {
    if (estado === 0) {
      // Si se encuentra en la pantalla inicial
      estado = 1; // Cambia a la pantalla de instrucciones
    } else if (estado === 1) {
      // Si se encuentra en la pantalla de instrucciones
      estado = 2; // Cambia a la experiencia interactiva
    }
  }
}

// ------------------------------------------------------
// TECLADO

function keyPressed() {
  // Detecta cuando el usuario presiona una tecla
  if (key === "r" || key === "R") {
    // Si la tecla presionada es "r" o "R"
    reiniciar(); // Se ejecuta la función que reinicia la experiencia
  }
}

// ------------------------------------------------------
// RESET

function reiniciar() {
  // Reinicia todos los elementos interactivos a su estado inicial
  estado = 0; // Vuelve a la pantalla de inicio
  presion = 0; // Reinicia el nivel de presión
  rotacionNube = 0; // Reinicia la rotación de la nube de palabras
  colorFondo = color(10, 10, 18); // Restablece el color inicial del fondo
  particulas = []; // Vacía el grupo de partículas

  for (let i = 0; i < 100; i++) {
    // Crea nuevamente las 100 partículas iniciales
    particulas.push(new Particula());
  }
}

// ------------------------------------------------------
// PRESIÓN

function actualizarPresion() {
  // // Actualiza el nivel de presión social y modifica el fondo

  // Convierte posición del mouse en un valor entre 0 y 1
  presion = map(mouseX, 0, width, 0, 1);
  // Cambia el color del fondo según la posición del mouse
  // Esto representa distintos niveles de tensión emocional

  // If/Else
  if (mouseX < width / 3) {
    colorFondo = color(10, 10, 18); // Más oscuro / Calmado
  } else if (mouseX < width / 1.5) {
    colorFondo = color(35, 10, 20); // Intermedio / Tensión
  } else {
    colorFondo = color(80, 0, 20); // Más intenso / Presión social alta
  }
}

// ------------------------------------------------------
// TRANSFORMACIÓN

// Transformación del tamaño de las imágenes
function dibujarTransformacion() {
  // Escala de la imagen grande (Se reduce con la presión social)
  let escalaGrande = map(mouseX, 0, width, 1, 0.25);
  // Escala de la imagen pequeña (Aumenta con la presión social)
  let escalaTriste = map(mouseX, 0, width, 0.15, 1);
  // Movimiento suave tipo “Respiración”
  let movimientoY = sin(frameCount * 0.03) * 8;

  // Mujer grande(Izquierda)
  push();
  translate(width * 0.3, height * 0.68 + movimientoY); // Permite trasladar la figura a otra coordenada
  rotate(sin(frameCount * 0.02) * 0.03); // Permite rotar la figura de forma orgánica y mas suave
  scale(escalaGrande * 1.5); // Permite cambiar el tamaño de la imagen
  tint(255, 230); // Permite aplicar transparencia o color a una iamgen
  image(mujerGrande, 0, 0, 160, 350); // Permite "llamar" a la imagen inscrita antes del setup
  pop();

  // Flecha simbólica de transformación
  fill(255, 120, 140); // Se utiliza para cambiar el color del relleno de la figura
  textSize(50); // Cambia el tamaño del texto
  text("→", width / 1.9, height * 0.63); // Inserta texto en ciertas coordenadas

  // Mujer triste(Derecha)
  push();
  translate(width * 0.7, height * 0.58 - movimientoY);
  scale(escalaTriste * 1.7);
  rotate(sin(frameCount * 0.04) * 0.02);
  image(mujerPequena, 0, 0, 220, 300);
  pop();
}

// ------------------------------------------------------
// BURBUJA

// Nube / Burbuja que se produce al sobrepensar debido a todo el estrés externo que las espectativas producen
function dibujarBurbuja() {
  // Nube de círculos aleatorios que representan ruido mental/social
  push();
  translate(width * 0.68, height * 0.25);
  rotate(rotacionNube);
  noFill();

  for (let i = 0; i < 120; i++) {
    // Repite el proceso 120 veces para generar la nube de círculos
    stroke(255, 35);
    ellipse(random(-70, 70), random(-70, 70), random(50, 70));
  }
  pop();

  textFont("verdana"); // Permite cambiar la tipografía de los textos

  // Palabras que se mueven(Representan las expectativas que comúnmente recaen sobre las mujeres)
  for (let i = 0; i < palabras.length; i++) {
    fill(255, 160, 190);

    // Random()
    let tamaño = map(mouseX, 0, width, 10, 22); // Tamaño de texto depende del mouse (Más presión = Más grande, visible, asfixiante)
    textSize(tamaño);

    // Movimiento ondulatorio de las palabras
    let x = width * 0.75 + sin(frameCount * 0.01 + i) * 100;
    let y = height * 0.15 + i * 12;

    text(palabras[i], x, y);
  }
}

// ------------------------------------------------------
// PARTÍCULAS

function dibujarParticulas() {
  // Dibuja y actualiza todas las partículas del entorno
  for (let p of particulas) {
    // Recorre cada partícula almacenada en el array
    p.mostrar(); // Dibuja visualmente la partícula
    p.mover(); // Actualiza su posición para generar movimiento
  }
}

// ------------------------------------------------------
// FONDO

function dibujarFondo() {
  // Encargada de construir el ambiente visual
  for (let i = 0; i < width; i += 40) {
    // Grilla sútil que genera estructura visual
    stroke(255, 10); // Define el color de las líneas con baja opacidad
    line(i, 0, i, height); // Dibuja líneas verticales
    line(0, i, width, i); // Dibuja líneas horizontales
  }

  // Forma decorativa transparente tipo base
  noStroke();
  fill(255, 100, 150, 18);
  ellipse(width / 2, height - 20, 500, 30);

  // Círculos decorativos adicionales (Sensación de presión)
  noFill();
  stroke(255, 60);

  // Grupo de círculos ubicado a la izquierda
  ellipse(width * 0.42, height * 0.24, width * 0.03);
  ellipse(width * 0.37, height * 0.28, width * 0.025);
  ellipse(width * 0.34, height * 0.33, width * 0.02);
  // Grupo de círculos ubicado a la derecha
  ellipse(width * 0.75, height * 0.47, width * 0.03);
  ellipse(width * 0.77, height * 0.55, width * 0.025);
  ellipse(width * 0.75, height * 0.6, width * 0.02);
}

// ------------------------------------------------------
// TEXTOS

function dibujarTexto() {
  // Dibuja los mensajes reflexivos y elementos decorativos
  noStroke();
  textAlign(LEFT); // Texto alineado a la izquierda (Mensaje interno)
  textSize(18);
  fill(255, 120, 140);

  text(
    "La presión no cambia quién eres,\nsolo distorsiona cómo te ves.",
    40,
    60
  );

  textAlign(RIGHT); // Texto alineado a la derecha (Mensaje de reflexión)
  text(
    "Apaga el ruido exterior,\nsolo escúchate a ti.",
    width - 40,
    height - 50
  );

  // Líneas decorativas (Encuadre visual)
  stroke(255, 40);
  line(20, 40, 20, 90);
  line(width - 20, height - 20, width - 20, height - 80);
}

// ------------------------------------------------------
// LIENZO RESPONSIVO

function windowResized() {
  // Ajusta el canvas y algunos elementos cuando cambia el tamaño de la ventana
  resizeCanvas(windowWidth, windowHeight); // Redimensiona automáticamente el canvas según el tamaño de la ventana

  botonX = width / 2 - botonAncho / 2; // Recalcula la posición horizontal del botón para mantenerlo centrado
  botonY = height * 0.75; // Recalcula la posición vertical del botón
}
```

