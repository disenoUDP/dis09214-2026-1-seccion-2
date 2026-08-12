# sesión 06 - 14/04
# Examen

# La Mirada Masculina  
### Autoras: Dafne Hernandez, Josefina Puña  
## Descripción del proyecto  
### ¿Qué es?  
Es un sketch hecho en P5.js que tiene como objetivo visibilizar y reflexionar sobre el trato que reciben las mujeres en cuanto a la estética y los estándares de belleza impuestos por la sociedad, donde se ve a las mujeres como un objeto para el deleite de los hombres (male gaze), reduciendolas a un objeto sexual en vez de ser vistas como personas con profundidad psicológica.  
A través de elementos visuales, sonoros e interactivos, buscamos representar la presión constante que existe sobre la apariencia femenina, donde se espera que las mujeres tengan una imagen “perfecta”, inalcanzable y muchas veces sexualizada para el disfrute de los hombres. Esta exigencia crea inseguridades, frustración y la sensación de no ser suficientes, ya que los modelos de belleza suelen ser irreales e imposibles de alcanzar. El sketch pone en evidencia la constante presión estética que viven día a día las mujeres, influyendo en la percepción que tienen de sí mismas. De esta forma, nuestro proyecto utiliza el lenguaje visual y la programación creativa para transformar una problemática de género en una experiencia interactiva y reflexiva.  

### ¿Qué se ve en pantalla?  
En el sketch que se regula al tamaño de la ventana se pueden apreciar tres estados:  
1. Instrucciones: Aquí se guia y se explica al usuario los pasos que tiene que seguir para tener la experiencia completa.
2. Televisión: Este es el estado de principal interacción. Se aprecia principalmente un mueble con una televisión antigua, la que muestra distintas imágenes en su pantalla, la primera es la estática, seguida de las rayas verticales que aparecen cuando una televisión no tiene señal, y por último aparecen imágenes de mujeres atractivas para la mirada mascuina. Cada una tiene un audio que tiene directa relación con lo que muestra la pantalla.  
3. Teléfono: Aparece un celular agarrado por una mano, con imágenes rectangulares de distintos tonos de piel, algunos con un tick y otros con una equis.

### ¿Qué elementos visuales aparecen?  
Principalmente imágenes y botones, también se pueden apreciar franjas, rectangulos, emoticones y distintos colores.  

## Descripción conceptual  
### Idea central del proyecto y su relación con el sistema diseñado  
Este sketch utiliza la televisión como símbolo de los medios de comunicación, que durante mucho tiempo han mostrado imágenes de mujeres desde una mirada centrada en la apariencia física. La primera parte, donde aparece la estática, representa la saturación de mensajes mediáticos que constantemente rodean a las personas. Luego, las barras de colores hacen referencia a las transmisiones televisivas y los sistemas de difusión audiovisual, haciendo referencia a los mecanismos mediante los cuales se producen y distribuyen estos discursos visuales.  

El rápido paso de fotografías refleja el consumo acelerado de imágenes que ocurre tanto en la televisión como en las redes sociales. Debido a la velocidad con que aparecen, no hay tiempo para analizarlas críticamente, lo que normaliza ciertos cuerpos y rasgos como ideales de belleza. Aquí empieza a sonar el audio del episodio 2 de "Formas de Ver" de John Berger que habla de las mujeres de la época y su función de complacer visualmente al hombre.  

La mano masculina sosteniendo un celular representa el uso de las redes sociales y otras plataformas, donde las personas están expuestas constantemente a imágenes e ideales de belleza. En la pantalla aparecen distintos tonos de piel, representendo una abstracción del cuerpo femenino, algunos marcados con un tick y otros con una equis, evidenciando cómo ciertos rasgos físicos los hombres aceptan y valoran, mientras que otros los rechazan o consideran menos deseables.  

Desde la perspectiva del male gaze (mirada masculina), nuestra obra evidencia cómo los medios convierten a las mujeres en imágenes para ser observadas y evaluadas, asociando su valor principalmente a su aspecto físico. Así, nuestro sketch invita a reflexionar sobre cómo los medios influyen en la forma en que entendemos la belleza y cómo las mujeres perciben su propia imagen.  

