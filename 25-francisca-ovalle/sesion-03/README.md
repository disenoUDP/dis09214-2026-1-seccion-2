# Sesión 03 - 27/03 Apuntes  
---
## ¿Qué es un algoritmo?
*Secuencia paso a paso*, logicas, intrucciones, ordenadas y finitas.
Caracteristicas principales:  
Precisión, orden, finito y definición

#### ESTRUCTURA:
**Inpud o entrada**: ingredientes para empezar  
**Algoritmo**: Lista de instruccionjes  
**Output**: Resultado final o solución del problema

**Diagrama de flujo**: *Representación gráfica del algoritmo* o de los pasos del proceso. En programación se usa
como herramienta de planificación para visualizar la logica de un programa antes de escribir una sola línea
de codigo.

**Lenguaje de programación**: existen entre 700 y 900 lenguajes que se utilizan actualmente en la industria y en el desarrollo
de software profesional
Python y Java son los más utilizados.

**P5.js**: Utiliza principalmente el lenguaje de **JavaScript.**
No es un lenguaje nuevo si no como una biblioteca de JavaScript.  

---
#### FUNCIONES MAESTRAS EN P5.JS

**setup(){**: se ejecuta solo al inicio, *configura el entorno incial*, define tamaño de lienzo (createcanvas)
carga imagenes y sonidos y establece configuraciones que no cambiarán.

**draw(){**: se ejecuta en blucle infinito lo que *permite crear animaciones*. 

Se puede escribir arriba de los función: 
**{createCanvas}** *Siempre dentro de septup*
Sintaxis: createCanvas([width], [height],[renderer],[canvas];
Ejemplo: createCanvas(100,100);

Optativo:  
**[renderer]** Es el modo "2D" el que usas por *defecto si no escribes nada*, optimizas formas basicas, textos e imagenes planas.  
**[canvas]** Es parámetro oculto y menos utilizado pero útil si eres diseñador.  

**{background}** Para designar el color de nuestro {canvas}**(se puede poner en setup o draw pero tienen resultados diferentes)**.
Sintaxis: background(v1,v2,v3,[a]);  
Ejemplo: background(250, 150, 220, 40);  
**[a]** *Es para dar semitransparencia al color 0-225.*  
**Escala de grises**: 0 es negro y 255 blanco
**Color RGB** (3 números): (Rojo, verde, azul)
**También se puede colocar el nombre del color** ('blue'); (siempre entre comillas).
**Transparencia** (4 números): (RGB y el cuarto es a)  

**colorMode(RGB)**  
R RED G GREEN B BLUE  
**colorMode(HSB)**  
H HUE S SATURATION B BRIGHTNESS  
**colorMode(HSL)**  
H HUE S SATURATION L LIGHTNESS  

#### DIBUJAR EN P5.js  
Funciona con un sistema de coordenadas (x,y), como un plano cartesiano solo que en este caso el 0,0 está en laesquina izquierda superior.
##### PLANO DE COORDENADAS:
![Plano](https://archive.p5js.org/assets/learn/coordinate-system-and-shapes/images/drawing-03.svg)  

---
#### FIGURAS GEOMÉTRICAS 2D:  
**point(x,y)** Dibuja un px en las coordenadas dadas<br>
**line(x1,y1,x2,y2)** Dibuja un línea desde el punto incial hasta el final<br>
**rect(x,y,ancho,alto)** Dibuja un rectángulo, por defecto, x, y definen la esquina superior izquierda<br>
**ellipse(x,y, ancho, alto)** Dibuja un óvalo o círculo, x,y definen el centro del ellipse<br>
**circle(x,y, diametro)** Para hacer un circulo perfecto<br>
**square(x,y, lado)** Dibuja un cuadrado<br>
**triangle(x1,y1,x2,y2,x3,y3)** x, y definen cada coordenada de cada esquina
**quad(x1,y1,x2,y2,x3,y3,x4,y4)** Dibuja un cuadrilátero, sirve para hacer formas irregulares de cuatro lados.  
#### TAMAÑO DEL BORDE:  
**strokeWeight();** Establece el tamaño del borde o el ancho de un punto o línea<br>
Sintaxis: strakeWeight(weight);<br>
Ejemplo: strokeWeight(25);  
**noStroke();** Se usa para que la fig no tenga borde  
#### COLOR DEL BORDE:
**stroke();** Establece el color que se utiliza para dibujar puntos, líneas y contornos de fig.<br>
Sintaxis: stroke(v1,v2,v3, [alpha])<br>
Ejemplo: stroke(245,0,0)  
#### FORMA DEL BORDE/LÍNEA:  
**strokeCap();** Define la forma de la línea o borde de nuestras fig.<br>
Las constantes son: **ROUND**, **SQUARE**, **PROYECT**<br>
Sintaxis: strokeCap(cap);<br>
Ejemplo: strokeCap(SQUARE);  
#### RELLENO DE COLOR:  
**fill();** Establece el COLOR de relleno para las figuras (Se pone arriba de las figuras que quieres colorear).<br>
Sintaxis: fill(v1,v2,v3,[alpha]);<br>
Ejemplo: fill(210,40,160);  
#### FIGURAS GEOMÉTRICAS 2D AVANZADAS:  
**arc();** Sirve para hacer arcos o medios círculos, x,y es el centro del circulo, w y h es la anchura y altura y star y stop es donde comienza
y termina *(guiandose por el sentido del reloj y los grados)*.<br>
Sintaxis: arc(x,y,w,h,start, stop)<br>
Ejemplo: arc(250,250,100,100,270,90);<br>
**SE SUGIERE ACTIVAR EL MODO ÁNGULO EN SETUP**
**angleMode(DEGREES);**  
##### GRADOS:  
![GRADOS](https://thumbs.dreamstime.com/b/c%C3%ADrculo-con-los-grados-marcados-74654200.jpg)



