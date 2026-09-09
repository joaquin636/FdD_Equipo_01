# LISTA DE EXIGENCIAS

**Edición:** 01

**PROYECTO:** Diseño y desarrollo de chaleco inteligente

**Fecha:** 31 Agosto 2026

**CLIENTE:** Personas con discapacidad visual

**Elaborado:** Equipo 1

**Revisado:** …......

---

## LEYENDA

| Letra | Nombre |
|:---:|---|
| D | Daniela |
| Y | Yanella |
| S | Sharlene |
| M | Manuel |
| J | Joaquin |

---

## LISTA DE EXIGENCIAS

| Fecha (cambios) | Deseo o Exigencia | DESCRIPCIÓN | Responsable |
|---|---|---|:---:|
| 9/9/26 | E | **FUNCIÓN PRINCIPAL:** Detectar obstáculos y situaciones de riesgo, estimar su proximidad y dirección y comunicar alertas al usuario y a la plataforma digital para favorecer un desplazamiento más seguro y autónomo. [1], [3], [4], [5] | **TODOS** |
| 9/9/26 | E | **GEOMETRÍA:** El dispositivo debe ser compacto y adaptable, permitiendo su colocación en diferentes prendas mediante un sistema de sujeción. | **Y** |
|  | E | Los sensores deben cubrir principalmente las zonas frontal, izquierda y derecha de la trayectoria del usuario. | **J** |
|  | D | Su diseño debe ser discreto, ligero y apropiado para el uso cotidiano. [3], [4] | **Y** |
| 9/9/26 | E | **CINEMÁTICA:** El sistema debe realizar mediciones continuamente mientras el usuario se desplaza. Las alertas deben actualizarse según los cambios en la distancia de los obstáculos y el movimiento del usuario. [2], [3] | **J** |
| 9/9/26 | E | **FUERZAS:** El chaleco y sus componentes deben soportar movimientos cotidianos como caminar, sentarse y levantarse, manteniendo los componentes firmemente sujetos. | **M** |
| 9/9/26 | E | **MATERIA:** *Entrada:* Entorno del usuario, distancias de obstáculos y datos de movimiento. | **S** |
|  | | *Salida:* Información procesada, alertas auditivas y, ante un posible incidente, información para el contacto responsable. [1], [3], [4], [5] | **M** |
| 9/9/26 | E | **ENERGÍA:** Utilizar una batería portátil, recargable y de bajo consumo que permita el funcionamiento durante una jornada de uso razonable. [2] | **J** |
| 9/9/26 |  | **SEÑALES:** Entradas: Señal de encendido y apagado, señales de los sensores de distancia e IMU. | **J** |
|  | E | Salidas: Detección, dirección, proximidad, alertas auditivas y estado del sistema. | **D** |
|  | E | Las señales de alerta deben aumentar su intensidad o frecuencia cuando el obstáculo se encuentre más próximo, según la configuración definida. [2], [3] | **D** |
| 9/9/26 | E | **CONTROL:** El sistema debe procesar la información de los sensores mediante un microcontrolador y controlar las alertas según el nivel de riesgo detectado. También debe analizar el movimiento posterior a un posible incidente. [2], [3], [4] | **J** |
| 9/9/26 | E | **ELECTRONICA (Hardware):** El sistema sera contralado por un ESP32 DevKit V1 con la intencion de poder enviar datos por vía Wi-fi o Bluethoot a algun dispositivo, como fuentes base del proyecto se usaran los sensores HC-SR04 (medidor de proximidad), VL53L1X (mide desniveles, escalones o peldaños), MPU6050 (Detecta movimientops bruscos como caidas o choques); estos sensores tendran como finalidad prevenir caidas y brindar un mayor apoyo a personas con discapacidad | **J** |
|  |  | [2], [3], [4] |  |
|  |  | **SOFTWARE:** Para el trabajo en conjunto de los sensores y el ESP32 DevKit V1 se plantea usar al plataforma ARDUINO IDE usando como lenguaje C++ | **S** |
|  |  | La información extraida de los sensores se debera mandar hacia una pagina web o aplicacion en donde se almacenaran, y se podra realizar un monitoreo a el usuario que la este portando () |  |
|  |  | Debe reducir alertas innecesarias y detectar patrones asociados a posibles caídas. [1], [2], [3], [4], [5] | **D** |
|  |  | **COMUNICACIONES:** Permitir la comunicación inalámbrica entre el módulo, el teléfono inteligente y el auricular para transmitir alertas y enviar información de posibles emergencias al contacto responsable. [2], [4] | **M** |
| 9/9/26 | E | **SEGURIDAD:** No debe representar riesgos físicos o eléctricos para el usuario. Los componentes deben estar protegidos y correctamente aislados. | **S** |
| 9/9/26 | E | **ERGONOMÍA:** El dispositivo debe ser ligero, cómodo y fácil de colocar y retirar. El sistema de sujeción debe adaptarse a diferentes usuarios y prendas sin limitar el movimiento ni generar molestias durante el desplazamiento. [4], [5] | **Y** |
| 9/9/26 | E | **FABRICACIÓN:** El sistema debe incorporar componentes y estructuras fabricadas mediante impresión 3D cuando corresponda, utilizando un máximo de 1 kg de filamento. | **M** |
| 9/9/26 | E | **CONTROL DE CALIDAD:** Realizar pruebas de sensores, alertas, comunicación, detección de posibles caídas, alimentación, autonomía y resistencia del ensamblaje. [1], [2], [3], [4] | **S** |
| 9/9/26 | E | **MONTAJE:** Los sensores, vibradores, batería y demás componentes deben quedar firmemente sujetos y protegidos dentro del módulo.. | **M** |
| 9/9/26 | E | **TRANSPORTE:** El chaleco debe ser compacto y fácil de transportar, protegiendo sus componentes electrónicos durante el traslado. [4], [5] | **S** |
| 9/9/26 | E | **USO:** Debe poder colocarse y retirarse fácilmente, permitiendo el uso cotidiano mientras el usuario recibe alertas mediante un auricular abierto. [4], [5] | **Y** |
| 9/9/26 | E | **MANTEMINIEMTO:** El diseño debe permitir acceder a los sensores, batería y componentes electrónicos para realizar mantenimiento o reemplazos sin desmontar completamente el dispositivo. | **M** |
| 9/9/26 | E | **COSTOS:** Mantener una relación adecuada entre funcionalidad, calidad y costo, priorizando componentes accesibles sin comprometer la seguridad ni el funcionamiento. [2] | **D** |
| 9/9/26 | E | **PLAZOS:** El proyecto inició el miércoles 19 de agosto de 2026 y se espera su finalización durante el mes de diciembre de 2026. | **J** |

