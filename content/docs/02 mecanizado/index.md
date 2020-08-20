---
title: '02 Mecanizado CNC'
date: 2020-06-17T19:30:08+10:00
draft: false
weight: 2
summary: Simulación en Fusion 360.
---
## Router CNC
Es una herramienta de control automatizado que que posee 3 ejes con motores de precisión con un cabezal que permite desbastar, cortar y grabar en el material de trabajo a través de una broca revolucionada. La utilización de estas máquinas asegura consistencia  y calidad en un proceso fácilmente automatizable. 

CNC es la sigla para Control Numérico Computarizado. 
![Imagen Simple](/img/cnc.jpg)


## Simulación de Corte en FUSION 360
![Imagen Simple](/img/silla.PNG)

A continuación se evidencia la simulación de corte en el software Fusion 360 de una silla de madera. El material base fue una plancha de terciado de 15mm de grosor y de 1220mm X 1220mm de dimensión. Para el corte se separan todas las piezas de la silla en la tabla y se proyecta el recorrido de la fresa. Se realizó con un cortador de **6mm  L22.5 mm** de tipo **Flat End Mill**
![Imagen Simple](/img/broca.jpg)

---

###### Piezas en la Tabla de Terciado
Se ubican las piezas y componentes de la silla de manera que quepan todas.

Piezas a recortar de la Tabla:
1. Patas Frontales (A y B)
2. Patas Posteriores (A y B)
3. Larguero (x2)
4. Travesaños (x2)
![Imagen Simple](/img/tablas.jpg)

###### Corte 2D Contour (Encastres)
La fresadora corta los pequeños encastres necesarios para luego poner en su lugar los travesaños y largueros. Se hace cortando en el eje Z con profundidades de 3mm, la mitad del largo de la broca.
![Imagen Simple](/img/cont.jpg)
{{< video-local src="contour1.mp4" >}}

###### 2D Pocket (Ensambles)
Se desbasta el material en capas de 3mm, nuevamente. Se hace a lo largo de toda la cara con el objetivo de dejar una pieza de ensamble.
![Imagen Simple](/img/pocket.jpg)
{{< video-local src="pocekt.mp4" >}}

###### 2D Contour (Exterior)
En este proceso se recorta el contorno de la pieza. Aquí se repite un proceso parecido al de los encastres, con la diferencia de que se dejan unos espacios llamados **Tabs** para sostener la pieza mientras se recorta. 
![Imagen Simple](/img/cont2.jpg)
{{< video-local src="contour2.mp4" >}}

###### Pieza Resultante
![Imagen Simple](/img/final.jpg)

---

#### Asiento y Respaldo
En la imagen a continuación se ven los recorridos que hace la fresadora para cortar el asiento. Esta no hace un corte en esos trazados, desbasta la mitad del grosor del material (4,5 mm) para que este pueda moldearse posteriormente. 

![Imagen Simple](/img/asiento.jpg)
{{< video-local src="asiento.mp4" >}}

Para el respaldo se tuvo que alargar la fresa para evitar que colisione con la tabla de madera. EL nuevo largo de la broca es de 40 mm. El contorno morado que se ve en las próximas imágenes es un límite de selección para que la máquina no tenga que cortar espacios inservibles. 
![Imagen Simple](/img/fresa2.jpg)

1. **Adaptive Clearing** 
En este paso se "limpia" la tabla desbastando material para que en los procedimientos posteriores la cortadora pueda moverse libremente y no colisione con los lugares de la tabla que no serán respaldo. En la imagen se ve el recorrido del router para hacer el desbaste.
![Imagen Simple](/img/res1.jpg)
{{< video-local src="adaptive.mp4" >}}

2. **Parallel (1)** 
El recorrido en este paso es hacia lo largo del respaldo. Cada tramo está separado a 2mm del siguiente.
![Imagen Simple](/img/res2.jpg)
{{< video-local src="parallel1.mp4" >}}

3. **Parallel (2)** 
Se giraron en 90° los trazados del paso anterior para cortar a lo ancho de la tabla. 
![Imagen Simple](/img/res3.jpg)
{{< video-local src="parallel2.mp4" >}}