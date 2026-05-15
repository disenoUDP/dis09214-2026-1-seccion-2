# sesión 05 - 17/04
TRANSFORMACIONES & {If - else}
-
Angulos, angleMode [video info](https://youtu.be/DMg-WRfNB60?si=M7ZQaqsv-Q1tpMuN) <img width="446" height="384" alt="image" src="https://github.com/user-attachments/assets/1283c066-eadc-4de9-81ab-02c628cdb917" /> movimiento como el de las agujas del reloj

Por defecto p5.js usa RADIANES para medir los ángulos.
angleMode(RADIANS)
Para cambiar a grados se usa esto en el fuction SETUP
angleMode(DEGREES) 

ROTACIÓN rotate(); 
-
rotate(valor radianes o en grados); ejemplo: rotate(20); [referencia](https://p5js.org/reference/p5/rotate/)  

  * Sirve para rotar elementos.
  * SIEMPRE ROTA ALREDEDOR DEL PUNTO DE ORIGEN (0,0)
  * Se recomienda usar con translate(); y en algunos casos con rectMode(CENTER);
  * [ejemplo](https://editor.p5js.org/PoliMujica/sketches/XFVDpysTg)

TRASLADAR translate();
-  
  * translate(x,y);
  * Sirve para trasladar el PUNTO DE ORIGEN (0,0) a otra cordenada de mi canvas.
  * [ejemplo](https://editor.p5js.org/PoliMujica/sketches/ddsUf63Oy)

GUARDAR Y RESTAURAR
-