### ¿Cuál es la regla de oro de tu sistema?  
Al presionar el mouse en uno de los botones de la televisión, la imagen en la pantalla de la tele cambia, el primer clic lleva a las barras de colores, el segundo clic lleva a las fotos, y finalmente el tercero nos devuelve a la estática.  

### ¿Cómo se relaciona esta lógica con la problemática de género elegida?  
El presionar el mouse y cambiar de "canal" en la televisión está relacinado con el deseo de las mujeres de querer escapar de los estándares de belleza y del male gaze, pero siempre encontrandose con otra situación similar y agobiante. Finalmente es el hombre el que esta cambiando de "canal", representando que es él quién controla lo que la mujer cree de sí misma.     

## Input / Output y sistema  
### ¿Qué datos entran?  
* El usuario presiona el mouse.  
* la estática y las barras (franjas) generados por la función random.  
* Fotos en loop.
* Cambio de tamaño de ventana.
* El usuario presiona el botón.
* El usuario presiona la letra Q.  
  
### ¿Cómo se procesan y transforman?  
El código detecta y transforma las acciones mediante:  

* Condicionales.  
* Loops.  
* Rotaciónes.  
* Generación random.    
* Funciones propias.
* Botones.  
  
### ¿Qué respuesta visual producen?  
En respuesta a las distintas interacciones del usuario se genera:  

* La pantalla de la tele cambia su contenido (clic).  
* Aparece la pantalla del celular.  
* La estática y las franjas cambian al azar.
* Aparecen distintos tonos de piel en el celular.  


## Pensamiento computacional    
### Reglas que gobiernan el sistema (inputs, procesos, outputs)  
Las reglas que gobiernan el sistema son:  

* Si el usuario presiona el mouse en el circulo de la tele: Se cambia la pantalla del televisor.  
* Si el usuario presiona el botón "Continuar": Se cambia a la siguiente "pantalla" del proyecto.
* Si el usuario agranda o achica la ventana del sketch: El sketch cambia de tamaño proporcionalmente.
* Si el usuario presiona la letra Q: Aparecen en la pantalla del celular distintos tonos de piel, algunos con tick y otros con equis.
  
### Explicación del sistema de interactividad    
El programa detecta las siguientes acciones (inputs): los clics, los random, las teclas, tamaño de la ventana, etc. Las interpreta (procesos) mediante condiciones, variables o cálculos y entrega una respuesta (output) visible en el sketch: cambia y adapta el contenido visual del televisor o de la pantalla.  

## Referentes  
#### "Do Women Have To Be Naked To Get Into the Met. Museum?" de Guerrilla Girls (1989)  
La obra evidencia que mientras las mujeres artistas estaban excluidas de las galerías, sus cuerpos eran utilizados masivamente como meros objetos decorativos y sexuales para el disfrute visual de los hombres.

