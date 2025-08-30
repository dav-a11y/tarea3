# Tarea 3 - Práctica de Comandos Básicos en Linux

## Objetivo
Documentar el uso de comandos básicos de Linux para la creación, navegación, edición, copia, eliminación de archivos, administración de permisos, búsqueda de información, gestión de procesos y uso de paquetes.  
Se incluye además la creación de un script sencillo.

---

## Materiales
- Computador con Linux.
- Terminal de comandos.
- Cuenta de GitHub para subir la tarea.
- Editor de texto (`nano`, `vim`, `gedit`, etc.).
- Paquete `cowsay` instalado.

---
## Desarrollo paso a paso

### Navegación
1. Abrir la terminal y dirigirse al directorio personal con:
   cd ~
   
2. En la terminal Verificar ubicación:
   pwd

3. En la terminal Listar archivos y directorios:
   ls -l

   ![paso 1]("pantallazos\cd pwm ls.jpeg")

### Crear directorios  
   
1. En la terminal Crear carpeta principal:
   mkdir Practica_Linux

   
2. En la terminal Crear subdirectorios:
   mkdir Practica_Linux/Documentos
   mkdir Practica_Linux/Backup

   ![paso 2]("pantallazos\mkdir.jpeg")

### Crear y editar archivos
   
1. En la terminal Crear archivo vacío:
   touch Practica_Linux/Documentos/nota.txt
   
   
2. En la terminal Editar el archivo:
   nano Practica_Linux/Documentos/nota.txt

   ![paso 3]("pantallazos\touch nano y cd.jpeg")
   
3. En la terminal Verificar Contenido:
   Hola, este es mi primer archivo en Linux.


### Copiar y renombrar archivos

1. Copiar nota.txt a Backup:
   cp Practica_Linux/Documentos/nota.txt Practica_Linux/Backup/


2. Renombrar archivo original:
   mv Practica_Linux/Documentos/nota.txt Practica_Linux/Documentos/nota_final.txt


### Eliminar y ver contenido

1. Eliminar carpeta Backup:
   rmdir Practica_Linux/Backup

   ![paso 4]("pantallazos\rm.jpeg")

2. Ver contenido:
   cat Practica_Linux/Documentos/nota_final.txt


### Permisos

1. Cambiar permisos:
   chmod 600 Practica_Linux/Documentos/nota_final.txt

   ![paso 5]("pantallazos\chmod.jpeg")


2. Verificar:
   ls -l Practica_Linux/Documentos/
   
   
### Buscar y Filtrar

1. Buscar archivo:


2. Buscar palabra "Linux":

   ![paso 6]("pantallazos\grep.jpeg")

### Procesos

1. Ver procesos:
   top

   ![paso 7]("pantallazos\htop.jpeg")

2. Crear proceso y matarlo:
   sleep 300 &
   kill [PID]

   ![paso 8]("pantallazos\sleep 300.jpeg")

### Paquetes

1. Actualizar paquetes:
   sudo apt update


2. Instalar cowsay:
   sudo apt install cowsay

   ![paso 9]("pantallazos\cowsay.jpeg")

### Script Final

1. Archivo: mis_comandos.sh
   #!/bin/bash
   mkdir -p logs
   date > logs/fecha.text
   cowsay "¡Ejercicio completado!"


2. Ejecutar:
   bash mis_comandos.sh

   ![paso 10]("pantallazos\mis comandos 3.jpeg")
 

