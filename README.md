# Configuración del entorno de desarrollo Web
## Introducción
1. En esta práctica se han visto los conceptos fundamentales para la creación de un espacio de trabajo en local. Para éllo se ha   instalado el programa Xampp que trabajará como servidor local. Eclipse será el editor de código. Se trabajajará con la directiva virtual host de apache.
---
## Indice 
1. Instalación Xamp
2. Configuración Virtual Host
3. Instalación de Eclipse
4. Definición del Workspace
5. Definición del proyecto
6. Definición del repositorio local
7. Creación del repositorio local
8. Exportación de la branca master
---
## 1. Instalación Xampp
Para la instalación de un servidor local se ha utilizado Xampp. El programa hace que se aplique el protocolo http a todos los documentos generados en el editor. https://github.com/excilia/pla1.pqtm10.local/commit/35fa8b0d2db7e7475ce9ed87895fc58e52d2664b#diff-364cd84a33221f56a55f6cd358870b99
## 2. Configuración Virtual Host
Se ha realizado la directiva Virtual Host consistente en modificar el archivo de apache httpd y el host de windows con objeto de indicar al servidor las ip y las dns de los directorios creados. Este es el texto que se tiene que poner en el fichero en la ruta C:\xampp\apache\conf\extra\httpd_vhosts.

NameVirtualHost *:80
##########################primer virtual host##############################################
 <VirtualHost *:80>
    ServerAdmin webmaster@proba.local
    DocumentRoot "C:/PQTM19/Projectes/proba.local"
    ServerName proba.local
	ErrorLog "logs/proba.local-error.log"
    CustomLog "logs/proba.local-access.log" common
	<Directory "C:/PQTM19/Projectes/proba.local">
		DirectoryIndex index.php index.html index.htm
		Options Indexes FollowSymLinks Includes ExecCGI
		AllowOverride All
		Order allow,deny
		Allow from all
		Require all granted
	</Directory>
</VirtualHost>

También se tiene que modificar el host en esta ruta y añadir la ip y el nombre del directorio
C:\Windows\System32\drivers\etc\hosts

## 3. Instalación de Eclipse
Se ha instalado Eclipse como editor de texto. Se ha instalado en un directorio creado en la carpeta Xampp.

## 4. Definición del Workspace
El workspace se ha definico en la carpeta indicada dentro de proyectos.

## 5. Definición del proyecto
El proyecto consiste en la creación de los directorios y las instrucciones necesarias para habilitar el espacio de trabajo.

## 6. Definición del repositorio local
Se ha diseñado un repositorio local en la carpeta Xampp

## 7. Creación del repositorio local
Se ha creado un repositorio local en la carpeta Xampp

## 8. Exportación de la branca master
La branca master puede ser guardada y actualida. También se puede descargar y ser abierto por cualquier persona que quiera acceder al proyecto generado.
