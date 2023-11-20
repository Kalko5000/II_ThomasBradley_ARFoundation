# Interfaces Inteligentes - Practica 07: II_ThomasBradley_ARFoundation 

- Autor: Thomas Edward Bradley  
- Fecha: 20/11/23  

## Resumen  
Siguiendo [esta](https://codelabs.developers.google.com/arcore-unity-ar-foundation#0) guía podemos configurar un proyecto AR dentro de unity, el cual consiste en un coche que recoge paquetes sobre un terreno. 
Una vez completado el funcionamiento basico tenemos que llevar a cabo ciertas modificaciones sobre el proyecto.      

## Ejemplo de Ejecución

## Tarea 01  
![tarea_01](./img/II_Exam01_img01.jpg)  
***Scripts:*** PackageSpawner.cs  
  
Primero agregué un canvas y le añadi texto (con fuente descargada de la Unity Asset Store, y valor del texto por defecto a '0'). Tras jugar un poco con esto y posicionarlo de tal manera que se muestre apropiadamente en mi movil 
empecé a modificar el script 'PackageSpawner.cs'. Le añadi un atributo privado int count (inicializado a -1) y un objeto publico de tipo Text llamado score (al cual le pasamos el texto en el canvas), debemos incluir las librerias 
necesarias para que funcione. Ahora cuando se inserta un nuevo paquete en la escena incrementamos count y actualizamos el texto (texto por defecto en 0 y count por defecto a -1, de este modo no se detecta el primer paquete en aparecer
y el jugador no nota lo que esta pasando).  

## Tarea 02  
![tarea_02](./gif/II_Exam01_gif02.gif)   
***Scripts:*** -  
  
E 