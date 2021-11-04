# asincronismo-js
Curso de Asincronismo con JavaScript (Platzi)
Oscar Barajas Tavares

# Ejes
Callbacks
Promesas
Async Await

## Asincronismo
JS es un lenguaje de programacion asincrono y no bloqueante con un manejador de eventos (event-loop) implementando en un unico hilo para sus interfaces de entrada y de salida.

El asincronismo es básicamente una manera de aprovechar el tiempo y los recursos de nuestra aplicación, ejecutando tareas y procesos mientras otros son resueltos en background (como la llegada de la información de una API), para posteriormente continuar con las tareas que requerían esa información que no tenías de manera instantánea.


### Memory heap
Región de memoria libre, normalmente de gran tamaño, dedicada al alojamiento dinámico de
objetos. Es compartida por todo el programa y controlada por un recolector de basura que se
encarga de liberar aquello que no se necesita.

### Pila de ejecucion (call stack)
La pila de llamadas, se encarga de albergar las instrucciones que deben ejecutarse. Nos indica en que punto del programa estamos, por donde vamos.

### Cola de tareas (Queue)
Cada vez que nuestro programa recibe una notificación del exterior o de otro contexto distinto al de la aplicación, el mensaje se inserta en una cola de mensajes pendientes y se registra su callback correspondiente.

### Eventloop o Loop de eventos
Cuando la pila de llamadas (call stack) se vacía, es decir, no hay nada más que ejecutar, se
procesan los mensajes de la cola. Con cada ‘tick’ del bucle de eventos, se procesa un nuevo
mensaje.


## Callbacks
Una funcion que recibe como argumento otra funcion y la cual se ejecuta cuando esta es llamada.

### Generar scripts en package.json y usarlos
"scripts": {
    "callback": "node src/callback/index.js"
},

npm run callback


