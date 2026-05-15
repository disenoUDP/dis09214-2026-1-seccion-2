# sesión 06 - 17/04   


# Transformaciones y condicionales
## Variables dinámicas nuevas ;o  

### Angulos Radiales  

P5 utiliza por defecto los angulos en radiales, esto puede ser complejo de entender y sostener.   
Para facilitar utilizaremos en el setup el **angleMode(DEGREES)** esto nos permitirá trabajar con grados y no palabras.

### Rotation y Traslate

Para hac
-> translate()  
-> rotation()

### Guardar y restaurar  

Funciones que trabajan juntas como un "sistema de memoria temporal" para el estilo y las transformaciones del lienzo.  
-> push();  
-> pop();

* Si yo quiero que un objeto gire o vaya en sentido antihorario, debo colocar un "-"
    * Ejemplo: rotate(-10);
 

### Escala


## Lógica Condicional y Expresión BOOLEANA

Ejemplo: Si algún estudiante apaga por completo las luces de la sala

#### Operadores  
Para construir las expresiones booleanas se usan 3 elementos  
-> Operandos (o Valores): Son datos básicos que se evalúan. Puede ser  
      -> Variables: como X, Y, mouseX, etc.
      -> Constantes o litearales: Valores fijos como "5, hola" o los mismos booleanos

-> Operaciones de comparación: Permite constrastar valores
      -> == Igual a
      -> != Desigual a
      -> > o < Mayor o menor a  
      -> >= o =< Igual o mayor/menor

-> Operadores Lógicos: Sirven para combinar varias expresiones  
      -> andperson **&&** Es verdadero solo si ambas partes son verdaderas.  
      -> or (||) A diferencia de & devuelve true cuando al menos uno de los operandos es igual a true.

## If - else if - else  
La sentencia if es una estructura especial que existe en casi todos los lenguajes de  programación; toma una condición –expresada como un booleano–  
y ejecuta una pieza de código contenida dentro de las llaves { }  

Ejemplo: If(condición){ejecutra este código si es true}  
else if:(condición 2){ejecutra este código si es true}
else{ejecuta este código si ambas condiciones son falsas}

* Esto sirve para generar acciones condicionales, ejemplos programar botones o acciones de uso :)
      

