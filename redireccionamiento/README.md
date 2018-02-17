# Redireccionamiento

Para realizar los redireccionamientos, se utilizará:

* cat: para concatenar
* sort: para ordenar
* uniq: reportar u omitir lineas repetidas
* wc: conteo de palabras,salto de líneas y bytes
* grep: Filtros
* head: imprimir la primera parte de los archivos
* tail: imprimir la última parte de los archivos
* tee: leer del "standard input" e imprimir al "standard output" ó archivos.
* fmt: Para eliminar espacios entre palabras u otros (quizas saltos de línea). -u uniforma los espacios, un espacio entre palabras y dos espacios entre párrafos.
* nl: para contar líneas

## Standard Input, Output and Error

Todos los programas envian sus resultados a un archivo especial llamado "standard output" (stdout) y los estados de los mensajes a un archivo llamado "standard err" (stderr).

0 input
1 output
2 error

Por defecto ambos están vinculados a la pantalla y no almacenados a un archivo en el disco. Además, muchos programas toman la "standard input" (stdin) que esta vinculada al teclado por defecto.

El carácter que se necesita para hacerlo anexar datos a un archivo es **>**. Si lo utilizamos, permite redireccionar la salida de un comando a otro lugar, en caso de error el archivo de destino queda truncado, con **>>** se puede anexar a un archivo.

Para redireccionar tanto stdout y stderr a un mismo archivo utilizamos (el orden es necesario, la redirección de stdout debe ocurrir siempre antes que la redirección de stderr):

```
$ ls -la /root > resultado.txt 2>&1
```

Otra forma es con **&>**:

```
$ ls -la /root &> resultado.txt
```

Si queremos redireccionar todo a la nada se puede redireccionar a **/dev/null**, por ejemplo para redireccionar el error de un comando y que no se vea en la pantalla:

```
$ ls -la /root 2> /dev/null
```

Si queremos evitar que el operador > reescriba el contenido de un archivo (dará error):

```
$ set -o noclobber
Para habilitar nuevamente
$ set +o noclobber
```


