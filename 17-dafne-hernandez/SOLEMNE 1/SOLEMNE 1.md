# SOLEMNE 1  

Crear dibujo en p5 usando de referente a un artista abstracto.  
**Referente**: Sonia Delaunay y Theo Van Doesburg.  
- **Obras a inspiración**:
- 
  - Rythme Couleur, 1955.
![https://auroraathena.com/app/uploads/2025/02/Sonia-Delaunay-Rythme-Couleur-1955-Front-Without-Frame-1.jpg](https://auroraathena.com/app/uploads/2025/02/Sonia-Delaunay-Rythme-Couleur-1955-Front-Without-Frame-1.jpg)  
  - Grand Helice Rouge, 1970.   
 ![https://www.frestoniangallery.com/artworks/145-sonia-delaunay-grand-helice-rouge-1970/](https://static-assets.artlogic.net/w_2400,h_2400,c_limit,f_auto,fl_lossy,q_auto/artlogicstorage/rcfa/images/view/b338af090c1362c7721174cbe48b0bded0d626f3/frestoniangallery-sonia-delaunay-grand-helice-rouge-1970.jpg)
  - Dance, 1917.
  
 ![https://uploads5.wikiart.org/images/theo-van-doesburg/dance-i.jpg!Large.jpg](https://uploads5.wikiart.org/images/theo-van-doesburg/dance-i.jpg!Large.jpg)  

Me inspiré en base de estas tres obras para crear el mío, utilicé los tipos de figuras que se encuentran en las distintas obras, y lo combiné con los colores brillantes que caracterizaban los trabajos de Sonia Delaunay; Apesar de que las figuras que se encuentran en mi trabajo no están compactas y unidas todas entre sí, por más de que las obras tengan esa caracteristica, decidí reinterpretarlas para crear algo que se acoplara a mí idea inicial. Encontré dificultades en la composición de lo que quería plasmar, pero luego de unos intentos logré hacer una compo final con la que me quedé bastante satisfecha.  

y con ello al momento de traspasarlo a p5.js se presentaron las dificultades más evidentes que era el tema de las coordenadas, pero con el pasar del tiempo se fué haciendo aún más fácil hasta lograr hacerlo sin pensar tanto, la única figura con la que se presenta dificultad es el arco, pero depende más que nada de los ángulos que necesita. 

## CÓDIGO P5.JS  

function setup() {  
  createCanvas(500, 500);  
  background(255, 227, 250); // Se le agrega un fondo al canvas  
  angleMode(DEGREES);  
}  

function draw() {    
  //background(220);  
  noStroke()  
  fill(196, 0, 0); // Se le agrega relleno de color rojo al Rectangulo   
  rect(30,30,80,170); // Crea un rectangulo en el canvas en las coordenadas 30,30  
  fill(0,0,255); //  Se le agrega relleno de color azul al Triangulo   
  triangle(40,200,110,270,110,200); // Crea un Triangulo en el canvas en las coordenadas 40,200,110,270,110,200  
  fill(196, 0, 0); //  Se le agrega relleno de color rojo al cuadrado  
  square(40,350,80); // Crea un cuadrado en el canvas en las coordenadas 40,350  
  fill(0,0,255); //  Se le agrega relleno de color azul al circulo  
  circle(120,430,40); // Crea un circulo en el canvas en las coordenadas 120,430  
  fill(216, 137, 250); //  Se le agrega relleno de color morado al triangulo  
  triangle(110,295,200,390,200,220); // Crea un triangulo en el canvas en las coordenadas 110,295,200,390,200,220  
  fill(232, 220, 0); //  Se le agrega relleno de color amarillo al arco  
  arc(110,190,190,210,270,90); // Crea un arco en el canvas en las coordenadas 110,190  
  fill(0,255,0); //  Se le agrega relleno de color verde al rectangulo  
  rect(180,40,10,140); // Crea un rectangulo en el canvas en las coordenadas 180,40  
  fill(232, 94, 0); //  Se le agrega relleno de color naranjo al arco  
  arc(110,190,140,160,270,90); // Crea un arco en el canvas en las coordenadas 110,190  
  fill(216, 137, 250); //  Se le agrega relleno de color morado al rectangulo  
  rect(190,40,120,90); // Crea un rectangulo en el canvas en las coordenadas 190,40  
  fill(239, 255, 20); //  Se le agrega relleno de color blanco amarillo  
  circle(255,90,70); // Crea un circulo en el canvas en las coordenadas 255,90  
  fill(196, 0, 0); //  Se le agrega relleno de color rojo al rectangulo  
  rect(250,80,10,70); // Crea un rectangulo en el canvas en las coordenadas 250,80  
  fill(255, 249, 3); // Se le agrega relleno de color arco amarillo  
  arc(290,295,150,150,-47,133); // Crea un arco en el canvas en las coordenadas 290,295  
  fill(120, 247, 52); // Se le agrega relleno de color verde al circulo  
  circle(260,270,50); // Crea un circulo en el canvas en las coordenadas 260,270  
  fill(247, 54, 115); // Se le agrega relleno de color rosa al triangulo y cuadrado  
  square(200,280,50); // Crea un cuadrado en el canvas en las coordenadas 200,280  
  triangle(200,330,200,390,250,330); // Crea un triangulo en el canvas en las coordenadas 200,330,200,390,250,330  
  fill(250, 121, 30); // Se le agrega relleno de color naranjo al triangulo y rectangulo  
  triangle(200,390,250,390,250,330); // Crea un triangulo en el canvas en las coordenadas 200,390,250,390,250,330  
  rect(200,390,50,40); // // Crea un rectangulo en el canvas en las coordenadas 200,390  
  stroke(0,0,0); // Se le agrega color del borde de linea negro  
  strokeWeight(3); //Se le agrega grosor a la linea  
  line(190,400,320,260); // crea una linea en las coordenadadas 190,400,320,260  
  noStroke() // Se activa quitar los bordes  
  fill(88, 17, 130); // Se le agrega relleno de color morado al arco  
  arc(290,295,90,90,-47, 133); // Crea un arco en el canvas en las coordenadas 290,295  
  fill(242, 0, 153); // Se le agrega relleno de color rosa al rectangulo  
  rect(260,130,80,70); // Crea un rectangulo en el canvas en las coordenadas 260,130  
  fill(121, 255, 48); // Se le agrega relleno de color verde al rectangulo  
  rect(310,70,90,60); // Crea un rectangulo en el canvas en las coordenadas 310,70  
  fill(0,0,255); // Se le agrega relleno de color azul al rectangulo  
  rect(430,160,10,220); // Crea un rectangulo en el canvas en las coordenadas 430,160  
  fill(88, 186, 34); // Se le agrega relleno de color verde al triangulo  
  triangle(400,150,340,240,470,240); // Crea un triangulo en el canvas en las coordenadas 400,150,340,240,470,240  
  fill(196, 0, 0); // Se le agrega relleno de color rojo al triangulo y rectangulo  
  triangle(400,70,400,130,340,130); // Crea un triangulo en el canvas en las coordenadas 400,70,400,130,340,130  
  rect(340,130,60,40); // Crea un rectangulo en el canvas en las coordenadas 340,130  
  fill(0,0,0); //Se le agrega relleno de color negro al rectangulo  
  rect(380,400,110,50); // Crea un rectangulo en el canvas en las coordenadas 380,400  
  fill(196, 0, 0); // Se le agrega relleno de color rojo al rectangulo  
  rect(380,350,110,50); // Crea un rectangulo en el canvas en las coordenadas 380,350    
  fill(208, 52, 247); // Se le agrega relleno de color magenta al rectangulo    
  rect(380,310,110,40); // Crea un rectangulo en el canvas en las coordenadas 380,310   
  fill(232, 220, 0); // Se le agrega relleno de color amarillo al arco  
  arc(435,400,70,70,0,180); // Crea un arco en el canvas en las coordenadas 435,400  
  fill(250, 121, 30); // Se le agrega relleno de color naranjo al circulo  
  circle(435,395,50); // Crea un circulo en el canvas en las coordenadas 435,395  
  fill(0,0,255); // Se le agrega relleno de color azul al arco  
  arc(360,215,125,125,-227, -47); // Crea un arco en el canvas en las coordenadas 360,215  
  fill(0,0,0); // Se le agrega relleno de color negro al circulo y al texto  
  circle(400,120,45); // Crea un circulo en el canvas en las coordenadas 400,120  
  textSize(12) // Se le agrega tamaño al texto  
  textFont('Helvetica') // Se le cambia la tipografía al texto  
  text("Dafne Hernández",390,490); // se crea un texto en las coordenadas 390,490  

}  
### [p5.js](https://editor.p5js.org/kitcaaatt/sketches/3Jrq2LqaJ)  

 ### Trabajo final en p5.js  
 
 <img width="1000" height="1000" alt="image" src="https://github.com/user-attachments/assets/4978c2f7-1b97-4a2f-8158-c7b1d8272741" />


### Versión en cuadricula de 32x32  

<img width="371" height="364" alt="image" src="https://github.com/user-attachments/assets/ff92ec4a-8249-4d7b-9649-4b2c58990924" />  







