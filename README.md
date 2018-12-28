# Emparejamiento
Servidor para emparejar jugadores

Este proyecto es la parte Servidor de un cliente-servidor, se encarga de recibir mensajes solicitando jugar a un juego (identificado por código), por ejemplo 3eR (tres en raya) y un puerto en el que el cliente abrirá el servidor (si es el host).

Los mensajes al servidor usan el formato <código_de_juego>/<puerto>

Si no hay otro cliente que haya querido jugar al mismo juego el servidor le devolverá null y el cliente abrirá el puerto, esperando a otro jugador. Será el host.

Si hay cliente el servidor devolverá un mensaje <ip>:<puerto> y el cliente deberá conectarse a él.
