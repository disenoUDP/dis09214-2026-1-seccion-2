# EXAMEN
# Manspreading

**Autor:** Amanda Venegas

## Información del proyecto

**Nombre del proyecto:** Manspreading

**Autor:** Amanda Venegas

---

# Descripción objetiva

## ¿Qué es el proyecto?

*Manspreading* es un proyecto interactivo desarrollado en p5.js que busca representar de forma visual el fenómeno del manspreading y evidenciar cómo este comportamiento puede afectar el espacio de otras personas en el transporte público.

## ¿Qué se ve en pantalla?

El proyecto presenta tres pantallas: una pantalla de inicio, una pantalla de instrucciones y una pantalla de interacción.

En la escena principal se observa el interior de un vagón de metro con un hombre y una mujer sentados uno al lado del otro. A medida que el usuario interactúa mediante clics, el personaje masculino comienza a ocupar cada vez más espacio con la apertura de sus piernas.

## ¿Qué elementos visuales aparecen?

* Fondo del metro.
* Personaje masculino.
* Personaje femenino.
* Ícono de enojo.
* Botón de reinicio.
* Texto con título e instrucciones.
* Partículas y cambios de color como respuesta a la interacción.

---

# Descripción conceptual

La idea central del proyecto es representar visualmente cómo una acción cotidiana, como el manspreading, puede afectar el espacio compartido y generar incomodidad en otras personas.

El sistema utiliza la interacción del usuario para exagerar progresivamente el comportamiento del personaje masculino, haciendo visible una situación que normalmente puede pasar desapercibida.

### Regla de oro del sistema

**A mayor cantidad de clics, mayor es el espacio que ocupa el personaje masculino y mayor es la incomodidad que experimenta la mujer.**

### Relación con la problemática de género

El proyecto representa cómo ciertas conductas cotidianas pueden reflejar desigualdades en el uso del espacio público. El manspreading muestra una ocupación desproporcionada del espacio compartido, obligando a la mujer a desplazarse y manifestando visualmente la incomodidad que esto genera.

---

# Input / Output y sistema

## Input

* Clic del mouse.
* Botón de reinicio.

## Proceso

Cada clic modifica distintas variables del programa.

El personaje masculino aumenta gradualmente el tamaño de su cuerpo y separa más sus piernas. Cuando se alcanza el máximo de interacción, la mujer se desplaza, aparece un ícono de enojo, se generan partículas y comienza a reproducirse un sonido.

## Output

* Crecimiento del personaje masculino.
* Cambio de color del fondo.
* Desplazamiento de la mujer.
* Aparición del ícono de enojo.
* Sistema de partículas.
* Reproducción de sonido.
* Posibilidad de reiniciar la interacción.

---

# Pensamiento computacional

El funcionamiento del proyecto se basa en la interacción del usuario mediante clics. Cada clic produce cambios dentro de la escena, haciendo que el personaje masculino ocupe cada vez más espacio y que la mujer reaccione alejándose.

A medida que aumenta la cantidad de clics, también cambian otros elementos del sistema, como el color del fondo, la aparición del ícono de enojo, las partículas y el sonido. Todos estos cambios siguen reglas definidas en el programa y ocurren en momentos específicos de la interacción.

La experiencia está organizada en tres estados: una pantalla de inicio, una pantalla de instrucciones y una pantalla de interacción. Además, el usuario puede volver al estado inicial utilizando el botón de reinicio.


---

# Referentes

## Referentes visuales

* Interior del Metro de Santiago como escenario cotidiano del transporte público.
* Señaléticas e ilustraciones de campañas sobre el uso responsable del espacio público.

<img width="451" height="640" alt="image" src="https://github.com/user-attachments/assets/26182615-0403-4dac-8791-052bee865f94" />
Universitat Oberta de Catalunya. (2023, 22 de marzo). Mansplaining, manspreading y gaslighting. UOC News. https://www.uoc.edu/es/news/2023/074-mansplaining

## Referentes teóricos

* Concepto de manspreading como práctica relacionada con el uso desigual del espacio compartido.
* Reflexiones sobre convivencia y género en espacios públicos.

---

