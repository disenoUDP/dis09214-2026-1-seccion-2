# EXAMEN - 26/06 

**INFORMACIÓN DEL PROYECTO**   
***Nombre del proyecto:*** Ecos de Aflicción   
***Autores:***  Nissa Contreras/Sofía Díaz  
***Problemática de género elegida:***   Violencia hacía la mujer dentro de una relación 



***¿Qué es el proyecto?:***   
Es una pieza gráfica interactiva y experimental que busca representar el ciclo de una relación marcada por la manipulación emocional y la violencia psicológica hacia la mujer. A través de tres escenas consecutivas, el usuario recorre distintas etapas de una relación abusiva mediante la interacción con botones y el teclado, convirtiéndose en un participante activo de la experiencia.
La obra evidencia, a través de la interacción, el ciclo de violencia y los patrones de conducta que experimentan muchas mujeres víctimas de abuso psicológico dentro de una relación de pareja. Mediante recursos visuales, animaciones y cambios en la composición, se representan las distintas fases de este proceso, mostrando cómo estas dinámicas se intensifican, se repiten y evolucionan con el tiempo. De este modo, la experiencia busca transmitir emociones como el miedo, la dependencia emocional, la inseguridad, la confusión y la tensión constante, reflejando un contexto de vulnerabilidad en el que la víctima siente que no existe una salida.


***¿Qué se ve en pantalla?:***   
En pantalla se observan ilustraciones de una pareja sobre fondos predominantemente rojos y negros, colores que transmiten tensión, peligro y angustia. Durante la experiencia aparecen frases manipuladoras repetidas, lágrimas que caen constantemente, círculos pulsantes y otros elementos gráficos que cambian cuando el usuario presiona una tecla. Todo el recorrido está acompañado por música ambiental que refuerza el tono emocional de la experiencia.

***¿Qué elementos visuales aparecen?***   
- Ilustraciones de una pareja en distintas escenas.
- Fondos rojos y negros.
- Patrones tipográficos con frases manipuladoras.
- Círculos pulsantes y círculos que aparecen y desaparecen.
- Sistema de partículas que simula lágrimas cayendo.
- Botones para avanzar y reiniciar la experiencia.
- Imágenes que cambian cuando el usuario interactúa.

 

COLORES: 

1. ROJO: en las primeras escenas es usado para representar el romanticismo al ir conociéndose y ver todo bonito, de forma idealizada/ pero con el paso del tiempo, conociendo realmente a la persona y de lo que es capaz se usa para representar un estado de alerta y dolor tanto físico como emocional.
2. BLANCO Y NEGRO: colores secundarios que representan tensión y  neutralidad, un escenario abierto a la imaginación 

TEXTO:  
INSTRUCCIONES: (BOTONES)
-	Continuar (2)
- Haz clic aquí para volver al inicio

FRASES:
- “ Lo prometo, cambiaré( indefinidamente)
- “Nadie te va a querer como yo”(indefinidamente)

ILUSTRACIONES:    

<img width="736" height="736" alt="Estado0" src="https://github.com/user-attachments/assets/a9726e6c-7e77-4663-9030-d6413e0faf2f" />
<img width="480" height="480" alt="Estado2" src="https://github.com/user-attachments/assets/21ccf2c0-d5d2-4abb-898f-360fa5eef196" />
<img width="736" height="506" alt="Estado1" src="https://github.com/user-attachments/assets/d7affd05-14d6-49c6-b2b7-ab97efbe6351" />
<img width="650" height="570" alt="segundoE0" src="https://github.com/user-attachments/assets/94e9fbeb-d4c5-49f0-b70e-f7c81f7ff863" />
<img width="1020" height="1020" alt="segundoE1" src="https://github.com/user-attachments/assets/cb9acf5b-da22-48d1-84a2-3075356adfbe" />
<img width="338" height="338" alt="segundoE2" src="https://github.com/user-attachments/assets/52371ff6-4d02-4475-a526-fb16f3d278fa" />   

