# sesión 03 - 27/03
P5.js/encargo solemne01
--  

ALGORITMO
--
Es una secuencia instrucciones paso a paso,
lógicas, definidas, ordenadas y finitas que
permiten solucionar un problema o realizar
una tarea específica.  

* Características
*  Precisión: Cada paso debe estar clarísimo (sin ambigüedades).
*  Finitud: Tiene que terminar en algún momento; no puede ser infinito.
*  Definición: Si sigues el mismo algoritmo dos veces con los mismos datos,
   deberías obtener siempre el mismo resultado.

estructura: input- la info para empezar/ Proceso- Los pasos lógicos que transforman esa entrada. (algoritmo)/ output- resultado o solución al problema

DIAGRAMA DE FLUJO
--
Representación gráfica de un algoritmo o de los
pasos de un proceso. En programación, se utiliza
como una herramienta de planificación para
visualizar la lógica de un programa antes de
escribir una sola línea de código.  
* Se usan componentes Estándar (Simbología), para
  que cualquier programador pueda entenderlo.

  P5.js
  --
  
p5.js no es un lenguaje nuevo desde cero,
sino una biblioteca (library) de
JavaScript. Esto significa que usa toda la
potencia y la sintaxis de JavaScript, pero
te regala un "vocabulario" especializado
para dibujar, animar y crear cosas visuales
de forma mucho más sencilla.

setup(): Se ejecuta una sola vez al principio
(para crear el lienzo).

propósito: Configurar el entorno inicial.

Qué sucede: Defines el tamaño del lienzo
(createCanvas), cargas imágenes o sonidos, y
estableces configuraciones que no cambiarán
(como el color de fondo inicial).

draw(): Se ejecuta en un bucle infinito
(normalmente 60 veces por segundo), lo que
permite crear animaciones.

propósito: Crear movimiento y responder a la
interacción en tiempo real.

Qué sucede: Dibujas formas que cambian
de posición, detectas dónde está el ratón o
cambias colores gradualmente.  

* laplataforma usa un sistema de cordenadas para dibujar XyY conel punto 0 en la esquina superior izquierda.

COMO SE HACEN LAS FIGURAS:
* point(x, y); Dibuja un solo píxel en las coordenadas dadas.
* line(x1, y1, x2, y2); Dibuja una línea desde un punto inicial hasta un punto final.
* rect(x, y, ancho, alto); Dibuja un rectángulo. Por defecto, x e y definen la esquina superior izquierda.
* ellipse(x, y, ancho, alto); Dibuja un óvalo o círculo. A diferencia del rectángulo, x e y definen el centro de la figura.
* circle(x, y, diámetro); Una versión simplificada de la elipse cuando quieres un círculo perfecto.
* square(x, y, lado); Un rectángulo donde todos los lados son iguales.
* triangle(x1, y1, x2, y2, x3, y3); Necesitas darle las coordenadas de sus tres esquinas.
* quad(x1, y1, x2, y2, x3, y3, x4, y4); Un cuadrilátero. Sirve para hacer formas irregulares de cuatro lados.


SOLEMNE 1: CREAR UN DIBUJO INSPIRADO EN UNA PINTURA DE ARTE ABSTRACTO:
mi referente: Hilma Af Klint, Svanen nr 17  
![svanen, nr 17](https://artequinvina.cl/wp-content/uploads/2024/11/Hilma_af_Klint_Svanen.jpg)

version 1 de mi dibujo: ![dibujo geométrico ](https://github.com/user-attachments/assets/9ee6a81a-9e5e-4f53-ba34-6ca2efc28a9c)




