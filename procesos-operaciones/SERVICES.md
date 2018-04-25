# Managing starting processes

Para administrar procesos se utiliza upstart o systemd.

Los procesos que se inician se encuentran en /etc/init ó en /etc/rc.local y ver las carpetas.

Para upstart:

```
Estado de un servicio
$ status <servicio>

Iniciar de un servicio
$ start <servicio>

Detener de un servicio
$ stop <servicio>

Reiniciar de un servicio
$ restart <servicio>

Para evitar que se inicie al reiniciar, es necesario crear en /etc/init un archivo override con el contenido "manual", luego para que se el servicio inicie al reniciar el servidor simplemente eliminar dicho archivo:
$ echo manual | sudo tee /etc/init/ssh.override

```

Para ver las unidades que estan corriendo:

```
Listar todos los servicios
$ systemctl list-units

Ver los procesos que estan activo s para iniciarse automaticamente
$ systemctl list-unit-files | grep enabled

Para ver los procesos que estan corriendo actualmente
$ systemctl | grep running

Estado de un servicio
$ systemctl status <servicio>

Iniciar de un servicio
$ systemctl start <servicio>

Detener de un servicio
$ systemctl stop <servicio>

Reiniciar de un servicio
$ systemctl restart <servicio>

Para evitar que se inicie al reiniciar
$ systemctl disable <servicio>

Para frozar que se inicie al reiniciar
$ systemctl enable <servicio>

Alternativamente se puede utilizar service, p. e.:
$ service ssh status
```