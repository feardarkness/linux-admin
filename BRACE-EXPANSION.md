# Expansión con llaves

Se utiliza para realizar multiples cadenas de un patrón.

Por ejemplo:

1. imprimiremos *ariel-1-sip ariel-2-sip ariel-3-sip ariel-4-sip*.
  ```
  $ echo ariel-{1,2,3,4}-sip
  otra forma
  $ echo ariel-{1..4}-sip
  ```
2. imprimimos un rango de letras ascendiente y descendiente
  ```
  $ echo {A..Z}
  $ echo {Z..A}
  ```

