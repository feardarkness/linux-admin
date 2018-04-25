# Processes

Todo los procesos que corren tienen asociado un usuario. Init es el padre de todos los procesos, por eso tiene el PID 1.

Usualmente para ver los procesos se utilia top, htop ó ps.
```
$ top
$ htop
$ ps auxjf
```

Para buscar un proceso específico (devuelve el PID):

```
$ pgrep chrome

$ pidof chrome
```

Es posible matar procesos (PID 123), el ejemplo 2 envia la señal KILL (-9) al proceso 123:

```
$ kill 123
$ kill -KILL 123
```

Para ver todas las señales que pueden utilizarse:

```
$ kill -l
```

Si un proceso esta corriendo y consumiendo demasiado el CPU podemos cambiar su prioridad (NICE). Para cambiar el valor NICE a 5 del proceso 1234:

```
$ renice 5 1234
```