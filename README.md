# SPANISH
Un taller de revisión de ITV quiere gestionar los vehículos
que van recibiendo para la revisión así como las colas que
estos vehículos van provocando a los diferentes boxes del
taller donde son atendidos.

El taller de revisión se compone de 6 boxes, todos ellos con las mismas
responsabilidades de revisión de vehículos, es decir, indistintamente del
box por el cual un vehículo paso, pasará por las mismas fases de
revisión, que son siempre 4 y con el siguiente orden:
1. Revisión inicial de elementos de seguridad
2. Revisión del sistema eléctrico
3. Revisión de emisión de humos
4. Revisión de frenos y dirección.

----------------------------------------------------------------------------

Desde el sistema se tendrá la capacidad decidir en cualquier momento
que los vehículos que estén dentro de un box se muevan todos a la vez, de
la fase de revisión donde estén hacia la fase siguiente. Se asume en
este caso que están todos listos para pasar de fase y que un supuesto
mecánico los ha dado el visto bueno.

Cuando un vehículo llega al taller se le toma tanto el número de matrícula
(4 números seguidos de 3 letras) como el modelo y del vehículo, además del
tipo que puede ser (coche, microbús, furgoneta o camión). Si el registro
del vehículo es correcto (no puede haber dos vehículos con la misma
matrícula), este vehículo se pondrá automáticamente a la cola general.

La cola general no pertenece a ningún box concreto, pudiendo pasar a la cola
de fases de revisión del box que desde el programa informático se
decida. Lógicamente, la primera fase de revisión del box que reclamo
al siguiente vehículo de la cola general tiene que estar libre para atender este
vehículo, sino se le denegará ese reclamo.

----------------------------------------------------------------------------
Las opciones que el programa tiene que presentar al menú son las siguientes:
----------------------------------------------------------------------------
1. Alta y recepción de vehículos: se encargará de pedir los datos
de registro del vehículo y ponerlo automáticamente a la cola
general. No se podrán introducir a la cola dos vehículos con la
misma matrícula. Si alguna de los datos se introduce
incorrectamente, se volverá a pedir el dato hasta que
se introduzca bien. Hay que informar el usuario sobre en qué posición de
la cola general se encuentra el vehículo recibido.

2. Reclamar vehículo para entrar al box: se preguntará por el box que
desea recibir el siguiente vehículo que se encuentra a la cola inicial, si es
que hay alguno y hay lugar para él en ese box (no hay
de haber ningún vehículo en la primera fase de revisión de ese box). Si no
se introduce un número de box correcto, se volverá a pedir
hasta que sea válido. Si no es posible la entrada del vehículo al box,
se denegará esta operación informando al usuario (tanto en el caso
favorable como al desfavorable de la operación).

3. Mover todos los vehículos de fase dentro de un box. Se preguntará por el
número de box donde se quiere desplazar una fase a todos los vehículos
para sus adentros. Por supuesto, si un vehículo se encuentra en la última fase,
quedará ya fuera del box.

4. Información del estado de un box concreto: se preguntará por el
número de box (entre 1 y 6). Se mostrará en qué estado se encuentra
cada fase del box, mostrando de cada una qué vehículo tiene
asignado (mostrando su matrícula, marca, modelo y su tipo),
si lo tiene.

5. Información general de todos los boxes: similar a la opción anterior
pero por los 6 boxes del taller.

6. Salir del programa.
