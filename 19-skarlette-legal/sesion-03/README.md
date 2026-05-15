# sesión 03 - 27/03

# p5.js  

##  ¿Qué es un algoritmo?

Un **algoritmo** es un conjunto de instrucciones ordenadas que permiten resolver un problema o realizar una tarea.

###  Características 

- **Precisión:** Cada paso debe ser claro y sin ambigüedades.  
- **Orden:** Las instrucciones siguen una secuencia lógica.  
- **Finitud:** Debe terminar en algún momento.  
- **Definición:** Con los mismos datos de entrada, siempre produce el mismo resultado.  

---

##  Estructura 

Todo algoritmo se compone de:

- **Input (Entrada):** Datos o información inicial.  
- **Proceso:** Pasos que transforman la entrada.  
- **Output (Salida):** Resultado final.  

###  Ejemplo (Sandwich)

- **Input:** Ingredientes y utensilios  
- **Proceso:** Lista de pasos para prepararlo  
- **Output:** Sandwich terminado  

---

##  Diagrama de flujo

Representación gráfica de un algoritmo.

- Permite **visualizar la lógica** antes de programar  
- Utiliza **simbología estándar**  
- Facilita la comprensión entre programadores  

---

##  Lenguajes de programación

- Existen más de **8.000 lenguajes** en la historia  
- Actualmente se usan entre **700 y 900**  

###  Categorías principales

| Categoría              | Ejemplos                  |
|----------------------|--------------------------|
| Propósito general     | Python, Java, C++, C#    |
| Desarrollo web        | JavaScript, TypeScript, PHP, Ruby |
| Bajo nivel / sistemas | C, Rust, Go              |
| Análisis de datos     | R, Python, Julia         |
| Desarrollo móvil      | Swift, Kotlin            |

---

##  p5.js

p5.js es una **biblioteca de JavaScript**, no un lenguaje nuevo.

##  Funciones principales

### `setup()`

- Se ejecuta **una sola vez**  
- Configura el entorno inicial  

##  Función `draw()`

La función `draw()` es una de las más importantes en p5.js.

- Se ejecuta en un **bucle infinito** (aprox. 60 veces por segundo).
- Permite crear **animaciones** e **interacción en tiempo real**.

function draw() {
  background(220);
  circle(mouseX, mouseY, 50);
}

##  Función `createCanvas()`

### Definición
La función `createCanvas()` se utiliza para crear el lienzo de trabajo (canvas) en p5.js, definiendo sus dimensiones y, opcionalmente, el modo de renderizado.

### Ejemplo
createCanvas(100, 100);


##  Función `background()`
background(v1, v2, v3, [a]);


### Parámetros
* **v1, v2, v3:**
  Corresponden a los valores del modelo de color RGB:

  * R (Red): 0–255
  * G (Green): 0–255
  * B (Blue): 0–255

* **a (alpha, opcional):**
  Controla la transparencia:

  * 0 → completamente transparente
  * 255 → completamente opaco


### Ejemplo
background(250, 150, 228, 150);


### Consideraciones de uso

* Si se utiliza en `setup()`, el fondo se dibuja una sola vez.
* Si se utiliza en `draw()`, el fondo se actualiza en cada frame, eliminando cualquier rastro previo.


### Formas de uso

* **Escala de grises:**

javascript
background(220);


* **Color RGB:**

background(255, 0, 0);


* **Nombre de color:**
background('blue');


* **Con transparencia:**
background(0, 0, 255, 50);

## Modos de color

### Modelo RGB (por defecto)

El modelo RGB representa los colores mediante la combinación de tres canales:

* R (Red): 0–255
* G (Green): 0–255
* B (Blue): 0–255

colorMode(RGB)


---

### Modelo HSB / HSV

Este modelo representa el color de forma más perceptual:

* H (Hue / tono): 0°–360°
* S (Saturation): 0%–100%
* B (Brightness): 0%–100%
colorMode(HSB);


---

### Modelo HSL

Similar a HSB, pero utiliza luminosidad en lugar de brillo:

* H (Hue): 0°–360°
* S (Saturation): 0%–100%
* L (Lightness): 0%–100%
colorMode(HSL);

## { FIGURAS GEOMÉTRICAS 2D}

* **point(x, y);** Dibuja un solo píxel en las coordenadas dadas.
 
* **line(x1, y1, x2, y2);** Dibuja una línea desde un punto inicial hasta un punto final.
  
* **rect(x, y, ancho, alto);** Dibuja un rectángulo. Por defecto, x e y definen la esquina superior izquierda.
  
* **ellipse(x, y, ancho, alto);** Dibuja un óvalo o círculo. A diferencia del rectángulo, x e y definen el centro de la figura.
  
* **circle(x, y, diámetro);** Una versión simplificada de la elipse cuando quieres un círculo perfecto.
  
* **square(x, y, lado);** Un rectángulo donde todos los lados son iguales.
  
* **triangle(x1, y1, x2, y2, x3, y3);** Necesitas darle las coordenadas de sus tres esquinas.
  
* **quad(x1, y1, x2, y2, x3, y3, x4, y4);** Un cuadrilátero. Sirve para hacer formas irregulares de cuatro lados.


---

##  TAMAÑO DEL BORDE 
 strokeWeight(weight);

*Ejemplo:*

strokeWeight();
Establece el tamaño del borde
de las figuras o el ancho de la
linea o punto.

Siempre se pone arriba de
Stroke();

strokeWeight(25);

**noStroke();** para quitar el borde.

###  COLOR DEL BORDE 
 stroke(v1, v2, v3, [alpha]);

##  FORMA DEL BORDE / LINEA 
strokeCap(cap);

**Las constantes son:
ROUND
SQUARE
PROJECT**

Por defecto siempre es ROUND  

## RELLENO DE COLOR 
fill(v1, v2, v3, [alpha]);
fill();
Establece el COLOR de relleno
para las figuras.


## DESAFIO 1 + DESAFIO 2


 # SOLEMNE 1

 Recreae el dibujo que realizamos en formato 500x500 pixeles.


