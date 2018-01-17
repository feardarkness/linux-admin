# VIM

En command mode
- dd: eliminar una línea
- a: para comenzar a editar, append
- i: para comenzar a editar, insert
- o: para insertar una línea despues de la línea en donde nos encontramos
- yy: para copiar la línea entera
- p: para pegar despues de la línea en donde nos encontramos
- P: para pegar antes de la línea en donde nos encontramos
- u: para hacer undo de la última modificación. Si se continua presionando u va hasta el primer cambio.
- /: para buscar, ej: /texto, luego presionar n para buscar la siguiente línea que iguala el texto.

Con :
- *:$* para ir al final del documento
- *:q* para salir (si existen cambios, se hará un mensaje de advertencia)
- *:q!* para olvidar los cambios que se han realizado al documento y salir de vim
- *:e!* para olvidar los cambios que se han realizado al documento, sin salir de vim
- *:w* para guardar el archivo
- *:wq* para guardar el archivo y salir

