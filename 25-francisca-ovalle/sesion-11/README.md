# sesión 11 - 19/06  
-------
# SONIDO: INTRODUCCIÓN A LA PROGRAMACIÓN EN p5.js
---

## PARTE 1: TRABAJO CON ARCHIVOS DE SONIDO *loadSound*

#### PASO 1: Subir sus sonidos a P5
1. Hacer clic en la pequeña **flecha hacia la derecha (>)** ubicada en la esquina superior izquierda del editor (debajo del botón de *Play*). Esto abrirá el menú de archivos laterales.
2. Hacer clic en el icono de **+** o el menú desplegable junto a *Files*.
3. Seleccionar **Upload file**
4. Arrastrar el archivo de sonido.
   * *Formatos recomendados:* mp3 o wav
5. **Recomendación:** usar nombres de archivo cortos, en minúsculas y sin espacios. Hacer una carpeta llamada ASSETS.

#### PASO 2: Declarar y precargar el sonido  
1. Creamos una variable global al inicio del código para guardar nuestro sonido.
2. Usamos el function preload inicializamos nuestra variable y cargamos el sonido con loadSound.
   
### PASO 3: Activar mi sonido
Le damos play al sonido en el function setup con:  

Con esta instrucción, el sonido va a comenzar cuando le demos play a nuestro sketch.  

#### Lo ideal es activar mi sonido con un *mousePressed*

## MÉTODOS Y FUNCIONES DE CONTROL

### Métodos de control de sonido  
Play: Reproduce el sonido una vez.
Loop: Reproduce el sonido en bucle infinito.  
Stop: Detiene el sonido por completo.  
Pause: Pausa el sonido en el segundo actual.  
setVolume : Modifica el volumen.  
Rate: Modifica la velocidad de reproducción.   
  
### Métodos de consulta o estados del sonido  
Playing: Devuelve true si el sonido está sonando en este momento y false si no.  
Pause: Devuelve true si el sonido fue congelado con pause.  
Looping: Devuelve true si el sonido está configurado para repetirse en loop.  
currentTime: Devuelve el segundo exacto en el que va la reproducción   
Duration: Devuelve la duración total del archivo de audio en segundos   
gotVolume: Devuelve el nivel de volumen actual del reproductor (un número entre   
getRate: Devuelve la velocidad de reproducción actual   


## PARTE 2: SÍNTESIS DE AUDIO 

### 3 Componentes de un Sintetizador Básico

El oscilador, sine, triangle, sawthonth, square
*La frecuencia:* Controla qué tan rápido vibra la onda. Matemáticamente, a mayor frecuencia, el sonido es más agudo; a menor frecuencia, es más grave.   
*La Amplitud: Controla la altura de la onda, lo que nosotros percibimos como el volumen.  

