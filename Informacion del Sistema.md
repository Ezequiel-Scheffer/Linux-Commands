# Informacion del Sistema

## Gestion de Recursos

#### mostrar tareas ejecutandose y su uso de recursos 
```
top
```

#### mostrar tareas ejecutables y recursos mejorado
```
htop
```

#### muestra el estado de la RAM en megabytes
```
free -h
```
--------------------------------------

## Espacio de Disco


#### mostrar una lista de las particiones montadas
```
df -h
```

#### mostrar el tamaño de los archivos y directorios ordenados por tamaño
```
ls -lSr |more
```

#### Estimar el espacio usado por el directorio ‘dir1′
```
du -sh directorio
```

#### mostrar el tamaño de los archivos y directorios ordenados por tamaño
```
du -sk * | sort -rn
```
----------------------------------------

## Informacion del Sistema


#### mostrar datos de usuarios conectados
```
who -a
```

#### mostrar historial de reinicio
```
last reboot
```

#### Mostrar arquitectura y versión de Linux y Kernel
```
uname -a
```

#### mostrar el kernel cargado.
```
lsmod
```

#### mostrar componentes de hardware del sistema.
```
dmidecode -q
```

#### Listar particiones de disco duro
```
*cat /etc/fstab
```

#### mostrar características de disco duro
```
hdparm -i /dev/hda
```

#### mostrar dispositivos PCI
```
lspci
```

#### mostrar dispositivos USB
```
lsusb
```

#### mostrar eventosde proceso de carga de kernel
```
tail /var/log/dmesg
```

#### mostrar los eventos del sistema
```
tail /var/log/messages
```

#### mostrar lista de archivos abiertos por procesos
```
lsof -p $$
```

#### mostrar lista de archivos abiertos en un camino dado del sistema
```
lsof /directorio
```

#### mostrar llamadas del sistema hechas y recibidas por un proceso
```
strace -c ls >/dev/null
```

#### mostrar las llamadas a la biblioteca
```
strace -f -e open ls >/dev/null
```

#### mostrar interrupciones en tiempo real
```
watch -n1 'cat /proc/interrupts'
```
----------------------------------------

## Listar procesos y tareas

#### mostrar procesos en background con jobID y PID
```
jobs -l
```

#### mostrar procesos
```
ps
```

#### mostrar procesos activos
```
ps -eafw
```

#### mostrar árbol de sistema de procesos.
```
pstree
```

#### mostrar procesos ordenados por consumo de memoria
```
ps aux | sort -k 5
```
---------------------------------

## Finalizar procesos

#### finalizar proceso para recargar configuracion
```
kill -1 ID_Processo
```

#### forzar cierte de proceso por PID
```
kill -9 PID
```

#### finalizar proceso por nombre
```
killall -9 nombre
```