## Referencias bibliográficas

1. Ji H, Mendonça I, Aritsugi M. Multi-Scene Dataset and Object Detector for Outside Blind Individual Identification. *IEEE Access* [Internet]. 2026 [citado 2026]; 14: 1423-1438. Disponible en:
   https://ieeexplore.ieee.org/document/11317963

2. Alfikri MD, Kaliski R. Real-Time Pedestrian Detection on IoT Edge Devices: A Lightweight Deep Learning Approach. *arXiv* [Internet]. 2024 [citado 2025]. Disponible en:
   https://arxiv.org/abs/2409.15740

3. Leong X, Kanesaraj Ramasamy R. Obstacle Detection and Distance Estimation for Visually Impaired People. *IEEE Access* [Internet]. 2023 [citado 2025]; 11: 136609-136629. Disponible en:
   https://ieeexplore.ieee.org/document/10336791

4. Balboa Trigo PA. Sistema de asistencia para personas con discapacidad visual basado en visión por computadora [tesis]. Centro de Investigación Científica y de Educación Superior de Ensenada [Internet]. 2020 [citado 2026]. Disponible en:
   https://cicese.repositorioinstitucional.mx/jspui/bitstream/1007/3362/1/Tesis_Pablo%20Alberto%20Balboa%20Trigo_20%20nov%202020.pdf

5. Hamzeh Alashhab SR. Aplicaciones de visión artificial para ayuda a personas con dificultades visuales [tesis doctoral]. Universidad de Alicante [Internet]. 2022 [citado 2026]. Disponible en:
   https://rua.ua.es/entities/publication/162679e1-c5dd-4986-ba1e-3bfc306f8c11
