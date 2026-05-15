# Apuntes-P5-Dibujo-geom-trico-27-03

## *Conseguir apuntes previos

## Color en P5  
Usar páginas en RGB  
&#8594; [color codes](https://htmlcolorcodes.com/)  
&#8594; [sharp color picker](https://colorpicker.net/)

Cambio de colores con comando **colorMode/(HSB)**

## Donde pongo el background en el setuo/() o el draw/()  
&#8594; Si quieren un color limpio de fondo, debe estar en el draw  
&#8594; Si quieren que deje una estela encima del lienzo, debe estar en el setup

### Dibujar en P5.js  
El canvas funciona con un sistema de coordenadas /(X,Y) como un plano cartesiano, sino que el punto /(0,0) esta en la esquina superior izquierda.

### Figuras geométricas 2D
* Point/(x,y) 
* Stroke Usado para bordes-líneas en valores RGB
    * Strokeweight Usado para asignar el tamaño de ese borde
* Line(x1,y1,x2,y2)
* Rect(x1,y1,x2,y2)
   * Fill(valores en RGB)
* Ellipse(x,y1, alto, ancho)
* Circle(x,y,radio)
* square(x,y,lado) cuadrado perfecto
* triangle(x1,y1,x2,y2,x3,y3) triangulo y cada vertice se pone en la manesilla del reloj
* quad(x1,y1,x2,y2,x3,y3,x4,y4) cuadrilatero irregular cada vertice en las manesillas del reloj

### Figuras geométricas AVANZADAS
* angleMode(Degrees)
   * arc(x,y,diametro inicial,diametro final,start,stop)
   * Los grados parten a las 15hrs en el sentido del reloj y siguen sentido horario en negativo.
 
### Forma del borde / línea

strokeCap();  
Define la forma de la línea o borde de nuestras figuras
&#8594; ROUND  
&#8594; SQUARE  

### Desafíos

Canvas de 500
