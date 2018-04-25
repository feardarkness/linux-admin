# Para instalar packages

Se puede utilizar dpkg o apt.

Para listar todas las dependencias instaladas:
```
$ dpkg -l
```

Para listar las ubicaciones de todo lo instalado con un paquete
```
$ dpkg -L <nombre-paquete>
$ dpkg -L xterm
```

Para listar con apt-get los paquetes disponibles:
```
$ apt-cache pkgnames
```

Para buscar un paquete:
```
$ apt-cache search xterm
```
