[![Waffle.io - Columns and their card count](https://badge.waffle.io/JuanCS95/prevencion-acoso.svg?columns=backlog)](https://waffle.io/JuanCS95/prevencion-acoso)
[![Build Status](https://travis-ci.org/JuanCS95/prevencion-acoso.svg?branch=master)](https://travis-ci.org/JuanCS95/prevencion-acoso)

# Prevención acoso

## Software necesario

Explicar aquí cómo instalar lo siguiente:
* JDK 1.8
-Antes de la instalacion de JDK, se necesitan abilitar repositorios adicionales. Con estas lineas se instalan los repositorios y java
sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer

-Use el comando siguiente para asegurarse de configurar la version de Java por defecto

sudo apt-get install oracle-java8-set-default

-luego de instalar java, use este comando para verificar que se instalo y para verificar la version
java -version
* Maven
-Para instalar primero actualize los paquetes con 

sudo apt update

-Luego instale Maven usando

sudo apt install maven

-Luego, para verificar la instalacion utilize

mvn -version

* MySQL

sudo apt-get update
sudo apt-get install mysql-server
mysql_secure_installation

* Eclipse

Para instalar Eclipse, descargue desde el link http://www.eclipse.org/downloads/index.php

Haga click derecho en el paquete que se descargue

Extraer el contenido en una carpeta

Haga doble click en el archivo Eclipse.exe para abrir Eclipse

Opcionalmente, haga click derecho en el archivo y presione crear accesso directo 

## Configuración del entorno

Explicar aquí cómo hacer lo siguiente:
* Crear la base de datos.
Para crear una base de datos
-Abra una consola
-entre en Mysql con:
Mysql -u root -proot
-incregre:
create database nombreDeBase;
* Cargar los datos iniciales.
Para cargar los datos iniciales, use el archivo DataGenerator para declarar los objetos a guardar en la base de datos.
Sobre el archivo GenerateDataMain use el boton derecho, vaya a run as y use Java Aplicacion
* Importar el proyecto en Eclipse.
Para importar un proyecto vaya a file, import en eclipse, luego elija el tipo de proyecto que quiere importar, busque el proyecto en su directorio antes de apretar finalizar
