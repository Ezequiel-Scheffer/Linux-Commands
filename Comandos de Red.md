# Comandos de RED

## Operaciones de RED
---------------------------

#### mostrar la configuración de Ethernet
```
ifconfig eth0
```

#### activar interface eth0
```
ifup eth0
```

#### deshabilitar interface eth0
```
ifdown eth0
```

#### configurar una dirección IP
```
ifconfig eth0 192.168.1.1 netmask 255.255.255.0
```

#### configurar eth0 en modo común para capturar paquetes (sniffing)
```
ifconfig eth0 promisc
```

#### activar la interface ‘eth0′ en modo dhcp
```
dhclient eth0
```

#### mostrar mesa de recorrido
```
route -n
```

#### configurar entrada predeterminada
```
route add -net 0/0 gw IP_Gateway
```

#### configurar ruta estática para buscar la red ’192.168.0.0/16′
```
route add -net 192.168.0.0 netmask 255.255.0.0 gw 192.168.1.1
```

#### eliminar ruta estática
```
route del 0/0 gw IP_gateway
```

#### activar recorrido ip
```
echo “1” > /proc/sys/net/ipv4/ip_forward
```

#### mostrar nombre del host
```
hostname
```

#### buscar nombre del host para resolver el nombre a una dirección ip
```
host www.paginaweb.com
```

#### buscar nombre del host para resolver el nombre a una dirección ip y viceversa
```
nslookup www.paginaweb.com
```

#### mostrar estado de enlace de todas las interfaces
```
ip link show
```

#### mostrar estado de enlace de eth0
```
mii-tool eth0
```

#### mostrar estadísticas de tarjeta de red eth0
```
ethtool eth0
```

#### mostrar todas las conexiones de red activas y sus PID
```
netstat -tup
```

#### mostrar todos los servicios de escucha de red en el sistema y sus PID
```
etstat -tupl
```

#### mostrar todo el tráfico HTTP
```
tcpdump tcp port 80
```

#### mostrar redes inalámbricas
```
iwlist scan
```

#### mostrar configuración de una tarjeta de red inalámbrica
```
iwconfig wlan0
```

#### buscar en base de datos Whois
```
whois www.paginaweb.com
```

---------------------------------------------
## SSH, SCP y Tunneling


#### iniciar sesion ssh
```
ssh usuario@servidor.dominio.es
```

#### iniciar sesion ssh con compatibilidad X11 (permite ejecutar tareas visuales)
```
ssh -X usuario@maquina 
```

#### iniciar sesion ssh en puerto determinado
```
ssh -p 15000 usuario@maquina 
```

#### copiar archivo mediante scp
```
scp /archivo usuario@servidor.dominio.es:/directorio
```

#### creacion de tunel ssh
```
ssh -f usuario@servidor.dominio.es -L 2000:servidor.dominio.es:25 -N
```

#### redireccion de puertos mediante tunneling
```
ssh -v -L4001:localhost:4001 usuario@servidor.dominio.es
```
