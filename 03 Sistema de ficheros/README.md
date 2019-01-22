## Sistema de archivos

Un sistema de archivos es a grandes rasgos la forma en la que se almacenan
archivos y carpetas dentro de una partición en un disco o otro medio de
almacenamiento, por ejemplo, memorias USB, microSD, etc.

Un sistema de ficheros popular para memorias USB y microSD es **FAT**, en
Windows la unidad C: usa un sistema de archivos **NTFS**, etc.

Linux soporta una gran cantidad de sistema de ficheros, pero el más
común en las mayoria de las distros es ***ext4***.

## Sistemas de archivos en Linux

Algunos sistemas de ficheros que Linux entiende:

::: columns

:::: column

Para discos convencionales:

* ext2, ext3, ext4
* xfs
* zfs
* btrfs
* ntfs

::::

:::: column

Para memorias flash:

* FAT
* ubifs
* f2fs
* jffs2

::::

:::

## Particiones y sistemas de ficheros

Una partición debemos imaginarla como una región física de un disco,
en donde se almacenan archivos y carpetas usando un mismo método.

El sistema de ficheros es ese método de almacenar un archivo o carpeta
dentro de la partición.

Hay muchas forma de guardar archivos en una partición, cada una de
ellas tiene sus ventajas y desventajas.

Sin embargo Linux se encarga de dar acceso a los archivos y carpetas
sin importar la partición donde se encuentren o el sistema de archivos
que se use.

## Directorios y particiones

En los sistemas basados en UNIX todas las particiones, aparecen bajo la
misma estructura de carpetas, sin importar el sistema de ficheros que
usen o si se encuentran en un dispositivo físico diferente.

Esta estructura de carpetas se puede ver como un árbol, cuya raíz es
la carpeta /, cada carpeta dentro de la raíz es una rama, los archivos
son hojas y cada rama puede tener más ramas en ella.

Cuando se *monta* una partición, es como si tomáramos todas las ramas
dentro de la partición y se añadieran al árbol principal.

## Jerarquía Estándar

La jerarquía estándar del sistema de ficheros es la estructura de
carpetas que se puede esperar encontrar en cualquier sistema basado
en Linux.

![[Filesystem Hierarchy Standard](https://es.wikipedia.org/wiki/Filesystem_Hierarchy_Standard#Especificando_los_directorios_definidos_por_FHS)](../res/img/dirtree.jpg){height=60%}

---
title: 'Estructura del sistema de archivos'
author: Emilio Cabrera
institute: Laboratorio de Investigación y Desarrollo de Software Libre
logo: '../res/img/lidsol.png'
theme: PaloAlto
colortheme: spruce
navigation: horizontal
output:
  beamer_presentation:
    slide_level: 2
---
