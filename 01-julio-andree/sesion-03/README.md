# Apuntes - 27/03  
### Presentación de P5js  
Funtionsetup: Se ejecuta al principio solo una vez, configura el entorno principal que no va a cambiar.  
FuntionDraw: Se ejecuta en un cicli infinito a 60 fps, aquí se permite crear.  
### Codigos:  
createCanvas: creación de lienzo poder ajustar su tamaño en pixeles. cuenta con más variables de configuración (ancho,alto,render,canvas) Render: Poder cambiar de 2d a 3d. Canvas: Para diseño web. este codigo siempre va dentro del setup.  
background: Color de fondo (R,G,B,[alpha]) Alpha se refiere a transparencia de color. Para color limpio de fondo escribe backgraund en Draw y para mantener el color toda la función escribir en setup.  
**Estos codigos van siempre por encima de la figura**  
stroke: color de borde (R,G,B,[alpha]).  
strokeWeight: Tamaño del borde.  
fill: color de relleno (R,G,B).  
strokeCap: para mejorar borde de la figura arco.  
  
##Figuras geométricas  
point: Pinta un pixel en las coordenadas dadas (x,y)  
line: Dibuja linea desde punto inicial a punto final (x,y,x2,y2)  
rect: Dibuja un rectangulo, x e y definen la esquina superior izquierda (x,y,ancho,alto)  
ellipse: Dibuja un óvalo o circulo, x e y definen el centro de la figura (x,y,ancho,alto)  
circle: Para circulo perfecto (x,y,diámetro)  
square: Rectángulo donde todos los lados son iguales (x,y,tamaño pixel por pixel)  
triangle: Dibuja tiangulo, definir coordenadas de sus tres esquinas (x,y,x2,y2,x3,y3)  
squad: Dibuja cuadrilátero, Formas irregulares de cuatro coordenadas (x,y,x2,y2,x3,y3,x4,y4)

### Arco  
angleMode(DEGREES): Escribir en setup para trabajar con arcos.  
arc: Dibuja arcos (x,y,ancho,alto,inicio,termino) Inicio y termino se refiere donde cominza y termina el angulo. El angulo 0 comienza a la izquierda del circulo y gira a las manillas del reloj.  
Imagen descriptiva:
