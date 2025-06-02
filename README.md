
# Rover VexRobot 

Proyecto de robótica autónoma desarrollado en el Instituto Tecnológico de Ensenada (ITE) como parte del curso de Ingeniería. El rover fue diseñado para realizar desplazamientos precisos en un circuito cerrado, utilizando encoders ópticos para navegación y un sensor BMP180 para la recolección de datos atmosféricos.

##  Descripción del Proyecto

El Rover VexRobot es un vehículo autónomo que navega un circuito prediseñado ejecutando movimientos lineales y giros con precisión milimétrica. El control se basa en cálculos físicos de distancia, revoluciones por pulso y ajustes dinámicos durante la marcha para corregir desviaciones.

##  Lógica y Programación

Todo el código fue implementado en **ROBOTC** utilizando programación estructurada con funciones modulares. El sistema se compone de:

- **Control por encoders** para medir distancia recorrida.
- **Algoritmo de corrección de trayectoria**, que compara pulsos de ambos motores para mantener dirección.
- **Funciones de avance y giros** (90°, 180°, etc.) calculadas en base a la circunferencia de la rueda.
- **Adaptación dinámica** según condiciones de fricción del terreno y estado de batería.
- **Módulo de espera para ejecución manual** desde control remoto.

##  Testing y Validación

Se realizaron pruebas experimentales con diferentes niveles de velocidad y carga de batería. Se documentaron desfases, márgenes de error y ajustes para mejorar precisión:

- **Precisión promedio en trayecto recto:** ±7%
- **Precisión promedio en giros:** 70–97% dependiendo del giro
- **Distancia objetivo alcanzada (1 metro):** error ≤ 7 cm

##  Hardware Utilizado

- Controlador VEX Cortex
- Motores VEX 393 (2 hilos)
- Encoders ópticos VEX
- Sensor BMP180 (implementado por un compañero)
- Estructura de aluminio (C-Canales, placas y ángulos)

##  Cálculos Implementados

- **Circunferencia de rueda:** 10.16 cm × π ≈ 31.91 cm  
- **Pulsos por revolución:** 360  
- **Distancia por pulso:** ≈ 0.08859 cm  
- **Ejemplo:** para recorrer 100 cm → 100 / 0.08859 ≈ 1128 pulsos

##  Integrantes del Proyecto

- Arias Hernández Mario de Jesús *(sensor BMP180 y análisis atmosférico)*
- Caballero Sánchez Rubén Abimael *(programación y control autónomo)*
- García Beltrán Estefanía *(documentación y estructura física)*