SONIDO: (MELODIA): 
[nostalgia.mp3](https://github.com/user-attachments/files/29368148/nostalgia.mp3)   



 
   
**DESCRIPCIÓN CONCEPTUAL**  

Aflicción es el concepto central de nuestro proyecto. A través de este, buscamos visibilizar la violencia psicológica dentro de una relación de pareja, mostrando cómo las palabras y las conductas manipuladoras afectan emocionalmente a la víctima. El sistema está diseñado para que cada interacción revele una nueva dimensión del conflicto, utilizando imágenes, animaciones y frases que representan distintas fases de la manipulación emocional.
La experiencia no pretende mostrar violencia física, sino evidenciar aquellas formas de control que muchas veces pasan desapercibidas, como la culpa, la dependencia emocional, las falsas promesas de cambio y el aislamiento.

***¿Cuál es la regla de oro de tu sistema?***   

Mientras mayor es la interacción del usuario, mayor es la intensidad emocional y visual de la experiencia.
Cada vez que el usuario presiona una tecla, el sistema revela una versión más perturbadora de la escena, aumentando la carga emocional mediante cambios de imágenes, colores y elementos gráficos.


***¿Cómo se relaciona esta lógica con la problemática de género elegida?***    

Así como ocurre en muchas situaciones de la vida real, los episodios de violencia suelen comenzar de manera silenciosa y casi imperceptible, manifestándose a través de acciones sutiles o minimizadas. Sin embargo, a medida que estos actos aumentan en intensidad y frecuencia, dejan de ser visibles únicamente para la mujer violentada y comienzan también a evidenciarse para quienes la rodean. La interacción representa el proceso que viven muchas víctimas de violencia psicológica: detrás de una relación que inicialmente parece normal comienzan a aparecer conductas de control, manipulación y chantaje emocional. Las frases repetidas, como “nadie te va a querer como yo”, cambiaré, lo prometo", representan un discurso frecuente en relaciones abusivas, mientras que las lágrimas, la oscuridad y los cambios visuales simbolizan el deterioro emocional provocado por este tipo de violencia.

**INPUT/OUTPUT**    
INPUT: 
El sistema recibe: 
* Presionar el botón Continuar.
* Presionar el botón Volver al inicio.
* Presionar cualquier tecla del teclado.
* El paso del tiempo (frames), que permite mantener las animaciones.
¿Cómo se procesan y transforman?
El programa utiliza una variable llamada estado para controlar el recorrido entre las tres escenas. Dependiendo del estado y de si el usuario mantiene una tecla presionada, el sistema activa distintas funciones que modifican completamente la apariencia visual.
Además, se generan automáticamente:
* lágrimas mediante un sistema de partículas;
* círculos con posiciones, tamaños y velocidades aleatorias;
* patrones de texto repetitivo;
* animaciones que cambian continuamente con el tiempo.
  
OUTPUT:
Como respuesta, el sistema produce:
* cambios entre las tres escenas;
* aparición de nuevas imágenes;
* patrones tipográficos dinámicos;
* animaciones de lágrimas y círculos;
* cambios de color y composición;
* reproducción continua de sonido ambiental.


**PENSAMIENTO COMPUTACIONAL**   
El proyecto está construido mediante un sistema de estados que organiza la narrativa interactiva. Cada estado contiene reglas específicas que determinan qué imágenes, animaciones e interacciones se muestran al usuario.
Reglas: 
* El botón Continuar cambia el estado de la experiencia.
* El botón Volver al inicio reinicia todo el recorrido.
* Presionar una tecla activa una segunda versión de cada escena.
* Los círculos utilizan funciones matemáticas para modificar su tamaño continuamente.
* Las lágrimas funcionan como un sistema de partículas que cae y se reinicia automáticamente al salir de la pantalla.
* El sonido permanece activo durante toda la experiencia para mantener la atmósfera emocional.
Explicación del sistema: 
La interactividad está basada en acciones simples del usuario, pero con un fuerte impacto narrativo. Cada decisión —avanzar de escena o presionar una tecla— modifica el ambiente visual y revela nuevos elementos relacionados con la violencia psicológica. De este modo, el usuario no solo observa la historia, sino que participa activamente en el descubrimiento de las distintas etapas del ciclo de manipulación emocional, reforzando el mensaje del proyecto mediante la interacción.





**REFERENTES**   
https://cl.pinterest.com/pin/738168195224596645/ 
https://cl.pinterest.com/pin/741123682471567439/ 
https://cl.pinterest.com/pin/113715959329156043/ 
https://cl.pinterest.com/pin/738168195224586938/ 
https://cl.pinterest.com/pin/738168195224560407/ 
https://cl.pinterest.com/pin/763078730641438138/ 
https://cl.pinterest.com/pin/738168195224596212/ 
https://cl.pinterest.com/pin/928445279406415338/ 
https://cl.pinterest.com/pin/11610911542005364/ 



**DIAGRAMA DE FLUJO**  
<img width="1548" height="2583" alt="DIAGRAMA DE FLUJO EXAMEN" src="https://github.com/user-attachments/assets/aed93cfb-7944-467a-b6c4-cac50300f4d4" />    



**LINK AL SKETCH EN P5.JS**  
:[p5.js](https://editor.p5js.org/sofiaaadiaz/sketches/17zCag412) 



**CÓDIGO DE P5.JS**

```
let estado = 0; // Variable que controla en qué pantalla se encuentra el programa. 0 = Inicio, 1 = Experiencia, 2 = Final
let botonAvanzar; // Botones para avanzar y reiniciar la experiencia
let botonInicio; // Botones para avanzar y reiniciar la experiencia

let fondoEstado0; // Variables donde se almacenan las imágenes de fondo del estado 0
let fondoEstado1; // Variables donde se almacenan las imágenes de fondo del estado 1
let fondoEstado2; // Variables donde se almacenan las imágenes de fondo del estado 2

let segundoE0; // Imágenes que aparecen al presionar una tecla en cada estado
let segundoE1; // Imágenes que aparecen al presionar una tecla en cada estado
let segundoE2; // Imágenes que aparecen al presionar una tecla en cada estado

let miSonido; // Variable que almacena el sonido de fondo

let circulosConfusion = []; // Array que guarda todos los círculos de confusión

let Diametro = [0, 20, 60, 110, 160, 210, 260, 310, 360, 410]; // Array que contiene los diferentes diámetros del círculo pulsante
let index = 0; // Índice que recorre el array Diametro

let lagrimas = []; // Array que almacena todas las lágrimas del sistema de partículas

let tamanoCirculo; // Variables utilizadas para crear un círculo aleatorio en el estado 1
let bordeCirculo; // Variables utilizadas para crear un círculo aleatorio en el estado 1

class CirculoConfusion {
  // Clase que genera círculos que aparecen y desaparecen
  constructor() {
    // Al crear cada círculo se inicializan sus propiedades
    this.reiniciar();
  }

  reiniciar() {
    // Asigna nuevas propiedades aleatorias al círculo para que vuelva a aparecer
    this.x = random(width); // Posición aleatoria dentro del canvas
    this.y = random(height); // Posición aleatoria dentro del canvas

    this.tamanoBase = random(80, 250); // Tamaño máximo del círculo
    this.velocidad = random(0.08, 0.015); // // Asigna una velocidad aleatoria para el efecto de pulsación del círculo
    this.fase = random(TWO_PI); // Desfase para que todos los círculos no respiren al mismo tiempo
    this.alpha = random(20, 80); // Transparencia aleatoria
  }

  mostrar() {
    // Dibuja un círculo y anima su efecto de pulsación
    let escala = map(sin(frameCount * this.velocidad + this.fase), -1, 1, 0, 1); // Convierte el movimiento en un valor entre 0 y 1

    let tam = this.tamanoBase * escala; // Calcula el tamaño actual

    noStroke(); // Elimina el borde de la figura
    fill(176, 21, 21, this.alpha); // Asigna el color con el que se rellenará la siguiente figura que se dibuje.
    ellipse(this.x, this.y, tam); // Cambia el tamaño continuamente, en una posición específica de la pantalla

    if (escala < 0.02) {
      // Comprueba si el círculo ya es casi invisible
      this.reiniciar(); // Reinicia las propiedades del círculo para que vuelva a aparecer en otra posición con características diferentes
    }
  }
}

class Lagrima {
  // Class que genera lágrimas negras cayendo.
  constructor() {
    this.x = random(width); // Posición inicial aleatoria
    this.y = random(-height, 0); // Posición inicial aleatoria
    this.velocidad = random(2, 5); // Asigna la velocidad de caída
    this.tamano = random(8, 20); // Asigna un tamaño aleatorio
  }

  caer() {
    // Actualiza la posición de la lágrima y la reinicia cuando sale de la pantalla
    this.y += this.velocidad; // Hace descender la lágrima

    if (this.y > height + this.tamano * 3) {
      // Cuando sale de la pantalla, vuelve a aparecer encima
      this.y = random(-200, 0); // Coloca la lágrima nuevamente por encima del canvas
      this.x = random(width); // Asigna una nueva posición horizontal aleatoria
      this.velocidad = random(2, 5); // Genera una nueva velocidad de caída
      this.tamano = random(8, 20); // Genera un nuevo tamaño para la lágrima
    }
  }

  mostrar() {
    // Dibuja una lágrima utilizando círculo y triángulo
    push(); // Guarda la configuración actual
    translate(this.x, this.y); // Mueve el sistema de coordenadas

    noStroke(); // Elimina el borde de las figuras
    fill(0); // Asigna el color negro a las figuras

    // parte redonda
    circle(0, this.tamano * 0.25, this.tamano); // Dibuja la parte redonda de la lágrima

    // punta
    triangle(
      -this.tamano * 0.5, // Asigna la posición izquierda de la base del triángulo
      this.tamano * 0.2, // Asigna la altura de la base del triángulo
      this.tamano * 0.5, // Asigna la posición derecha de la base del triángulo
      this.tamano * 0.2, // Asigna la misma altura de la base
      0,
      -this.tamano * 1.6 // Hace que la punta se alargue hacia arriba, dándole la forma característica de lágrima
    );
    pop(); // Restaura la configuración
  }
}

function preload() {
  // Se ejecuta antes del setup. Aquí se cargan todos los recursos del proyecto

  /// Carga las imágenes utilizadas en los tres estados del programa
  fondoEstado0 = loadImage("IMÁGENES/Estado0.png");
  fondoEstado1 = loadImage("IMÁGENES/Estado1.png");
  fondoEstado2 = loadImage("IMÁGENES/Estado2.png");

  segundoE0 = loadImage("IMÁGENES/segundoE0.png");
  segundoE1 = loadImage("IMÁGENES/segundoE1.png");
  segundoE2 = loadImage("IMÁGENES/segundoE2.png");

  // Carga el sonido de fondo del sketch
  miSonido = loadSound("SONIDO/nostalgia.mp3");
}

function setup() {
  // Función que inicializa el programa y configura los elementos principales
  createCanvas(windowWidth, windowHeight); // Crea un canvas del tamaño de la ventana

  miSonido.loop(); // Asigna que el sonido se reproduzca en bucle

  botonAvanzar = createButton("Continuar"); // Crea el botón Continuar
  botonAvanzar.position(width / 2 - 40, height - 80); // Posiciona el botón en el centro horizontal y cerca de la parte inferior de la ventana
  botonAvanzar.mousePressed(avanzarEstado); // Ejecuta la función avanzarEstado() al hacer clic en el botón

  botonInicio = createButton("Haz clic para volver al inicio"); // Crea el botón de reinicio
  botonInicio.position(width / 2 - 90, height - 80); // Desplaza el botón 90 px a la izquierda y 80 px desde la parte inferior
  botonInicio.mousePressed(volverInicio); // Asigna una función al botón: cuando se presiona, se vuelve al inicio
  botonInicio.hide(); // Oculta el botón al iniciar, no se muestra en pantalla al comienzo

  for (let i = 0; i < 40; i++) {
    // Bucle que crea 40 círculos
    circulosConfusion.push(new CirculoConfusion()); // Los círculos se agregan al array circulosConfusion
  }

  for (let i = 0; i < 150; i++) {
    // Bucle que crea 150 lagrimas
    lagrimas.push(new Lagrima()); // Las figuras se agregan al array Lagrima
  }
}

function draw() {
  // Función que se ejecuta en bucle 60 veces por segundo
  switch (
    estado // Evalúa el valor de la variable "estado" para decidir qué bloque ejecutar
  ) {
    case 0: // Caso 0: pantalla inicial
      botonAvanzar.show(); // Muestra el botón para avanzar a la siguiente pantalla
      botonInicio.hide(); // Oculta el botón de inicio
      pantallaInicio(); // Llama a la función que dibuja la pantalla de inicio
      break; // Termina este caso

    case 1: // Caso 1: contenido intermedio
      botonAvanzar.show(); // Mantiene visible el botón de avanzar
      botonInicio.hide(); // Oculta el botón de inicio
      pantallaExperiencia(); // Dibuja la pantalla de experiencia
      break; // Termina este caso

    case 2: // Caso 2: pantalla final
      botonAvanzar.hide(); // Oculta el botón de avanzar
      botonInicio.show(); // Muestra el botón para volver al inicio
      pantallaFinal(); // Dibuja la pantalla final
      break; // Termina este caso
  }
}

function fondoCompleto(img) {
  // Función para poner imágenes como fondo sin deformar
  let escala = max(width / img.width, height / img.height); // Calcula la escala necesaria para que la imagen cubra toda la pantalla usando el valor mayor entre ancho y alto para evitar espacios vacíos

  let nuevoAncho = img.width * escala; // Calcula el nuevo ancho de la imagen después de aplicar la escala
  let nuevoAlto = img.height * escala; // Calcula el nuevo alto de la imagen después de aplicar la escala

  let x = (width - nuevoAncho) / 2; // Centra la imagen horizontalmente calculando el desplazamiento en X
  let y = (height - nuevoAlto) / 2; // Centra la imagen verticalmente calculando el desplazamiento en Y

  image(img, x, y, nuevoAncho, nuevoAlto); // Dibuja la imagen en pantalla con las nuevas dimensiones y posición
}

function pantallaInicio() {
  // Función que dibuja la pantalla de inicio del programa

  if (keyIsPressed) {
    // Si el usuario presiona cualquier tecla, se activa este bloque

    background(0); // Pinta el fondo de color negro
    textSize(18); // Define el tamaño del texto en 18 píxeles
    textAlign(LEFT, TOP); // Alinea el texto a la izquierda y arriba

    for (let x = 0; x <= width; x += 236) {
      // Bucle horizontal recorre la pantalla de izquierda a derecha

      for (let y = 0; y <= height; y += 20) {
        // Bucle vertical recorre la pantalla de arriba hacia abajo

        fill(random(210, 255), random(0, 20), random(0, 20), 50); // Asigna un color rojo random con transparencia para cada texto

        text("nadie te va a querer como yo", x, y); // Dibuja el texto "nadie te va a querer como yo" repetido en forma de patrón en toda la pantalla
      }
    }

    fondoCompleto(segundoE0); // Dibuja una imagen de fondo completa encima del patrón de texto
  } else if (estado == 0) {
    // Si no se presiona una tecla y el estado es 0, se muestra la pantalla inicial

    background(176, 21, 21); // Asigna el color rojo oscuro en valores RGB
    noStroke(); // Elimina el borde de las figuras
    fill(92, 6, 6, 100); // Asigna un color rojo más oscuro con transparencia
    ellipse(width / 2, height / 2, Diametro[index]); // Dibuja un círculo en el centro con un diámetro que cambia según el array "Diametro"

    if (frameCount % 10 == 0) {
      // Cada 10 frames se ejecuta el cambio de valor

      index++; // Avanza al siguiente valor del array

      if (index >= Diametro.length) {
        // Si llega al final del array cumple la siguente función

        index = 0; // Vuelve al inicio (loop infinito)
      }
    }

    fondoCompleto(fondoEstado0); // Dibuja la imagen de fondo de la pantalla de inicio
  }
}

function pantallaExperiencia() {
  // Función que dibuja la pantalla de experiencia

  if (keyIsPressed) {
    // Si el usuario presiona cualquier tecla, se activa este bloque

    background(0); // Pinta el fondo de color negro

    tamanoCirculo = random(20, 250); // Genera un tamaño aleatorio para el círculo
    bordeCirculo = random(1, 20); // Genera un grosor de borde aleatorio para el círculo

    stroke(82, 5, 5); // Asigna el color rojo oscuro al borde del círculo en valores RGB
    strokeWeight(bordeCirculo); // Aplica el grosor del borde generado aleatoriamente
    fill(255, 0, 0); // Asigna el color rojo intenso de relleno del círculo
    circle(width / 2, height / 2, tamanoCirculo); // Dibuja un círculo en el centro de la pantalla con tamaño variable

    fondoCompleto(segundoE1); // Dibuja una imagen de fondo encima del círculo
  } else {
    // Si no se presiona ninguna tecla

    background(176, 21, 21); // Pinta el fondo de rojo oscuro en valores RGB

    // Dibujar lágrimas
    for (let l of lagrimas) {
      // Recorre cada objeto del array "lagrimas"

      l.caer(); // Actualiza la posición de la lágrima con movimiento hacia abajo
      l.mostrar(); // Dibuja la lágrima en pantalla
    }

    fondoCompleto(fondoEstado1); // Dibuja la imagen de fondo correspondiente a la pantalla de experiencia
  }
}

function pantallaFinal() {
  // Función que dibuja la pantalla final del programa

  background(176, 21, 21); // Pinta el fondo con un color rojo oscuro en valores RGB
  textSize(18); // Define el tamaño del texto en 18 píxeles
  textAlign(LEFT, TOP); // Alinea el texto a la izquierda y arriba

  for (let x = 0; x <= width; x += 175) {
    // Recorre la pantalla horizontalmente dejando una separación de 175 píxeles

    for (let y = 0; y <= height; y += 20) {
      // Recorre la pantalla verticalmente dejando una separación de 20 píxeles

      fill(random(100, 255), random(100, 255), random(100, 255), 100); // Asigna un color aleatorio con transparencia para cada texto
      text("cambiaré, lo prometo", x, y); // Dibuja el texto "cambiaré, lo prometo" repetido formando un patrón sobre toda la pantalla
    }
  }

  if (keyIsPressed) {
    // Si el usuario presiona cualquier tecla
    background(0); // Cambia el fondo a color negro

    for (let c of circulosConfusion) {
      // Recorre todos los círculos almacenados en el array

      c.mostrar(); // Dibuja y anima cada círculo de confusión
    }

    fondoCompleto(segundoE2); // Dibuja la segunda imagen correspondiente al estado final
  } else {
    // Si no se presiona ninguna tecla

    fondoCompleto(fondoEstado2); // Muestra la imagen principal del estado final
  }
}

function avanzarEstado() {
  // Función que avanza entre las pantallas del programa

  userStartAudio(); // Activa el audio después de la interacción del usuario

  if (!miSonido.isPlaying()) {
    // Comprueba si el sonido no se está reproduciendo

    miSonido.loop(); // Inicia el sonido en reproducción continua
  }

  if (estado < 2) {
    // Comprueba que aún no se haya llegado al último estado

    estado++; // Avanza al siguiente estado de la experiencia
  }
}

function volverInicio() {
  // Función que reinicia la experiencia y vuelve a la pantalla inicial

  estado = 0; // Asigna el valor 0 a la variable estado para mostrar nuevamente la pantalla de inicio
}

function windowResized() {
  // Función que se ejecuta automáticamente cuando cambia el tamaño de la ventana

  resizeCanvas(windowWidth, windowHeight); // Ajusta el tamaño del canvas al nuevo ancho y alto de la ventana

  botonAvanzar.position(width / 2 - 40, height - 80); // Reposiciona el botón "Continuar" para que permanezca centrado horizontalmente y cerca de la parte inferior

  botonInicio.position(width / 2 - 100, height - 80); // Reposiciona el botón "Haz clic para volver al inicio" para mantenerlo centrado y cerca de la parte inferior
}
```
