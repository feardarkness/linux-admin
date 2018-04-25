# SFTP

Es ftp sobre ssh. Una vez dentro los archivos obtenidos se almacenan en el mismo directorio desde donde ejecutamos sftp.
Como utilizar *sftp <user>@<password>*:
```
$ sftp user@192.168.26.25
```

Una vez dentro se pueden utilizar los comandos conocidos (ls, pwd, etc)

Para obtener un archivo, utilizar *GET <nombre-archivo> <nombre-archivo-copiado>*
```
$ GET out.txt
```

Para cambiar el directorio a donde queremos que se copie los archivos *lcd <nombre-directorio>*
```
$ lcd /home/fear/carpeta-nueva
```
