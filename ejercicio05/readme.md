--
## Ejercicio 05- Taller Docker

### Healthcheck
El comando healthcheck se utiliza para verificar que un contenedor este funcionando correctamente. Que puede ayudar a identificar casos como por ejemplo que un servidor s
se encuentra en un bucle infinito y no puede realizar mas peticiones. Asi incluso si el contenedor siga ejecutandose.

Cada contenedor que tiene asignado un healthcheck, inicia con un estado inicial ( starting ). Cada vez que se ejecuta correctamente el checkeo pasa a ser saludable 
( healthy ). Si el checkeo por alguna razón falla, este vuelve a reintentar el checkeo (Por default 3), pasa a ser de estado insalubre ( unhealthy ), O también si el checkeo 
tarda demasiado ( default 30s ) entonces pasará a estado ( unhealthy ).


### Onbuild
El comando Onbuild permite establecer disparadores en una imagen. Posibilitando crear un contexto para cuando la imagen se use de base en otra imagen.
Esto permite automatizar tareas, como lo es la compilación de código. El Onbuild le inyecta las instrucciones a los metadatos del imagen.
Esto no altera la imagen final, ya que solo utiliza la imagen base para preconfigurar el constructor.

Una advertencia que si nos da la documentación de docker es que no se puede utilizar onbuild y onbuild sucesivamente. Ya que no permite un encadenamiento secuencial.

### Volume

El comando Volume permite hacer un bind-mount para poder percistir los datos de un contenedor, para que cuando se detenga o elimine el contenedor, los datos sigan estando.
