# Interfaces Inteligentes - Practica 07: AR Foundation  

- Autor: Thomas Edward Bradley  
- Fecha: 20/11/23  

## Resumen  
Siguiendo [esta](https://codelabs.developers.google.com/arcore-unity-ar-foundation#0) guía podemos configurar un proyecto AR dentro de unity, el cual consiste en un coche que recoge paquetes sobre un terreno. 
Una vez completado el funcionamiento basico tenemos que llevar a cabo ciertas modificaciones sobre el proyecto.      

## Ejemplo de Ejecución

Funcionamiento normal:  
![Gif_01](./gif/Horizontal_AR_GIF.gif)  
Funcionamiento en superficie vertical:  
![Gif_02](./gif/Vertical_AR_GIF.gif)  

## Tarea 01  
***Scripts:*** PackageSpawner.cs  
  
Primero agregué un canvas y le añadi texto (con fuente descargada de la Unity Asset Store, y valor del texto por defecto a '0'). Tras jugar un poco con esto y posicionarlo de tal manera que se muestre apropiadamente en mi movil 
empecé a modificar el script 'PackageSpawner.cs'. Le añadi un atributo privado int count (inicializado a -1) y un objeto publico de tipo Text llamado score (al cual le pasamos el texto en el canvas), debemos incluir las librerias 
necesarias para que funcione. Ahora cuando se inserta un nuevo paquete en la escena incrementamos count y actualizamos el texto (texto por defecto en 0 y count por defecto a -1, de este modo no se detecta el primer paquete en aparecer
y el jugador no nota lo que esta pasando).  

## Tarea 02  
***Scripts:*** -  
  
No estuve muy seguro de lo que tenia que hacer en este apartado por lo que intente simular el juego original pero sobre una superficie vertical. Esto se puede modificar en 'AR Plane Manager' cambiando 
de 'Horizontal' a 'Everything' el cual nos suscribe a ambos planos. El resultado de esto se puede ver en el segundo GIF. 
