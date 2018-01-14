# Filters

Los filtros toman una entrada, los modifican y sacan los datos.

- cat: Permite concatenar archivos. Lee uno o más archivos y los copia a stdout. Si ponemos solamente cat, se queda esperando datos desde stdin
- sort: permite ordenar los datos
- uniq: omite líneas repetidas
- wc: permite contar cantidad de líneas, palabras o bytes.
- grep: busca patrones de texto en archivos. Para buscar case insensitive **-i**, para buscar líneas que no igualan al patrón usar **-v**.
- tee: lee desde stdin, saca a stdout y a un archivo.
- split: Permite dividir un archivo de acuerdo a un acierta cantidad de líneas.
- diff: permite ver que líneas son diferentes entre dos archivos. El < representa el primer archivo, > representa el segundo. a add, d delete, c change

Ejemplos:
1. Para ver la cantidad de líneas que un comando devuelve en un comando utilizar:
  ```
  $ cat archivo.txt > wc -l
  ```

1. Para almacenar a un archivo los resultados del listado y luego buscar una palabra.
  ```
  $ cat archivo.txt > wc -l
  ```

1. Para dividir el archivo ar.txt en tres líneas cada uno (crea archivos xomo xaa, xab, xac...):
  ```
  $ split -l 3 ar.txt
  ```

