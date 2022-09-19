
## [Ver presentacion del proyecto](https://impresora3d-akv.my.canva.site/)

# Impresora 3D Cube

##  Introducción

Esta impresora estará pensada para imprimir diferentes tipos de materiales y darle upgrades proporcional con los elementos que se consiguen en argentina. A su vez esta impresora estará desarrollada sin comprar elementos en el extranjero por la actual situación en las importaciones.

## Elementos que se tienen en cuenta

Estructura:
Chasis en aluminio de 5mm para el eje X e Y. Y para el eje Z aluminio de 3mm (Panelado en aluminio)

__Dimensiones de impresión útiles:__

Eje X – 310mm

Eje Y – 310mm

Eje Z – 400mm (Se puede expandir asta 500mm)

__Dimensiones exteriores:__

Alto - 700mm

Ancho - 580mm

Profundidad - 580mm

## Objetivos
1.	Desarrollo y montaje de la impresora
2.	Configurar firmware (Marlin o RepRap firmware)
3.	Cerramiento y upgrade para impresiones más estables
4.	Lograr la aplicación de los diferentes conocimientos adquiridos durante el año.
5.	Conseguir la funcionalidad completa de la impresora.
6.	Aprender nuevos conocimientos de programación en G-Code durante su creación.
7.	Integrar conocimientos sobre mecánica y electrónica.


## Características que llevaron a la decision para el diseño

Realizar ina impresora 3D que cumpla con todos los criterios siguientes:

- Volumen de impresión entre 30 cms y 30 cms
    - Más grande que esto podría causar problemas de rigidez en el marco
    - Más pequeño es demasiada la inversión
- Marco construido de chapa plegada o aluminio (Esto se puede realizar en cualquier pais)
- Máxima visibilidad de las piezas imprimiéndose
- Extrusor directo
- Evitar el uso de perfiles estructurales 2020
- Electrónica libre (No se utiliza una placa especifica)
- Motores Nema17
- Guiás de precisión mecanizadas MGN12 (Para eje X e Y. Eje Z Se puede utilizar gias lineales)
- Sensor de autonivel
- Fleje flexible para la correcta extracción de la bandeja de impresión
- Fuente de alimentación 24V 20A
- Base caliente a 24V (Temperatura máxima 110º-120º)
- Pueta de acrilico

## Características por decidir en el diseño

- Electrónica
    - BTT Octopus
        - Placa de 128 bits destinada a trabajos de alta demanda
    - o	Pantalla TFT BTT
        - Pantalla TFT
- Movimiento lineal
    - 4 Barras lisas de 8mm (son los más baratos)
    - 3 Rieles lineales MGN12
- Bushings/cojinetes
    - Pueden ser impresos en 3d
        - Posiblemente lo mejor sea diseñar los _bushings_ completos para que se puedan sustituir
        - Hay que investigar si es conveniente utilizar bushings de 1 perímetro para que sean más flexibles y adaptables. Pero hay que ver si no se pierde mucha rigidez
    - Comprados
        - Lmk8uu 8mm baratos chinos
            - Son ruidosos y hay que estarlos lubricando
        - Bushings de bronce/polímero autolubricante
            - Son muy caros y su instalación requiere tolerancias muy exactas
        - Carro MGN12H
            - Son caros pero precisos
        - Extrusor Hotend Bmg o Bracket Hotend
        - Correa 4m
    -

## Caracteristicas de las impresoras 3D

<div align="left"><img src="/Imagenes/IMPRESORAS_3D.png"></div>

![IMPRESORAS_3D.png](https://github.com/AlessandroKlein/Impresora-3D/raw/main/Imagenes/IMPRESORAS_3D.png)