![Do Women Have To Be Naked To Get Into the Met. Museum?](https://artishockrevista.com/wp-content/uploads/2024/03/Guerrilla-Girls-Naked-1989.jpg)   

### Discurso película Barbie (2023)  
En este discurso dicho por la actriz America Ferrera se visibiliza todas las cosas que se le exigen a una mujer, sobre lo contradictorio y difícil que es siquiera intentar seguir los estándares impuestos por la sociedad y sobre complacer a los hombres físicamente. "Se supone que debes mantenerte bonita para los hombres, pero no tanto como para tentarlos demasiado" 

![Discurso Barbie](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSwCsnEQ3rsLDcF-zEyRYjwtSKs_Z6ersveWw&s)  


### La serie "Propped" de Jenny Saville (1992)  
La artista británica es conocida por sus enormes pinturas al óleo de cuerpos femeninos que escapan al canon de extrema delgadez. En "Propped" y otras obras, desafía el Male gaze al mostrar la piel con pliegues, marcas de celulitis y proporciones reales, celebrando el cuerpo tal y como es.  

![Propped](https://miro.medium.com/0*mgCLMtGMiNAHAGNi)  


### John Berger / Formas de ver, Episodio 2 (1972)  
John Berger afirma que muchas imágenes de mujeres en el arte occidental no las presentan como sujetos con autonomía, sino como objetos de observación y deseo. "Los hombres actúan y las mujeres aparecen. Los hombres miran a las mujeres. Las mujeres se observan a sí mismas siendo observadas."  
Berger crítica al poder, a las convenciones de la historia del arte y a la forma en que la cultura ha enseñado a hombres y mujeres a mirar y a mirarse.  

[![Formas de ver, Episodio 2](https://img.youtube.com/vi/Qud_422WKZY/0.jpg)](https://www.youtube.com/watch?v=Qud_422WKZY)  


## Diagrama de flujo  
![Diagrama de flujo](https://github.com/Josefina130/examen.md/blob/506fda2c8c1642d625609efd2cb29657ef498e46/Copia%20de%20%20Diagrama%20de%20flujo.png)  
[PDF Diagrama de flujo](https://github.com/Josefina130/examen.md/blob/main/Copia%20de%20%20Diagrama%20de%20flujo.png)  



## Código p5.js  

 ```  
let estado = 0; // Se crea la variable para definir el estado de las pantallas
let animando = false; // Se declara la variable animando para generar la animación más adelante en estado false
let visible = false; // // Se declaqra la variable visible para generar la visibilidad
let imagY; // Se declara la variable para la posición Y de la imagen
let imagX; // Se declara la variable para la posición X de la imagen
let imagW; // Se declara la variable para el ancho de la imagen
let imagH; // Se declara la variable para el alto de la imagen
let TopeC; // Se declara la variable para el punto donde debe parar la animación
let botonSiguiente; // Se declara la variable para el botón "Continuar"
let referencia; // Se declara la variable referencia 
let estadoBoton = 0; // Se declara la variable estadoBoton para el estado de la TV
let Fotos = []; // Se declara la variable Fotos
let index = 0;  // Se declara la variable index 
let r = 150; // Se declara la variable r para el color con un valor de 150
let g = 100; // Se declara la variable r para el color con un valor de 100
let b = 80; // Se declara la variable r para el color con un valor de 80
let tamC = 60; // Se declara la variable tamC para el tamaño del cuadrado con un valor de 60
let tam2 = 80; // Se declara la variable tam2 para el tamaño del cuadrado con un valor de 80
let tamaños = [60,70,80,90,100]; // Se declara la variable tamaños en donde se agregan los diversos tamaños que tendrá 
let tamaños2 = [70,80,90,100] // Se declara la variable tamaños2 en donde se agregan los diversos tamaños que tendrá 
let indexA = 0; // Se declara la variable indexA 
let emojis = ["✔️", "❌"]; // Se declara la variable emojis en donde se agregan los emojis
let foto1, foto2, foto3, foto4, foto5, foto6, foto7, foto8, foto9, foto10; // Se declara una variable con todas las fotos juntas

function preload(){ // Se activa la función para pre-cargar las imagenes y el sonido
  tele = loadImage('assets/tele.png');
  celu = loadImage ('assets/celular.png');
  mueble = loadImage ('assets/mueble.png');
  foto1 = loadImage('assets/foto1.jpg');
  foto2 = loadImage ('assets/foto2.jpg');
  foto3 = loadImage ('assets/foto3.jpg');
  foto4 = loadImage ('assets/foto4.jpg');
  foto5 = loadImage ('assets/foto5.jpg');
  foto6 = loadImage ('assets/foto6.jpg');
  foto7 = loadImage ('assets/foto7.jpg');
  foto8 = loadImage ('assets/foto8.jpg');
  foto9 = loadImage ('assets/foto9.jpg');
  foto10 = loadImage ('assets/foto10.jpg');
  est = loadSound ("EstaticaTV.mp3");
  john = loadSound ("John.mp3");
  estColor = loadSound ("TV.mp3");
}

function setup() {
  
  let anchoPantalla = min(windowWidth, (windowHeight * 16) / 9); // Se crea la variable y se calcula el ancho de la pantalla asegurando que no sobrepase el ancho de la ventana manteniendo la proporción vertical de 16:9
  let altoPantalla = (anchoPantalla * 9) / 16; // Se crea la variable y se calcula el alto de la pantalla forzando que el canvas se mantenga siempre en el formato 16:9
 createCanvas(anchoPantalla, altoPantalla); // Se crea el canvas con las variables de ancho y alto (1920x1080)
  imageMode(CENTER); // Se activa la opción para que las imágenes estén en el centro
  
  Fotos = [foto1, foto2, foto3, foto4, foto5, foto6, foto7, foto8, foto9, foto10]; // Se cargan las fotos dentro de la variable
  botonSiguiente = createButton('Continuar'); // Se crea el botón en el canvas y se le asigna el texto
  botonSiguiente.position(width / 2 - botonSiguiente.size().width / 2, height * 0.9);
  botonSiguiente.mousePressed(cambiarEstado); // Se aplica que el botón al presionarlo hará que se cambie de estado a otro
}

function draw() {
  rectMode(CORNER) // Se activa la opción para que los rectángulos inicien desde la esquina izq
  background(220);

  switch (estado) { // Controla qué pantalla se va a ejecutar
    case 0:
      pantallaInstrucciones(); // Si el estado es 0, se ejecutan las instrucciones iniciales
      break; // Finaliza la ejecución del caso 0
    case 1:
      pantallaExperiencia(); // Si el estado es 1, se ejecuta la experiencia
      break; // Finaliza la ejecución del caso 1
    case 2:
      pantallaFinal(); // Si el estado es 2, se ejecuta la pantalla final
      break; // Finaliza la ejecución del caso 2
  }
}

function pantallaInstrucciones() { // Se inicia la función para la pantalla de instrucciones
  
  textAlign(CENTER, TOP); // Se activa la opción para que el texto quede en el centro y arriba
  background(255, 201, 201); // Se le agrega un color al fondo
  
  for (let x = 0; x <= width; x = x + 40) { // Mediante el cómando for, se crea la variable x que tiene un valor igual a 0, y si este es mayor o igual al ancho del lienzo, será igual a x + 40, (la cantidad de separación entre círculos)
    for (let y = 0; y <= height; y = y + 40) { // Mediante el cómando for, se crea la variable y que tiene un valor igual a 0, y si este es mayor o igual al alto del lienzo, será igual a y + 40, (la cantidad de separación entre círculos)
  fill(random(255), random(255)); // Se rellena de color aleatorio
  ellipse(x, y, 5); // Se crea una ellipse en la posición x e y, con un tamaño de 5
    }
  }
  fill(0); // Se rellena de color negro
  textSize(24); // Se le asigna un tamaño al texto de 24
  text("INSTRUCCIONES", width / 2 , height * 0.2 - 20); // Se crea el texto "Instrucciones" y se posiciona en la mitad del ancho del canvas, en el 20% del alto - 20 del canvas
  textSize(20); // Se le asigna un tamaño al texto de 20
  textAlign(CENTER, CENTER);  
  fill(0); 
  noStroke(); 
  
  let instrucciones = `1. Haz click en el botón de abajo para continuar.
  
2. Ya en la televisión presiona el botón superior de color gris. (MÁXIMO de 2 veces)

3. Haz click en el botón de abajo para continuar.

4. Para iniciar la interacción mantén presionada la tecla "Q".

5. Para volver al inicio haz clic en el botón.`; 
  
  
  text(instrucciones, width * 0.1, height * 0.5, width * 0.8); // Se crea el texto con la variable instrucciones y se le asigna su posición X en el 10% y 50% del canvas, con un ancho de 80%
}

function pantallaExperiencia() { // Se inicia la función para la pantalla de la Experiencia
  
  background(163, 163, 163); // Se asigna color al fondo
  fill(64, 64, 64); // Se rellena de color gris 
  rect(width * 0.0, height * 0.6, width, height); // Se crea un rectangulo que inicia en el borde en el punto 0 y al 60% de la altura del canvas, y utilizará todo el ancho y alto del canvas

  
  let anchoEst = width * 0.185; // Se declara la variable anchoEst que utiliza un 18.5% de ancho
  let altoEst = height * 0.23; // Se declara la variable altoEst que utiliza un 23% de alto
  let posXEst = width * 0.39; // Se declara la variable posXEst que inicia en el 39% del ancho canvas 
  let posYEst = height * 0.2; // Se declara la variable posYEst que inicia en el 20% del alto canvas 

  image(mueble, width * 0.5,  height * 0.7, width * 0.3, height * 0.5); // Se integra una imagen que estará posicionada en el 50% y 70% del canvas y  que utiliza un 30% del ancho y 50% del alto total
  
  
  if (estadoBoton === 0){ // Se crea una condicional que dice, si el estado del boton está en 0 ocurrirá lo siguiente 
    
  fill(0); // Se rellena de color negro
  rect(posXEst, posYEst, anchoEst, altoEst); // Se crea un rectángulo en la posición posXEst, posYEst, anchoEst, altoEst 
    
  for (let i = 0; i < 300; i++) { // Se crea un loop en el que una variable llamada i cuando esta sea menor a 300 este irá aumentando de 1 en uno
    
  let x = random (posXEst, posXEst + anchoEst); // Se crea la variable x con una posición aleatoria dentro del rectángulo + el ancho
  let y = random(posYEst, posYEst + altoEst); // Se crea la variable y con una posición aleatoria dentro del rectángulo + el alto
  let tonoEst = random (255); // Se crea la variable para el tono, que será aleatorio en la gama de blancos - grises 
    
  noStroke(); // Se desactivan los bordes
  fill(tonoEst); // Se rellena del Tono aleatorio
  rect(x, y, 3, 2); // Se crea un rectangulo en la posicion x e y, que tendrá de tamaño 3 y 2
    }
  } 
    
  else if (estadoBoton === 1){  // Se crea una segunda condicional que si es que el estado del boton es 1 ocurrirá lo siguiente
  
  
  let Colores; // Se crea la variable Colores
  Colores = ["white", "yellow", "cyan", "lime", "fuchsia", "red", "blue"]; // Se le asignan los colores a la variable
  let anchoFranja = anchoEst / Colores.length; // Se crea la variable anchoFranja que será igual al ancho de la Estática dividido por la cantidad de colores
  let glitchX = random(-10, 15); // Se crea la variable GlitchX que hará que los colores se muevan de forma aleatoria entre -10 a 15 pixeles
    
  for (let i = 0; i < Colores.length; i++){ // Cuando la variable i sea menor que la cantidad de colores, esta aumentará de uno en uno 
    
  fill(Colores[i]); // Se rellena con los colores asignados
  noStroke(); // Se quitan los bordes
  rect(posXEst + (i * anchoFranja) + glitchX, posYEst, anchoFranja + 5, altoEst); // Se crea un rectangulo que estará en la posición de la estática (Rectangulo inicial) y se sumará por el ancho de las franjas que será 5 veces más ancha para que se superpongan entre sí   
  }
  } 
    
  else if (estadoBoton === 2) { // Se crea una nueva condicional; Si el estado del boton es 2, ocurrirá lo siguiente  
  
  let fotoX = posXEst + anchoEst / 2; // Se crea una variable llamada fotoX que será igual a posXest + anchoEst partido a la  mitad
  let fotoY = posYEst + altoEst /2; // Se crea una variable llamada fotoX que será igual a posYest + altoEst partido a la mitad

  if (Fotos[index]){ // Se crea una condicional que dice que si existe una foto guardada en el index entonces esta se agrega constantemente en las posiciones establecidas
  image(Fotos[index], fotoX, fotoY, anchoEst, altoEst); // Se ubican las fotos en x e y, con las variables establecidas
  }
  if (frameCount % 10 === 0) { // Cada 10 fps se avanza a la siguiente imagen sumando 1 al index
  index = index + 1;

  if (index >= Fotos.length) { // Se crea una condicional que si se muestran todas las fotos que están en el index está volverá hasta la primera nuevamente repitiendo el ciclo 
  index = 0; 
    } 
    }  
  } 
  
  let posXBoton = width * 0.605; // Se crea la variable posXBoton para los botones que manejarán los canales, y estos se posicionan en el 60.5% de X del canvas
  let posYBoton1 = height * 0.246; // Se crea la variable posYBoton1 que irá en el 24.6% de Y del canvas
  let posYBoton2 = height * 0.325; // Se crea la variable posYBoton2 que irá en el 32.5% de Y del canvas
  let tamBoton = width * 0.03; // Se crea la variable tamBoton y se le asigna un tamaño de 0.03% del canvas
  
    image(tele, width * 0.5, height * 0.35, width * 0.3, height * 0.4 );   // Se agrega la imagen de la tv en el 50% de X del canvas, y el 35% del ancho del canvas y utiliza un 30% de ancho y un 40% de alto 
  
  fill(94, 88, 69); // Se rellena de color café grisaceo
  ellipse(posXBoton, posYBoton1, tamBoton); // Se crea una ellipse en las coordenadas x e y 
  fill(67, 63, 50); // Se rellena de color café 
  ellipse(posXBoton, posYBoton2, tamBoton); // Se crea una ellipse en las coordenadas x e y 
}

function pantallaFinal() {

  // Se copia el fondo junto al loop de las imágenes en la tv sin interacción con el botón
  
  background(163, 163, 163); // Se asigna color al fondo
  fill(64, 64, 64); // Se rellena de color gris 
  rect(width * 0.0, height * 0.6, width * 1, height * 1 ); // Se crea un rectangulo que inicia en el borde en el punto 0 y al 60% de la altura del canvas, y utilizará todo el ancho y alto del canvas
  
  let anchoEst = width * 0.185; // Se declara la variable anchoEst que utiliza un 18.5% de ancho
  let altoEst = height * 0.23; // Se declara la variable altoEst que utiliza un 23% de alto
  let posXEst = width * 0.39; // Se declara la variable posXEst que inicia en el 39% del ancho canvas 
  let posYEst = height * 0.2; // Se declara la variable posYEst que inicia en el 20% del alto canvas 

  image(mueble, width * 0.5,  height * 0.7, width * 0.3, height * 0.5); // Se integra una imagen que estará posicionada en el 50% y 70% del canvas y  que utiliza un 30% del ancho y 50% del alto total
  
  let fotoX = posXEst + anchoEst / 2; // Se crea una variable llamada fotoX que será igual a posXest + anchoEst partido a la  mitad
  let fotoY = posYEst + altoEst /2; // Se crea una variable llamada fotoX que será igual a posYEst + altoEst partido a la mitad

  if (Fotos[index]){ // Si existe una foto guardada en el index entonces se agrega esa foto constantemente en las posiciones establecidas
  image(Fotos[index], fotoX, fotoY, anchoEst, altoEst); // Se ubican las fotos en x e y, con las variables establecidas
  }
  if (frameCount % 10 === 0) { // Cada 10 fps se avanza a la siguiente imagen sumándose 1 al index
  index = index + 1;

  if (index >= Fotos.length) { // Si se muestran todas las fotos que están en el index está volverá hasta la primera nuevamente repitiendo el ciclo 
  index = 0; 
    } 
    }
   image(tele, width * 0.5, height * 0.35, width * 0.3, height * 0.4 );   // Se agrega la imagen de la tv en el 50% de X del canvas, y el 35% del ancho del canvas y utiliza un 30% de ancho y un 40% de alto 
  
  imagH = height * 0.55; // Se le asigna el valor de un 55% del alto del canvas
  imagW = imagH * 0.8; // Se le asigna el valor al ancho de la imagen, que será imagH (el alto) - el 80% del ancho del canvas
  imagX = width * 0.45; // Se le asigna el valor a la posición de X que será de 45% del ancho del canvas
  topeC = height * 0.8; // Se le asigna el valor hasta dónde debe llegar la imagen que será hasta el 80% del canvas

  if (animando) { // Se crea una condiconal que si animando está activa, se ejecuta lo siguiente
  imagY = lerp(imagY, topeC, 0.1); // El lerp se utiliza para hacer movimientos o transiciones suaves, por lo que la variable imagY inicia desde su posición (Fuera del canvas) y con el lerp llegará hasta el tope establecido, avanzando un 10% de la distancia que falta para llegar a este

  if (abs(imagY - topeC) < 1) { // Se crea una condicional que dice que abs (Valor absoluto), por lo que se calcula la diferencia restando la posición actual (imagY) y la posición final (topeC), luego abs convierte el resultado en un valor positivo para obtener la distancia real entre la imagen y el destino, y si esta es menor a 1, significa que la imagen llegó al tope y se ejecuta
  imagY = topeC; // Se le asigna el valor a imagY que será el de topeC, para que este se quede en esa posición
  animando = false; // Al estar en false, esta aún no se ejecutará
  visible = true; // Si la animación terminó, la imagen continuará visible
  }
}

  if (!animando && visible) { // Se crea una condicional que dice que si no hay animación y  la imagen está visible, ocurrirá lo siguiente
  imagY = topeC; // Se le asigna nuevamente el valor a imagY que será el de topeC, para que este se quede en esa posición
  }
  if (visible || animando) { // Se crea una condicional que dice que si la imagen todavía está visible o animándose, ocurrirá lo siguiente
  imageMode(CENTER); // Se activa la opción para que la imagen esté en el centro
  image(celu, imagX, imagY, imagW, imagH); // Se agrega la imagen del celular, que estará en las posición del valor de las variables
  noStroke(); // Se activa que no hayan bordes

}

  if (keyIsPressed && (key === 'q' || key === 'Q')){ // Se crea la condicional que dice, que si la tecla Q o q, está presionada ocurrirá lo siguiente
  if (frameCount % 20 === 0){ // Se crea otra condicional dentro de la primera, que dice que cada 20fps avanza a la siguiente figura 
  r = random(60,240); // Se le asigna un valor de color aleatorio a r
  g = r * random(0.65, 0.8); // Se le asigna un valor de color aleatorio a g, que será r por el color aleatorio
  b = g * random(0.55, 0.75); // Se le asigna un valor de color aleatorio a b, que será g por el color aleatorio
  tamC = width * random(0.03, 0.05); // Se le asigna una posición al tamaño que será del ancho x los tamaños aleatorios asignados
  tam2 = width * random(0.035, 0.052); // Se le asigna una posición al tamaño que será del ancho x los tamaños aleatorios asignados
  indexA = indexA + 1; // Si se avanza 20fps se sumará un emoji al index
  if (indexA >= emojis.length) { // Se crea una condicional que dice que si la cantidad del index es igual o mayor a la cantidad de emojis, el index volverá a 0, repitiendo el ciclo
    indexA = 0;
    }
    }
    
  rectMode(CENTER) // Se activa la opción para que las figuras estén en el centro
  let posX= width * 0.477;  // Se declara y se le asigna un valor a la variable posX que estará en el 47.7% del ancho del canvas
  let posY = height * 0.7; // Se declara y se le asigna un valor a la variable posY que estará en el 70% del alto del canvas
  fill(r,g,b);  // Se rellena con los colores antes asignados
  rect(posX, posY,tamC, tam2); // Se crea un rectangulo en las posiciones declaradas por las variables
  textSize(tamC * 0.45); // Se le asigna tamaño al texto, que será de un 45%          
  textAlign(CENTER, CENTER); // Se activa la opción en el que el texto esté en el centro del canvas
  text(emojis[indexA], posX, posY); // Se crea un texto de los emojis que estarán en la posición declarada por las variables
  }
}

function cambiarEstado() { // Se activa la función para cambiar el estado
  estado = estado + 1; // Se asigna que el estado es igual a estado + 1
  if (estado > 2) estado = 0; // Se crea la condicional que dice que si estado es mayor a 2, el estado vuelve a 0
  
  if (estado === 1) { // Se crea una condicional que dice que si estado es igual a 1, ocurrirá lo siguiente
    imagY = height; // Se le asigna el valor a imagY que será igual al alto del canvas
    animando = true; // Se le asigna el valor a la animación que será true (O sea que se ejecuta)
    visible = false; // Se le asigna el valor a visible, que será false (Que no se muestra)
    estColor.stop(); // Se agregan los sonidos y se reproduce en loop el de "est" y se le configura el sonido al audio de "john"
    john.stop();
    est.loop();
    john.setVolume(1.0);
  }
  if (estado === 2) { // Se crea una condicional que dice que si el estado es igual a 2, ocurrirá lo siguiente
    est.stop(); // los sonidos estarán apagados
    estColor.stop();
  if (estadoBoton === 2) // Se crea una condicional que dice que si el estado es igual a 2 ocurrirá lo siguiente
    john.setVolume(0.15) // Se configura el volumen al sonido y se baja a 0.15
  }
  if (estado === 0){ // Se crea una condicional que dice que si el estado es igual a 0, ovurrirá lo siguiente
  est.stop(); // Se apagarán todos los sonidos
  estColor.stop();
  john.stop();
  }
}

function windowResized() { // Se activa la función Window Resized con los valores antes asignados
  let anchoPantalla = min(windowWidth, (windowHeight * 16) / 9); 
  let altoPantalla = (anchoPantalla * 9) / 16; 
  resizeCanvas(anchoPantalla, altoPantalla); 
  botonSiguiente.position(width / 2 - botonSiguiente.size().width / 2, height * 0.9);


}
function mousePressed() { // Se activa la función mouse pressed
  let posXBoton = width * 0.605; // Se crea la variable posXBoton para los botones que manejarán los canales, y estos se posicionan en el 60.5% de X del canvas
  let posYBoton1 = height * 0.246; // Se crea la variable posYBoton1 que irá en el 24.6% de Y del canvas
  let tamBoton = width * 0.03; // Se crea la variable tamBoton y se le asigna un tamaño de 0.03% del canvas
  let distancia = dist(mouseX, mouseY, posXBoton, posYBoton1); // Se declara la variable distancia, que será igual a dist(calcula la distancia entre dos puntos) por lo que calcula la distancia en la posición actual del mouse y la posición del botón

  if (distancia < tamBoton && estado === 1) { // Se crea una condicional que dice que si la distancia es mayor al tamaño del botón ocurrirá lo siguiente 
    estadoBoton = estadoBoton + 1; // El estado de botón es igual a estado de botón + 1
      
  if (estadoBoton > 2) { // Se crea una condicional que dice que si el estado de botón es mayor a 2, este volverá a 0
     estadoBoton = 0;
  }
  est.stop(); // Se agregan los audios y se apagan antes de iniciar 
  estColor.stop();
  john.stop();

  if (estadoBoton === 0) { // Se crea una condicional que si el estadoBoton es igual a 0 ocurrrirá lo siguiente
  est.loop(); // Se reproduce el sonido Est en loop
  } else if (estadoBoton === 1){ // Se crea una condicional que si el estadoBoton es igual a 1 ocurrrirá lo siguiente
  estColor.loop(); // Se reproduce el EstColor en loop
  } else if (estadoBoton === 2){ // Se crea una condicional que si el estadoBoton es igual a 2 ocurrrirá lo siguiente
  john.loop(); // Se reproduce el john en loop
  john.setVolume(2.0); // Se le ajusta el volumen al audio que será de 2
    }  
    }
}     
 ```  


## [Sketch p5.js](https://editor.p5js.org/kitcaaatt/sketches/68mtF3yJG)  
