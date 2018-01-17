# TEST

Para realizar tests. Permite validar si es unarchivo, un directorio u otros, también permite comparar valores.

También se puede utilizar como brackets

1. Imprime *sip* si 5 es igual a 5.
  ```
  $ test 5 -eq 5 && echo 'sip'
  ```

1. Imprime *sip* si 5 es igual a 5. Ojo con los espacios.
  ```
  $ [ 5 -eq 5 ]; echo 'sip'
  ```

1. Imprime el resultado de la compración de 5 con 5.
  ```
  $ [ 5 -eq 5 ]; echo $?
  ```