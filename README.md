[![Waffle.io - Columns and their card count](https://badge.waffle.io/JuanCS95/prevencion-acoso.svg?columns=backlog)](https://waffle.io/JuanCS95/prevencion-acoso)
[![Build Status](https://travis-ci.org/JuanCS95/prevencion-acoso.svg?branch=master)](https://travis-ci.org/JuanCS95/prevencion-acoso)

# Prevención acoso

## Software necesario

Explicar aquí cómo instalar lo siguiente:
* JDK 1.8

-Antes de la instalacion de JDK, se necesitan abilitar repositorios adicionales. Con estas lineas se instalan los repositorios y java
```
$ sudo apt-get install openjdk-8-jre
```

* Maven

-Para instalar primero actualize los paquetes con 
```
sudo apt update
```
-Luego instale Maven usando
```
sudo apt install maven
```
-Luego, para verificar la instalacion utilize
```
mvn -version
```
* MySQL
```
sudo apt-get update
sudo apt-get install mysql-server
mysql_secure_installation
```
* Eclipse

Abra un terminal (Ctrl-Alt-T) y cámbielo a permisos de raíz ingresando:
```
$ sudo su
```
Asegúrese de que Eclipse Indigo NO esté instalado en su Ubuntu. Es posible que deba eliminar los paquetes "eclipse" y "eclipse-platform" para deshacerse de ellos.
```
# apt-get remove eclipse eclipse-platform
## Configuración del entorno
```
Instala un Java 1.7 JDK
Instale Maven

Deshazte del acceso de root ya que no lo necesitarás más:
```
# salida
```

Descargar Eclipse. Las versiones "para desarrolladores Java EE", "para desarrolladores Java" y "para desarrolladores RCP y RAP" parecen funcionar. Actualmente, el archivo que se probó para trabajar está (tenga en cuenta que es para la versión de Ubuntu de 64 bits) disponible en esta página
Extraiga el archivo de instalación de Eclipse en su directorio de inicio:
```
$ cd
$ tar -xzvf <ruta / a / tu-archivo-tar>
```
Aumente la memoria para la instalación de Eclipse modificando el archivo ~ / eclipse / eclipse.ini.
Cambie la configuración de -Xmx (línea 20) a al menos 1G, se recomienda 2GB. (es decir, -Xmx2048m).
Cambie el -XX: MaxPermSize (línea 18) a un máximo de 512 m. Si tiene el ajuste -Xmx establecido en 1G, le sugiero que utilice un valor más bajo, por ejemplo, 300 m.
Ejecutar el Eclipse:
```
$ ~ / eclipse / eclipse
```
* Crear la base de datos.

Para crear una base de datos

-Abra una consola

-entre en Mysql con:
```
Mysql -u root -proot
```
-ingrece:
```
create database nombreDeBase;
```
* Cargar los datos iniciales.

Para cargar los datos iniciales, use el archivo DataGenerator para declarar los objetos a guardar en la base de datos.
Sobre el archivo GenerateDataMain use el boton derecho, vaya a run as y use Java Aplicacion
* Importar el proyecto en Eclipse.

Para importar un proyecto vaya a file, import en eclipse, luego elija el tipo de proyecto que quiere importar, busque el proyecto en su directorio antes de apretar finalizar
