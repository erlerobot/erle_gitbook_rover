# Conectando a la placa Erle

Como se ha mencionado anteriormente,  [APMover2](https://github.com/BeaglePilot/ardupilot/tree/master/APMrover2) funciona en el modo de dirección deslizante, que significa que las cuatro ruedas se manejan bloqueando mecánicamente en la sincronización de cada lado. y que las ruedas de tracción del lado izquierdo se puede conducir de forma independiente de las ruedas motrices del lado derecho.

Así que cuando se conecta a la placa Erle tendremos que conectar los dos ESC: uno a los motores del lado derecho y otro a los motores del lado izquierdo. a los canales de salida uno y tres.

Siguiendo la documentación [Ardurover documentation](http://rover.ardupilot.com/wiki/table-of-contents/), podemos encontrar en la sección [APM setup](http://rover.ardupilot.com/wiki/setup/) que el canal 1 corresponde a los motores del lado izquierdo y el canal 3 a los motores de lado derecho.

En resumen:

|**Canal**|**Motores**|
|-----|-----|
|1|lado izquierdo|
|3|lado derecho|

Así que usted debe conectar el ESC siguiendo estas especificaciones, es decir el ESC del lado derecho en el canal 3 y el ESC del lado izquierdo al canal 1.
