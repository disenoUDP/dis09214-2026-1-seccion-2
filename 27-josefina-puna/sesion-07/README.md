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

