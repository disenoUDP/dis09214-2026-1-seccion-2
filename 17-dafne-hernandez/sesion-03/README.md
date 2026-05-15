# Aprender a utilizar p5.js

**Antes de ponerse a codificar se debe hacer un diagrama de flujo**

Que es una representación gráfica de un algoritmo o de los pasos de un proceso. En programacion se utiliza como una herramienta de planificación para visualizar la lógica de un programa antes de escribir una sola linea de código

 - Se usan componentes estandar, simbologia, para que cualquier programador pueda entenderlo.

*Ej: La lampara no funciona -> preguntas: De si o no  
Si no -> Respuesta  
Si si -> otra pregunta -> respuesta  
Si no -> Respuesta  
Van desde arriba hacia abajo, y siempre tendrá la misma simbologia.*  

**Lenguajes de programacion:**  
| *Categoría* | *Ejemplos comunes* |
| :--- | :--- |
| **Propósito General** | Python, Java, C++, C# |
| **Desarrollo Web** | JavaScript, TypeScript, PHP, Ruby | 
| **Sistemas y Bajo Nivel** | C, Rust, Go |
| **Análisis de Datos** | R, Python, Julia |
| **Móvil** | Swift (iOS), Kotlin (Android) |

### ***El lenguaje de programación utiliza principalmente el lenguaje de JavaScript***

- p5 no es un lenguaje nuevo desde cero, si no, una biblioteca de JavaScript.

## **Funciones maestras**
- ***SETUP:***  se ejecuta una sola vez al principio (Para crear el lienzo)  
**Su próposito:** Configurar el enterno inicial.  
**Qué sucede:** Defines el tamaño del lienzo (Createcanva) cargas imágenes o sonidos y estableces configuraciones que no cambiarán (Cómo el color del fondo inicial).

- ***DRAW:*** Se ejecuta en un bucle inifinito, (Normalmente 60 veces por segundo) Lo que permite crear animaciones.  
**Su próposito:** Crear movimiento y responder a la interacción en tiempo real.  
**Qué sucede:** Dibujas formas que cambian de posición, detectas dónde está el ratón o cambias colores gradualmente.

- ***createCanvas*** Es la linea de código que se utiliza para crear el lienzo y determinar su tamaño.  
(createCanvas) : Sintaxis ```createCanvas([width],[heigth]);```  
###### El render configura el programa en 2D predeterminado (Si es que no se configura) pero si es que se quiere cambiar a 3D, se debe activar WEBGL, es indispensable para funciones como box, Sphere, luces o texturas complejas.  Canvas: es el parametro oculto menos utilizado pero útil si es que eres desarrollador Web.  

- ***Background:***  
Sintaxis ```Background(v1,v2,v3,[a]);``` : v1,v2,v3 son los valores de RGB  
El background sirve para designar el color de nuestro lienzo.  
4to parametro es el [a] es el canal alpha, si es que yo quiero que mi color sea transparente o semi transparente.

## Dibujar en p5.js  

Para dibujar en p5.js se debe entender que el *Canvas* funciona con un **Sistema de Coordenadas (x,y)** como el de un plano cartesiano, por lo que hay que tener en cuenta que el punto (0,0) no está en el centro, sino en la esquina superior izquierda.  

## FIGURAS GEOMÉTRICAS 2D  

- ```point(x,y);```: Dibuja un solo pixel en las coordenadas dadas.
- ```line(x1,y1,x2,y2);```: Dibuja una línea desde un punto inicial hasta un punto final.
- ```rect(x,y,ancho,alto);```:Dibuja un rectángulo. (x e y definen la ***esquina superior izquierda***).
- ```ellipse(x,y,ancho,alto);```: Dibuja un óvalo o círculo. (x e y definen el ***centro*** de la figura).
- ```circle(x,y,diámetro);```: Una versión simplificada del elipse cuando se quiere un circulo perfecto.
- ```square(x,y,lado);```: Un rectángulo (Cuadrado) donde todos los lados son iguales.
- ```triangle(x1,y2,x2,y2,x3,y3);```: Un triangulo, se necesita darle las coordenadas a sus tres esquinas.
- ```quad(x1,y1,x2,y2,x3,y3,x4,y4);```: Un cuadrilátero, sirve para hacer formas irregulares de cuatro lados.

##### Figura 2D Avanzada  
- ```arc(x,y,w,h,start,stop);```: Sirve para hacer arcos o medio circulo, *x e y* son las coordenadas del centro, *w y h* son ancho y alto, *start y stop*, es dónde comienza y termina el ángulo del arco.  
**Se sugiere agregar el modo** ```angleMode(DEGREES);``` Para los ángulos.
  en p5.js (y en la mayoría de leng. de programación) el **Grado 0** no está arriba, sino a la **derecha** y se mueve en el sentido del reloj.  

### Tamaño y color del borde  

- ```strokeWeigth(weigth);``` : Establece el tamaño al borde de las figuras o el ancho de una línea o punto.
- ```noStroke();``` : Se usa para que la figura no tenga borde.
- ```stroke(v1,v2,v3, [alpha]);```: Establece el color que se utiliza para dibujar puntos, lineas y contornos de figuras.

### Relleno de color  
- ```fill(v1,v2,v3, [alpha]);```: Establece el color del relleno para las figuras.

![Gato](https://i.pinimg.com/736x/58/b9/aa/58b9aac1da7597fa40825282bc9d3cf7.jpg)

 
