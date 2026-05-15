# sesión 03 - 27/03

### Algoritmo: Secuencia de instrucciones paso a paso, lógicas.
 * Cada paso debe estar clarisimo.
 * Los pasos deben tener lógica.

### Estructura:
1. Imput: Información para empezar.
2. Algoritmo: Instrucciones (transforman la entrada).
3. Output: Solución del problema.

### Diagrama de flujo:
Representacion gráfica de un algoritmo o de pasos del proceso (visualizar la lógica).  
Componentes estandar para que cualquier programador pueda entenderlo.

### Lenguaje de programación  
Proposito general: Python, Java, Cet, c#.  
Desarrollo Web : Javascript.  

### P5.js  
Utiliza principalmene el lenguaje Javascript.  
No es un lenguaje nuevo desde cero, sino una biblioteca.  

### setup(){   
Se ejecua una sola vez.  
Proposito: Configurar el entorno inicial.  
Que sucede: Defines el tamaño del lienzo, cargas imagenes o sonidos, y estableces configuraciones que no cambiarán.  

### draw(){   
Se ejecuta en un bucle infinito.  
Proposito: Crear movimiento y respnder a la interaccion en tiempo real.  
Que sucede: Dibujas formas que cambian de posición.  

### createCanvas (width, height)  
Para crear el lianzo y determinar su tamaño en pixeles (solo se pone una vez y siempre dentro del setup().  

### background (v1,v2,v3,[a]);  
Para designar el color de nuestro lienzo (en valores RGB), se puede poner en el setup u en el draw, el [a] se utiliza para darle semitransparencia al color.  

### Dibujar en P5.js  
El canvas funciona con un sistema de coordenadas (x,y), el punto (0,0) esta en la esquina superior izquierda.  

