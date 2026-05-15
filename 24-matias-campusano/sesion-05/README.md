# sesión 04 - 10/04
# Apuntes Pensamiento Computacional 10-04

## Variables integradas en P5.Js

### Posición del mouse  
Variables de sistema que determina la posición del mouse en coordenadas X e Y  
MouseX;  
MouseY;  
Ejemplo: Ellipse(mouseX, mouseY, 100,100);

#### Background  
Para que se marque la estela y generar un espacio de dibujo debemos dejar el background dentro del setup
No así si si dejo el background en la función **DRAW**  

### Variables integradas

## Creación de Variables Personales

Declarar tu variable:

let -> Para variables dinámiscas  
const -> Para variables constantes

Antiguamente se usaba *var* en vez de **let**.

Pasos para la variable.
1. Declarar tu variable -> let campoSanto; *(se puede inicializar la variable)*
2. Inicializa tu variable campoSanto = campoSanto+1
3. Usa tu variable

<img width="1552" height="458" alt="Captura de pantalla 2026-04-10 a la(s) 11 23 00 a m" src="https://github.com/user-attachments/assets/40d402a7-8fd9-46c6-8fa9-f5c6ef113f5e" />

La creación de variable siempre es lógica y avanza de pixel en pixel dependiendo de como queramos diagramar nuestro código.  

## Javascript Objects  
Esto sirve para organizar el código ordenado.  
Se agrupan valores dentro de una, esta estructura te permite agrupar variables sueltas como objetos dentro de un contenedor.  
Esto se organiza en pares de clave y valor.

### random();fuction  
Random()Si no pones nada devuelve un número decimal entre 0 y 1
    Ejemplo: random() da 0.4571.

### Variante Alpha le sume o le baja transparencia, este se puede usar en Stroke y Fill.

### Variable random

Se pueden crear varialbes juntas.
Al declarar las variables con el comando **Random** se puede utilizar como valor:
-> **widht** ancho
-> **height** altura

<img width="1732" height="458" alt="Captura de pantalla 2026-04-10 a la(s) 11 44 11 a m" src="https://github.com/user-attachments/assets/d760c551-2b7a-488a-9196-4d6698b8a698" />

### Posibilidad de viajes, mejoras y aprovechamiento de ayuda  
Ayuda de traducciones, ayuda, trabajo y posibilidad de becas 0:

## Sketch redimensionables  
createCanvas(windowWidth,windowHeight);

## map(); Fuction

Esta función nos permite convertir un valor de un rango a otro.
En términos simples: toma un número que está en una *escala* y lo traduce a una *escala* nueva

map(valor,min_original,max_original,min_nuevo,max_nuevo)

-> valor: variable que quieres mapear (por ejemplo, mouseX).
-> min_original y max_original: rango que se encuentra en ese valor actualmente
-> min_nuevo y max_nuevo: rango de lo que quieras transformar
