# Comandos Basicos y permisos



## Comandos básicos para manejo de ficheros

| Comando       |   Descripcion |
| ------------- | ------------- |
| `mv` |mover/renombrar archivos/directorios|
| `ls` |lista los archivos dentro de un directorio|
| `ln` |crea ligas a archivos|

## Administrar los permisos y la propiedad de los ficheros

chmod - cambia permisos del archivo/directorio

    u -> user  -> usuario

    g -> group -> grupo

    o -> other -> otros

    a -> all   -> todos

     

    + -> agrega permisos

    - -> quita permisos

     

    r -> lectura

    w -> escritura

    x -> ejecucion para archivo paso Transversal (puedo moverme atravez de el) para directorios

    s -> setuid/setgid

     

    ejemplo:

    `chmod g+rwx archivo.txt`

    agrega permisos de escritura, lectura y ejecucion al archivo.txt para el grupo

    `chmod a-r archivo.txt`

    elimina permisos de lectura a todos los usuarios (grupos y dueño incluidos)

     

    [Cambio de permisos con numeros octales](https://es.wikipedia.org/wiki/Sistema_octal)

     


    421 421 421

    rwx rwx rwx

     

    si quieres permisos de lectura es 4

    si quieres permisos de escritura es 2

    si quieres permisis de ejecucion es 1

    para combinar permisos los sumas por ejemplo, si quieres ejecucion y escritura es 2 + 1 = 3

     

    `$ chmod 751 archivo.txt`

     

    usuario tiene permisos 7 que es 4+2+1 que significa lectura,escritura y ejecucion

    grupo tiene permisos 5 que es 4 + 0 + 1 que significa lectura y ejecucion

    otros tiene permosos 1 que es 0 + 0 + 1 que solo significa ejecucion

     

chown - cambia al dueño/grupo del archivo/directorio

    `$ chown NuevoUser archivo`

    cambia el dueño actual a uno nuevo

    `chown NuevoUser:NuevoGrupo archivo`

    cambia el dueño actual y grupo actual del archivo

## Comandos miscelaneos

| Comando       |   Descripcion |
| ------------- | ------------- |
| `pwd`| Despliega el directorio actual de trabajo |
