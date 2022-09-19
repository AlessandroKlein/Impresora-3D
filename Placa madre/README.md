## Conectores

<div align="middle"><img src="/Placa madre/Imagenes/1.png"></div>

## Pines 

<div align="middle"><img src="/Placa madre/Imagenes/2.png"></div>

## Dimensiones generales

<div align="middle"><img src="/Placa madre/Imagenes/3.png"></div>



## Principales características

<div align="middle"><img src="/Placa madre/Imagenes/4.png"></div>

### Las características más importantes que podríamos destacar sobre las nuevas BTT Octopus Pro son las siguientes:

- Dos versiones disponibles de MCUs
- MCU de 32b ARM Cortex-M4 STM32F446ZET6 con una frecuencia de reloj de 180MHz y 512k de memoria flash, siendo esta versión la más aconsejable para firmwares Klipper o Marlin
- MCU de 32b ARM Cortex-M4 STM32F429ZGT6 con una frecuencia de reloj de 168Mhz y 1MB de memoria flash, siendo esta versión la más aconsejable para firmwares RRF
- Soporte directo para 3 tipos de firmwares disponibles: Klipper, Marlin y RRF
- Interface para Raspberry Pi tanto por USB como UART (por GPIO)
- Hasta 4 hotends disponibles
- Hasta 8 drivers de alto voltaje o normales con nueva electrónica de protección
- Alimentación independiente para motores, cama caliente y electrónica
- DCDC integrados para proveer alimentación a 12V (4A), 5V (8A) y 3.3V (1A). Ideal para no precisar componentes externos
- Hasta 6 ventiladores controlables y 2 sin control, con la posibilidad de selección del voltaje de trabajo entre Vin, 12V y 5V.
- Protección ante cortos en las tomas de ventiladores, importante por una mala manipulación o fallo de estos componentes ya que es uno de los problemas más comunes con las placas de nuestras máquinas
- Conector USB-C que permite la emulación serie para poder imprimir mediante USB
- Compatibilidad con casi cualquier pantalla aunque aconsejable siempre usar las estupendas pantallas duales de SKR
- MOSFETs de alto rendimiento que mejoran la eficiencia y velocidad de calentado de los calentadores
- Fusibles de protección reemplazables de forma sencilla
- Doble salida de motor para el eje Z
- Mejoras en bootloader, soportando la actualización por USB (aconsejable) y DFU (usuarios avanzados)
- EEPROM de 32K (AT24C32)
- Conectores para leds RGB y Neopixel
- Conector para interfaz WiFi (ESP8266)
- PT100 interface/amplificador instalado soportando sensores de 2/3/4 cables
- Protección ante corto en los conectores de termistores, otra gran mejora también aplicada a los ventiladores. Permite reusar estos pines para otras tareas con un pin que hace bypass de estas protecciones
- Soporte de BLTouch/3DTouch y similares con un conector destinado para ellos y usable por otros sistemas ABL. El puerto del PROBE se añadió protección extra con un optoacoplador para no necesitar usar un diodo BAT85
- CAN BUS mediante conector 6P6C RJ11 para futuros módulos de expansión
- SPI BUS puerto de expansión para módulos SPI como el MAX31865
- I2C BUS puerto de expansión para módulos I2C
- Soporte para módulos Relé y UPS



<div align="middle"><img src="/Placa madre/Imagenes/5.png"></div>

Para empezar se ha añadido soporte para drivers de alto voltaje (HV), en concreto hasta 60V teóricos aunque aconsejamos trabajar con sistemas de 48V. Por supuesto podemos usar nuestra placa Octopus PRO con drivers estándar gracias a que BigTreeTech ha puesto a nuestra disposición un jumper para elegir un modo u otro.



## Soporta

<div align="middle"><img src="/Placa madre/Imagenes/6.png"></div>



## Coneccion para 24v

<div align="middle"><img src="/Placa madre/Imagenes/7.png"></div>

En el caso que usemos drivers normales colocaremos el jumper de la parte superior del zócalo (debajo del conector del cable del motor) en la parte derecha, en ese caso los drivers usarían la entrada de corriente MOTHERBOARD que normalmente es 24v.


## Coneccion para 60v

<div align="middle"><img src="/Placa madre/Imagenes/8.png"></div>

En el caso que usemos drivers HV colocaremos el jumper en la parte izquierda haciendo que la alimentación de nuestros drivers usen la entrada de corriente MOTOR POWER IN que podremos alcanzar hasta 60V.



## Sensores PT100/PT1000

<div align="middle"><img src="/Placa madre/Imagenes/9.png"></div>

La Octopus PRO incluye la electrónica necesaria para poder usar los excelentes sensores PT100, soportando sensores de 2, 3 y 4 cables usando un micro-switch para indicarle a la placa qué tipo estamos utilizando en cada momento.

Configuración de micro-switches dependiendo del tipo de sensor PT100 usado:

1	2	3	4	Sensor
ON	ON	ON	OFF	PT100 – 2 cables
ON	ON	OFF	ON	PT1000 – 2 cables
OFF	ON	ON	OFF	PT100 – 3 cables (*)
OFF	ON	OFF	ON	PT1000 – 3 cables (*)
OFF	OFF	ON	OFF	PT100 – 4 cables
OFF	OFF	OFF	ON	PT1000 – 4 cables