# Diagrama de flujo
---
### Mi diagrama de flujo : https://miro.com/app/board/uXjVHPyg7iQ=/
---
<img width="257" height="493" alt="image" src="https://github.com/user-attachments/assets/bc1e5e11-77ea-4da1-aa3e-ffb6abfda6f0" />
<img width="246" height="534" alt="image" src="https://github.com/user-attachments/assets/34433890-8c00-4ffe-ac68-46682577d1d3" />

---
### Mi codigo p5js : https://editor.p5js.org/amanda.venegas1/sketches/HXfX3WCua
### correccion de mi codigo : https://editor.p5js.org/amanda.venegas1/sketches/dObnXFG0l
---


### Mi codigo nuevo 

```
// Estas son variables para guardar las imágenes y el sonido
let imagenFondo;
let chicaI;
let chicoI;
let enojoI;
let imagenReinicio;
let estado = 0; // Controla las pantallas del juego (0: Inicio, 1: Instrucciones, 2: Juego)
let click = 0; // Cuenta cuántas veces el usuario hace clic 
let rojo; // Variable de color rojo después usada en el map
let miSonido;

let particulas = []; // Arreglo asignado para guardar las partículas creadas por la clase

// Declare y agrupe variables 
let chico = { // Todas las variables del chico 
  x: 1140, // Posición de la imagen del chico en X
  y: 550, // Posición de la imagen del chico en Y          
  ancho: 450, // Tamaño del ancho de la imagen
  alto: 550, // Tamaño del alto de la imagen
  piernaD: 1170, // Posición de la pierna derecha
  piernaI: 1040, // Posición de la pierna izquierda  
  tamPierna: 90 // Tamaño del ancho de las piernas
};

let chica = { // Variables de la chica 
  x: 700, // Posición de la imagen de la chica en X          
  y: 450, // Posición de la imagen de la chica en Y          
  circuloX: 830, // Valor de X del círculo que es la cabeza 
  alto: 550 // Mantenemos el alto para controlar su tamaño vertical       
};

class Particula { // Estructura o molde para crear cada partícula de enojo
  constructor(x, y) { // Inicializa los valores al crear cada partícula
    this.x = x; // Coordenada X inicial
    this.y = y; // Coordenada Y inicial
    this.vx = random(-3, 3); // Velocidad aleatoria en el eje X
    this.vy = random(-7, -3); // Velocidad aleatoria hacia arriba en el eje Y
    this.alfa = 255; // Transparencia inicial de la partícula
    this.tamano = random(18, 35); // Diámetro aleatorio de la partícula
  }

  actualizar() { // Calcula el movimiento y desvanecimiento
    this.x += this.vx; // Suma la velocidad a la posición X
    this.y += this.vy; // Suma la velocidad a la posición Y
    this.alfa -= 7; // Disminuye la transparencia para desvanecerla
  }

  mostrar() { // Dibuja la partícula en el lienzo
    noStroke(); // Quita el borde
    fill(150, 20, 20, this.alfa); // Rellena con color rojo oscuro y aplica la transparencia actual
    circle(this.x, this.y, this.tamano); // Dibuja un círculo
  }

  estaMuerta() { // Comprueba si la partícula ya desapareció por completo
    return this.alfa <= 0; 
  }
}

function preload() { // Sirve para cargar archivos antes de que empiece el programa 
  miSonido = loadSound("tusoundtrack.mp3");
  imagenFondo = loadImage("metrofondo.png");
  chicaI = loadImage("chica.png");
  chicoI = loadImage("chico.png");
  enojoI = loadImage("enojo.png");
  imagenReinicio = loadImage("reinicio.png");
}

function setup() { // Es una función que se ejecuta solo una vez en el programa 
  createCanvas(1920, 1080); // Crea un lienzo en X, Y 
  frameRate(20); // Limita cuántas veces por segundo se ejecuta el draw 
  miSonido.setVolume(0.15); // Define el volumen del soundtrack
}

function draw() { // Es una función que se ejecuta constantemente en bucle
  if (estado == 0) { // Si el estado es 0 muestra la bienvenida
    pantallaInicio();
  } else if (estado == 1) { // Si el estado es 1 muestra las instrucciones
    pantallaInstrucciones();
  } else { // Si el estado es diferente muestra los elementos del juego
    backgroundS(); // Organiza los elementos del fondo 
    gestionarParticulas(); // Controla y borra las partículas
    mujer(); // Dibuja las partes de la chica
    hombre(); // Dibuja los elementos del chico
    titulo(); // Dibuja los elementos del título
    enojo(); // Dibuja la imagen del símbolo de enojo y activa partículas
    botonReiniciar(); // Dibuja el botón para volver a empezar
  }
}

function pantallaInicio() { // Elementos de la pantalla de bienvenida
  background(0); // Fondo negro
  textAlign(CENTER, CENTER); // Centra los textos en horizontal y vertical
  textFont("Georgia"); // Define la tipografía
  fill(255); // Color de texto blanco

  textSize(80); // Tamaño del título 
  text("Manspreading", width / 2, height / 2 - 180);

  textSize(40); // Texto informativo dividido en renglones
  text(
    "Es una costumbre en la que algunos hombres abren\n" +
    "excesivamente las piernas al sentarse, ocupando más\n" +
    "espacio del necesario y llegando a incomodar a la\n" +
    "persona que está a su lado.",
    width / 2,
    height / 2 + 50
  );

  textSize(30);
  fill(250, 250, 250, 200); // Blanco con un poco de transparencia
  text("Haz clic en la pantalla para continuar", width / 2, height / 2 + 380);
}

function pantallaInstrucciones() { // Menú intermedio con las reglas
  background(50); // Fondo gris oscuro
  fill(255);
  textAlign(CENTER);

  textSize(60); // Encabezado de la pantalla
  text("Instrucciones", width / 2, height / 2 - 250);

  textSize(35); // Lista de pasos para el usuario
  text(
    "1. Haz clic en la pantalla para interactuar.\n \n" +
    "2. Cada clic aumenta el espacio que ocupa el personaje masculino.\n \n" +
    "3. La interacción tiene un máximo de 7 clics.\n \n" +
    "4. Observa los cambios en la escena.\n \n" +
    "5. Reinicia cuando quieras.",
    width / 2,
    height / 2 + 20
  );

  textSize(30);
  fill(250, 250, 250, 200);
  text("Haz clic en la pantalla para comenzar", width / 2, height / 2 + 380);
}

function backgroundS() { // Función de los elementos del fondo, map e imágenes
  rojo = map(chico.ancho, 450, 510, 0, 255); // Convierte el rango del ancho a un rango de color de 0 a 255 
  background(rojo, 0, 0); // Crea un fondo que se tiñe usando la variable rojo

  image(imagenFondo, 0, 0, width, height); // Carga la imagen de fondo acoplada al lienzo
  fill(rojo, 0, 0, 150); // Rellena con un filtro rojo translúcido
  rect(0, 0, width, height); // Tamaño del rectángulo que cubre la pantalla
}

function mujer() { // Elementos del personaje de la chica
  noStroke(); // Quita el borde de las figuras
  
  // Calculamos el ancho ideal basado en la altura para que no se deforme
  let anchoProporcional = (chicaI.width / chicaI.height) * chica.alto;

  image(chicaI, chica.x, chica.y, anchoProporcional, chica.alto); // Coloca la imagen de la chica

  // Si el usuario llega al clic 6 el círculo de la cabeza cambia a colores locos
  if (click == 6) {
    fill(random(255), random(255), random(255));
    circle(chica.circuloX, chica.y - 100, random(300));
  } else { // Si no ha llegado a 6 clics mantiene el círculo rosa fijo
    fill(238, 157, 225);
    circle(chica.circuloX, chica.y - 100, 180); 
  }
}

function hombre() { // Esta función dibuja al personaje chico
  push(); // Guarda la configuración actual del dibujo 
  fill(91, 69, 169); // Define el color morado para las piernas
  noStroke();

  // Dibuja la pierna izquierda y la pierna derecha
  rect(chico.piernaI, chico.y + 200, chico.tamPierna, 300);
  rect(chico.piernaD, chico.y + 200, chico.tamPierna, 300);

  imageMode(CENTER); // Configura el dibujo de la imagen desde el centro
  image(chicoI, chico.x, chico.y - 40, chico.ancho, chico.alto); // Dibuja la imagen del chico ajustando la altura
  pop(); // Vuelve a la configuración original del programa
}

function titulo() { // Esta función dibuja el título superior
  push();
  fill(255); // Color blanco para el texto
  textSize(45); // Tamaño del texto
  textFont("Georgia");
  textAlign(CENTER, TOP); // Centrado horizontal alineado arriba
  text("¿Cómo ocupas el espacio?", width / 2, 50); // Texto impreso
  pop();
}

function enojo() { // Elementos de la imagen de enojo y partículas
  if (click >= 5) { // Después de 5 clics realiza lo siguiente
    push();
    translate(chica.circuloX + 70, chica.y - 130); // Desplaza el origen a la posición ajustada de la cabeza
    rotate(frameCount * 0.05); // Rota la imagen continuamente sobre su propio centro
    imageMode(CENTER);
    image(enojoI, 0, 0, 110, 110); // Dibuja el símbolo de enojo
    pop();

    if (frameCount % 2 == 0) { // Crea una partícula nueva de forma intermitente cada 2 cuadros
      let origenX = chica.circuloX  + random(-40, 40); // Variación aleatoria en X
      let origenY = (chica.y - 130) + random(-40, 40); // Variación aleatoria en Y
      particulas.push(new Particula(origenX, origenY)); // Añade una nueva partícula al arreglo
    }
  }
}

function gestionarParticulas() { // Recorre el arreglo al revés para actualizar y borrar partículas
  for (let i = particulas.length - 1; i >= 0; i--) {
    particulas[i].actualizar(); // Calcula la posición y la opacidad de la partícula
    particulas[i].mostrar(); // Pinta la partícula en la pantalla
    
    if (particulas[i].estaMuerta()) { // Si la transparencia llegó a 0 la remueve
      particulas.splice(i, 1); 
    }
  }
}

function botonReiniciar() { // Construye visualmente el botón de reinicio
  let botonX = width - 80; 
  let botonY = 60;

  push();
  fill(0); // Círculo base negro
  stroke(255); // Borde blanco
  circle(botonX, botonY, 70); 
  imageMode(CENTER);
  image(imagenReinicio, botonX, botonY, 45, 45); // Icono del botón centrado
  pop();
}

function mousePressed() { // Esta función se ejecuta cada vez que el usuario hace clic con el mouse
  if (estado == 0) { // Si está en inicio pasa a las instrucciones
    estado = 1;
    return;
  }

  if (estado == 1) { // Si está en instrucciones pasa al juego
    estado = 2;
    return;
  }

  if (estado == 2) { // Si ya está dentro del simulador interactivo
    let distanciaBoton = dist(mouseX, mouseY, width - 80, 60); // Calcula la distancia entre el mouse y el botón

    if (distanciaBoton < 35) { // Si hace clic dentro del rango del botón reinicia el programa
      reiniciar();
      return; 
    }

    if (click < 6) { // Si se da menos de 6 clics deforma y expande las dimensiones del chico
      chico.ancho += 20;  
      chico.alto += 35; 
      chico.piernaD += 20; // Abre la pierna derecha
      chico.piernaI -= 30; // Abre la pierna izquierda hacia afuera
      chico.tamPierna += 8; // Engrosa los rectángulos de las piernas
      click++; // Suma 1 al contador de clics
    }

    if (click == 5) { // Si el usuario da exactamente 5 clics desplaza a la chica
      chica.x -= 100; // Mueve la imagen de la chica a la izquierda
      chica.circuloX -= 100; // Mueve también el círculo de su cabeza
    }

    if (click == 6) { // En el último clic arranca el soundtrack en bucle continuo si no estaba sonando
      if (!miSonido.isPlaying()) {
        miSonido.loop();
      }
    }
  }
}

function reiniciar() { // Restablece todas las variables globales a sus valores originales
  estado = 0; 
  click = 0;
  miSonido.stop(); // Detiene la música por completo
  particulas = []; // Limpia el arreglo de partículas

  // Valores restaurados del chico
  chico.x = 1120;
  chico.y = 550;
  chico.ancho = 450;
  chico.alto = 550;
  chico.piernaD = 1150;
  chico.piernaI = 1020;
  chico.tamPierna = 90;

  // Valores restaurados de la chica
  chica.x = 700;
  chica.y = 450;
  chica.circuloX = 820;
}
```
