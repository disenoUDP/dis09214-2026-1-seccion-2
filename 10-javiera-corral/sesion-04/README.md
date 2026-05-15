# sesión 04 - 10/04
Forks:copia personal del repositorio, crear uno para poder editar bitacora o tareaas sin alterar la rama principal y luego hacer request para que lo actualice la profe o asisstente.
*siempre hacer sink para actualizar el fork 

clase de hoy: VARIABLES 
-
como hacer movimeinto en p5 (variables)

POSICIÓN DEL MOUSE
-
Sintaxis (mouseX, mouseY): Variables de sistema numérico que determinan la posición del mouse en las coordenadas X e Y.

si se desactiva el fondo y se utiliza estos comandos en una figura se puede "pintar" con ella. [ejemplo](https://editor.p5js.org/PoliMujica/sketches/KHG4X-Z6Y) 

 * [variable-and-changep5js](https://p5js.org/tutorials/variables-and-change/)

CREA TUS PROPIAS VARIABLE ⭐ <img width="409" height="345" alt="image" src="https://github.com/user-attachments/assets/846ddd45-d406-40b5-aec5-484a49250951" />

-
1. DECLARAR TU VARIABLE Para declarar una variable podemos usar **let** para variables dinámicas y **const** para variables constantes.
**¡OJO!**
Antiguamente se usaba var en vez de let,
pueden encontrar algunos tutoriales con var.

2. INICIALIZA TU VARIABLE

3. USA TU VARIABLE
   
JAVASCRIPT OBJECT <img width="450" height="338" alt="image" src="https://github.com/user-attachments/assets/0ef60e0b-607b-4163-8a82-527e4320cba6" />

-

Nos servirán para organizar nuestro código de una forma adecuada y ordenada.

Es la forma de agrupar muchas variables dentro de una variable.

Es una estructura de datos que te permite agrupar valores relacionados bajo un mismo nombre. En lugar de tener muchas variables sueltas, los objetos funcionan como un "contenedor" que organiza la información mediante pares de clave y valor.

Luego se accede a la información mediante notación de punto. [ejemplo](https://editor.p5js.org/PoliMujica/sketches/cuJXAPjTm) 

RANDOM FUNCTION
-
Su trabajo es devolver un número aleatorio dentro de un rango que tú definas.

random(): Si no pones nada, devuelve un número decimal entre 0 y 1
Ejemplo: random() da 0.4571.

random(máximo): Devuelve un número decimal entre 0 y el máximo que elijas.

Ejemplo: random(100) da un número entre 0 y 100.

random(mínimo, máximo): Devuelve un número decimal entre esos dos valores.

Ejemplo: random(20, 50) da un número entre 20 y 50.
[ejemplo en p5](https://editor.p5js.org/PoliMujica/sketches/t7x5F6rUt)

(width , height)
-
Variables integradas en p5, que corresponden
a los valores definidos en el createCanvas.

[Ej Sketch](https://editor.p5js.org/PoliMujica/sketches/sh0yWrsdA)

[REFERENCIA WIDTH](https://p5js.org/reference/p5/width/)
[REFERENCIA HEIGHT](https://p5js.org/reference/p5/height/


(windowWidth, windowHeight);
-
Variables integradas en p5, que permiten ajustar el
tamaño del lienzo al tamaño de la ventana del
navegador. Se usan en el createCanvas.

[referencia1](https://p5js.org/reference/p5/windowHeight/)
[referencia2](https://p5js.org/reference/p5/windowWidth/)


MAP FUNCTION
-
Esta función nos permite convertir un valor de un rango a otro. En términos simples: toma un número que está en una "escala" y lo traduce proporcionalmente a una "escala" nueva.

Sintaxis: map(valor, min_original, max_original, min_nuevo, max_nuevo)

valor: La variable que quieres "mapear" (por ejemplo, mouseX).
min_original y max_original: El rango en el que se encuentra ese valor actualmente
min_nuevo y max_nuevo: El rango al que lo quieres transformar.

[referencia map](https://p5js.org/reference/p5/map/) 

DESAFÍO DE LA CLASE: ¡ROMPER LA ESTÁTICA !
-
[dibujo con movimiento⭐](https://editor.p5js.org/StarBerryChiscake/sketches/nZlpO1lLY)

