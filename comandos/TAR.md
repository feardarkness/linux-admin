# TAR

tar se utiliza para unir archivos y comprimirlos.

Ejempo, para crear un archivo tar comprimido llamado exclusion.tar.gz, y excluir la carpeta mybkup/etc/ssh:

```
$ tar --exclude='mybkup/etc/ssh' -zcvf exclusion.tar.gz mybkup/
```
