# SED
Para filtrar y transformar textos.

- s para substitución
- 2 para escribir a un archivo

1. Substituimos la palabra *gato* con *pato* en todas las líneas.
  ```
  $ sed '/s/gato/pato/' archivo.txt
  ```

1. Substituimos la palabra *gato* con *pato*, y escribimos al archivo *pato.txt*. Solo se escriben las líneas modificadas
  ```
  $ sed '/s/gato/pato/w pato.txt' archivo.txt
  ```

1. Substituimos la palabra *gato* con *pato*, solo la primera línea encontrada con la palabra *gato*
  ```
  $ sed '0,/gato/s/gato/pato/' archivo.txt
  ```

