# Operaciones matemáticas

Para realizar operaciones matemáticas se puede utilizar $((expression)). Las operaciones aritméticas posibles son: +, -, *, /, % y **(exponenciación).

Ejemplo:

1. Sumar dos más dos:
  ```
  $ echo $((2+2))
  ```

2. Sumar tres más dos y luego elevar el resultado al cuadrado.
  ```
  $ echo $(($((3+2))**2))
  además, es posible agrupar con parentesis
  $ echo $(((3+2)**2))
  ```


