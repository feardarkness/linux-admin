# File permissions

- chmod
```sh
para dar permisos a todos
$ chmod a+rwx <nombre-archivo>

para dar permisos al usuario
$ chmod u+rwx <nombre-archivo>

para dar permisos al grupo
$ chmod g+rwx <nombre-archivo>

para dar permisos a otros
$ chmod o+rwx <nombre-archivo>
```
Aparte, se puede dar permisos por bits (1 execute, 2 write, 4 read)
```
$ chmod 421 <nombre-archivo>

para dar todos los permisos
$ chmod 777 <nombre-archivo>
```