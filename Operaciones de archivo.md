# Operaciones de Archivo

## Mostrar Contenido de Archivo
-------------------------------
#### muestra contenido de archivo
```
echo archivo
```

#### mostrar contenido de archivo
```
cat archivo
```

#### mostrar contenido de archivo empezando por el final
```
tac archivo
```

#### mostrar contenido de archivo desplazandose linea a linea
```
more archivo
```

#### mostrar contenido de archivo desplazandose adelante o atrás
```
less archivo
```

#### mostrar dos primeras lineas de archivo
```
head -2 archivo
```

#### mostrar dos ultimas lineas de archivo
```
tail -2 archivo
```

-------------------------------------------------------------------
## Manipilacion de texto


#### convertir minúsculas en mayúsculas
```
echo 'archivo' | tr '[:lower:]' '[:upper:]'
```

#### eliminar lineas 3 a 5 de archivo
```
sed '3,5d' archivo
```

#### eliminar lineas 5 a fin de archivo
```
sed '5,$d' archivo
```

#### eliminar linas en blanco
```
sed '/^$/d' archivo
```

#### eliminar linas en blanco y comentarios
```
sed '/ *#/d; /^$/d' archivo
```

#### sustituir una cadena por otra
```
sed 's/cadena1/cadena2/g' archivo 
```  

#### visualizar unicamente las líneas que contienen cadena
```
sed -n '/cadena/p'
```
