# sesión 06 - 14/04

# Loops  while y for  
## Loop  
* Bucle *   
Rizo de cabello en forma helicoidal  
Estructura de control que permita ejecutar un bloque de instrucciones de manera repetida mientras se cumple una condición especifica o hasta que se alcance un estado determinado.  

### while  
Bucles para repetir instrucciones mientras una instrucción sea verdadera (como sentencias if que se repite)  
while(condición booleana) [  
si es true ejecuta este código en BUCLE]  
```  
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(127, 233, 139);

  let y = 0;

  while (y <= 400) {
    stroke(139, 127, 233);
    strokeWeight(5);
    line(0, y, 400, y);
    y = y + 25;
  }

  let x = 0;

  while (x <= 400) {
    stroke(233, 127, 168);
    strokeWeight(5);
    line(x, 0, x, 400);
    x = x + 25;
  }
}
```
### for  
Los bucles `for` son útiles para repetir instrucciones un número determinado de veces.  
Son una especie de SHORTCUT para hacer loops y siempre tienen 4 elementos:  

1. Inicialización de una variable  
2. Condición booleana (V-F)  
3. Actualización ( Incrementación o decrementación)  
4. Lo que queremos que pasé cuando la condición sea TRUE

for(inicializacion variable;condiciíon booleana;actualizacion){  
Lo que queremos que pase cuando la condición sea verdadera}  

```
function setup() {
  createCanvas(400, 400);
  frameRate(10);
}

function draw() {
  background(127, 221, 233);

  /*
  let x=0;

  while(x < width){ 
    fill(233,127,168);
    ellipse(x,200,50);
    x=x+30;
  }
  */

  //for (let x = 0; x < width; x = x + 30) {
   // fill(random(255), random(255), random(255));
    //ellipse(x, 200, random(100));
  //}
  
  for (let y = 0 ; y < width; y = y + 30) {
    fill(random(225), random(225), random(225));
    ellipse(200, y, random(100));
  }
}
```
### nested loop  
Es un for dentro de otro for  
for (inicialización variable; condición booleana; actualización){  

Lo que queremos que pase cuando la condición sea verdadera  

for (inicialización variable; condición booleana; actualización){  
}  
Lo que queremos que pase cuando la condición sea verdadera  
}  
```
function setup() {
  createCanvas(400, 400);
  frameRate(24);
}

function draw() {
  background(0);

  for (let x = 0; x <= width; x = x + 25) {
    for (let y = 0; y <= height; y = y + 25) {
      fill(random(225), random(225), random(mouseY));
      ellipse(x, y, 15);
    }
  }
}

// Agregar valores Random en color y ellipse para movimiento 
// Agregar mouseX y mouseY  
```

```
function setup() {
  createCanvas(400, 400);
  noLoop(); // Solo dibuja una vez al inicio
}

function draw() {
  background(255);
  
  let size = 50; // Variable para el tamaño de cada cuadrado de la cuadrícula
  
  for (let x = 0; x < width; x = x+size) {
    for (let y = 0; y < height; y += size) {
      fill(random(255), random(255), random(255));
      rect(x, y, size, size);
    }
  }
}

function mousePressed() {
  // Cambia los colores cada vez que hago clic
  redraw();
}
```
