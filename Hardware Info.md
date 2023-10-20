# Informacion del Hardware del Sistema

## lscpu

#### El comando lscpu informa sobre la CPU y las unidades de procesamiento, una de las partes mas importantes del hardware en Linux. El comando no tiene más opciones o funcionalidades.
```
lscpu
```
--------------------------------------

## lshw – Lista de hardware en Linux

#### Esta utilidad de propósito general nos brinda información breve y detallada sobre múltiples unidades de hardware en Linux, como CPU, memoria, disco, controladores usb, adaptadores de red, etc. Lshw extrae la información de diferentes /proc files.
```
sudo lshw -short
```
--------------------------------------

## hwinfo – Información del hardware en Linux

#### Hwinfo es otra utilidad de prueba de hardware en Linux, de propósito general que puede brinda información breve y detallada sobre múltiples componentes de hardware diferentes. Su información es mucho mas extensa de lo que lshw puede aportar.
```
hwinfo --short
```
--------------------------------------

## lspci – Lista dispositivos pci

#### El comando lspci enumera todos los buses pci y detalles sobre los dispositivos conectados a ellos.El adaptador vga, la tarjeta gráfica, el adaptador de red, los puertos usb, los controladores sata, etc. caen dentro de esta categoría.
```
lspci
```

Si queremos, también podemos filtrar la información específica del dispositivo con grep:

```
lspci -v | grep "VGA" -A 12
```
--------------------------------------

## lsscsi – Listar dispositivos scsi
#### Enumera los dispositivos scsi / sata, como los discos duros y las unidades ópticas.
```
lsscsi
```
--------------------------------------

## lsusb – Lista de los usb
#### Este comando muestra los controladores USB y detalles sobre los dispositivos conectados a ellos. Por defecto, se imprime una breve información.
```
lsusb
```
--------------------------------------

## lsblk – Lista de dispositivos de bloque
#### Enumerar la información de todos los dispositivos de bloque, que son las particiones de disco duro y otros dispositivos de almacenamiento como unidades ópticas y unidades de memoria flash.
```
lsblk
```
--------------------------------------
