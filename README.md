# Linux-Commands
review of common linux commands


------------------------------

## CLI

#### Listar los CLI disponobles
```
cat /etc/shells
```
#### Saber con cual CLI estamos trabajando

```
echo $0
```
-------------------------------

## Desplazarse entre directorios

#### ir a directorio de raiz
```
cd
```

#### ir a directorio anterior
```
cd ..
```

#### entrar en directorio (ruta absoluta)
```
cd /directorio1/directorio
```

#### entrar en directorio (ruta relativa)
```
cd directorio1/directorio2
```

#### ir a directorio de usuario
```
cd ~
```

#### ir a ultimo directorio visitado
```
cd -
```

#### mostrar ruta actual
```
pwd
```
-------------------------------

## Listar archivos y Directorios

#### mostrar archivos y directorios
```
ls
```

#### mostrar archivos y directorios con detalles
```
ls -l
```

#### mostrar archivos y directorios incluidos los ocultos
```
ls -a
```

-------------------------------

## Manipulacion de Archivos y Directorios

#### renombrar o mover un archivo o directorio
```
mv origen destino
```

#### copiar un archivo
```
cp archivo direccion
```

#### copiar un directorio
```
cp -r origen destino
```

#### borrar el archivo llamado archivo
```
rm archivo
```

#### borrar directorio si está vacio
```
rm -d directorio
```

#### borrar directorio y su contenido
```
rm -r directorio
```

#### crear nuevo directorio
```
mkdir directorio
```

#### crear varios directorios simultáneamente
```
mkdir directorio1 directorio2
```

#### crear ruta de directorios
```
mkdir -p /directorio1/directorio2
```

#### crear archivo vacio
```
touch archivo
```
---------------------------------

## Enlaces Simbolicos


#### crear un enlace simbólico al archivo o directorio
```
ln -s archivo lnk1
```

#### crear enlace físico al archivo o directorio
```
ln archivo lnk1
```

-----------------------------------------------

## Ejecucion de comandos

### Ejecutar secuencialmente 2 comandos
Independientemente del resultado del comando1
```
comando1 ; comando2
```

Si el comando1 se ha ejecutado correctamente se ejecuta el comando2
```
comando1 && comando2
```

Si el comando1 se ha ejecutado de manera incorecta se ejecuta el comando2
```
comando1 || comando2
```

### Tuberias y Redirecciones

#### dirigir salida de comando a nuevo archivo
```
comando > archivo_out.txt
```

#### digir salida de comando para añadir a archivo 
```
comando >> archivo_out.txt
```

#### dirigir entrada de comandos
```
comando < archivo_in.txt
```

#### dirigir salida estandar y salida de error a un fichero:
```
comando &> archivo_out.txt
```

#### tuberia, dirigir salida de comando1 como entrada de comando2
```
comando1 | comando2
```

#### Ejecutar aplicacion en segundo plano

```
comando &
```
Para ver los procesos que se estan ejecutando en segundo plano:

```
bg
```
Para recuperar el ultimo proceso que se esta ejecutando en segundo plano:
```
fg
```

### Historial de Bash 

#### Para repetir el ultimo comando utilizado

```
!!
```
> Ejemplo: sudo !!

#### El comando anterior sin la última palabra
```
!*
```

#### La última palabra del comando anterior
```
!$  
```

#### Todos los parámetros del comando anterior
```
$*
```
>Ejemplo:
>```
>mkdir veryLongName
>cd $*
>```
>

#### Todos los parámetros del comando anterior como vector
``` 
$@
```
 -----------------------------------------------

## Ayuda sobre comandos

#### Mostrar un resumen de la funcion del comando xxxxx
```
whatis xxxxx
```

#### Mostrar la localización más probable para el programa xxxxxx
```
whereis xxxxx
```

#### Listar las páginas de manual que tratan acerca del comando xxxxx
```
apropos xxxxx
```

#### Mostrar el manual de uso o configuración del programa xxxxx
```
man xxxxx
```

#### Mostrar las páginas de manual que contengan la palabra xxxxx
```
man –k xxxxx
```

-----------------------------------------------

