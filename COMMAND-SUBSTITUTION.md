# Substitución de comandos

Permite usar la salida de un comando como parte de otro comando.

P. e.:

1. Listamos el directorio donde se encuentra node.

```
$ ls -la $(which node)
```

## Comillas dobles
Para evitar brace expansion, command substitution (excepto $, \ y `), se puede utilizar la comilla doble.

## Comillas simples
Para evitar cualquier tipo de expansión, se utiliza comillas simples.

## Backslash
El backslash permite escapar un solo carácter, se utiliza comunmente en comillas dobles.

## Otros

Para ver el calendario utilizar **cal**.
