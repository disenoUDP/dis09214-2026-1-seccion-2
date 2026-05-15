# sesión 07 - 15/05



function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);

  let x=0;

  while(x < width){ //while significa mientras. mientras X sea menor que el width de el canvas 
    fill(233,127,168); // relleno del circulo 
    ellipse(x,200,50);  // se crea un circulo en en x, 200 de tamaño 50
    x=x+30; // pero luego el valor de X amuneta a en 30 cada vez que el loop se repita. tecnicamente el loop de while termina cuando x sea igual o mayor que width 
  }

}



function setup() {
  createCanvas(400, 400);
  noFill();
  strokeWeight(2);
}

function draw() {
  // fondo negro
  background(0); 
  
  // creo variable diametro y le asigno un valor de 400
  let diametro = 400; 

  //loop Mientras el valor de mi varibale diametro sea mayor que 0

    
  while (diametro > 0) {
  // asigna un color al borde alterado por mi varbiale diametro
    stroke(diametro, 100, 255 - diametro / 2);
    
  // crea un circulo en cordenada x, cordenada y, diametro  
    circle(width / 2, height / 2, diametro);
    
  //creamos la variable opArt que será un map de mouseX
    let opArt = map(mouseX, 0, width, 5, 50); 
    diametro = diametro - opArt; 
  }
}
