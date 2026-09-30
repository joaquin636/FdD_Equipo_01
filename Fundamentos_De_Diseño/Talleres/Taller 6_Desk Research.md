# Desk Research
## Chaleco inteligente para asistencia en la movilidad de personas con discapacidad visual


## I. Definir el problema técnico

Las personas con discapacidad visual pueden enfrentar dificultades para identificar oportunamente obstáculos durante sus desplazamientos, especialmente cuando estos se encuentran en diferentes direcciones o alturas. Para nuestro proyecto, el problema se centra en obtener información sobre la ubicación y proximidad de los obstáculos y comunicarla de manera comprensible para el usuario.

La relevancia de esta problemática se sustenta en los antecedentes del informe. Los Censos Nacionales 2017 registraron 3 051 612 personas con alguna discapacidad en el Perú [1]. A escala mundial, la OMS estima que al menos 2 200 millones de personas presentan deterioro de la visión cercana o lejana [2]. Asimismo, un metaanálisis de 35 estudios estimó una prevalencia global agrupada de caídas de 17,7 % en personas con baja visión [3]. Este último dato corresponde a estudios internacionales y no representa una tasa específica del Perú.

**Problema técnico:**

Detectar obstáculos en diferentes sectores del entorno inmediato, estimar su ubicación y proximidad y transformar esa información en alertas hápticas interpretables, sin generar una carga excesiva para el usuario.

El chaleco se plantea como una ayuda complementaria a las estrategias de orientación y a las ayudas de movilidad existentes.

## II. Delimitar el foco de búsqueda

La búsqueda se organiza en cinco subtemas:

| N.º | Subtema | Información que se busca |
|---|---|---|
| 1 | Detección de obstáculos | Principios de detección, alcance, cobertura frontal y lateral y limitaciones de las tecnologías existentes. |
| 2 | Estimación de proximidad y dirección | Métodos para obtener información sobre distancia y sector de ubicación del obstáculo. |
| 3 | Comunicación háptica | Patrones de vibración para representar dirección y proximidad sin sobrecargar al usuario. |
| 4 | Integración corporal y energía | Configuraciones portátiles, ubicación de módulos, fijación y necesidades de alimentación. |
| 5 | Control y comunicación del estado | Procesamiento de mediciones, generación de alertas e información sobre el funcionamiento del sistema. |

Se consideran fuentes institucionales, productos comerciales, patentes, artículos científicos y tesis de repositorios. La información se analiza según su aporte funcional y sus limitaciones para el chaleco.

## III. Identificar el estado de la tecnología

### 3.1. Productos comerciales

WeWALK Smart Cane 2 integra detección de obstáculos y herramientas de navegación en un bastón [6]. NOA utiliza una configuración corporal sobre los hombros y cámaras para percibir el entorno [7]. Glide incorpora percepción y asistencia sobre la dirección del desplazamiento [8].

Estos productos permiten distinguir diferentes estrategias: comunicar información para que el usuario decida, integrar la detección en un dispositivo corporal o intervenir físicamente en el desplazamiento. Nuestro proyecto prioriza comunicar información mediante alertas hápticas.

### 3.2. Patentes

La patente CN215607427U presenta una mochila con detección de distancia y respuesta vibratoria [9]. CN210091198U describe un sistema de asistencia con detección distribuida mediante dispositivos portátiles, entre ellos un chaleco [10]. WO2023151351A1 plantea una guía háptica con percepción del entorno y actuadores distribuidos en el cuerpo [11].

Estos antecedentes orientan la distribución corporal de los elementos de detección y la transformación de información espacial en señales táctiles. La descripción de una patente no demuestra por sí sola el desempeño de nuestro prototipo.

### 3.3. Artículos científicos y tesis

Shen et al. desarrollaron un dispositivo con detección de objetos y presentación táctil. Reportaron 96 % de precisión para reconocer la posición izquierda o derecha de un obstáculo estacionario en sus condiciones experimentales [4].

Van Erp et al. estudiaron la representación de dirección, distancia y altura mediante una banda vibrotáctil. Identificaron que combinar demasiados parámetros puede generar sobrecarga informativa [12].

Las tesis revisadas incluyen detección ultrasónica, integración de localización y dispositivos corporales con respuestas táctiles y auditivas [13-15]. Constituyen antecedentes para comparar principios de funcionamiento, sin asumir que sus resultados se reproducirán automáticamente en el chaleco.

### 3.4. Síntesis

La arquitectura funcional común consiste en captar información del entorno, procesarla y comunicarla mediante estímulos no visuales. Para nuestro proyecto se priorizan:

- Detectar obstáculos en sectores frontal, izquierdo y derecho.
- Estimar su proximidad.
- Comunicar dirección y proximidad mediante patrones hápticos simples.
- Mantener sujetos y protegidos los componentes.
- Suministrar energía a las funciones principales.
- Gestionar mediciones inválidas e informar el estado del sistema.

## IV. Elaborar la matriz de Desk Research

### 4.1. Fuentes institucionales y contexto del problema

| N.º | Fuente | Autor/Institución | Año | Referencia | Estado de tecnología encontrado | Exigencia o requisito identificado | Restricción o limitación | Función principal | Aplicación al proyecto |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Perfil sociodemográfico del Perú: Censos Nacionales 2017 | INEI | 2018 | [1] | Aporta información sobre discapacidad en el Perú; no describe una tecnología. | Delimitar la población y justificar la relevancia del problema. | Los datos corresponden al censo de 2017 y no describen necesidades individuales de uso. | Sustentar el contexto del proyecto. | Utilizar los datos como antecedente nacional, diferenciando población con discapacidad y población con dificultad para ver. |
| 2 | Discapacidad visual y ceguera | OMS | s. f. | [2] | Presenta información mundial sobre discapacidad visual; no evalúa el chaleco. | Considerar las necesidades de movilidad y la diversidad de condiciones visuales. | Las cifras globales no representan directamente la situación local. | Orientar el propósito de asistencia. | Plantear el chaleco como apoyo complementario para la movilidad. |
| 3 | Objetivos de Desarrollo Sostenible | Naciones Unidas | s. f. | [5] | Proporciona un marco de inclusión y accesibilidad; no establece especificaciones técnicas del dispositivo. | Relacionar el proyecto con la reducción de barreras y la accesibilidad. | La relación con los ODS no demuestra un impacto social ya alcanzado. | Orientar la finalidad social del proyecto. | Vincular la propuesta con el ODS 10 y, de manera complementaria, con el ODS 11. |

### 4.2. Productos comerciales

| N.º | Fuente | Autor/Institución | Año | Referencia | Estado de tecnología encontrado | Exigencia o requisito identificado | Restricción o limitación | Función principal | Aplicación al proyecto |
|---|---|---|---|---|---|---|---|---|---|
| 4 | WeWALK Smart Cane 2 | WeWALK | s. f. | [6] | Integra detección de obstáculos y herramientas de navegación en un bastón. | Comunicar información útil durante el desplazamiento. | Su configuración en bastón difiere de una prenda corporal. | Detectar obstáculos y asistir la navegación. | Comparar la integración de funciones y plantear el chaleco como complemento de las ayudas habituales. |
| 5 | NOA: manual de usuario | biped robotics | 2024 | [7] | Utiliza cámaras en un dispositivo corporal colocado sobre los hombros. | Distribuir la percepción del entorno sin ocupar las manos del usuario. | Su arquitectura y procesamiento no pueden trasladarse directamente al prototipo. | Percibir el entorno y comunicar información. | Estudiar la ubicación corporal de los módulos y su cobertura. |
| 6 | Glide | Glidance | s. f. | [8] | Combina percepción del entorno con asistencia sobre la dirección del desplazamiento. | Definir si el sistema comunica información o interviene en la trayectoria. | Su mecanismo de guía física difiere del funcionamiento previsto del chaleco. | Asistir la dirección del desplazamiento. | Delimitar el alcance del chaleco hacia la emisión de alertas para que el usuario decida. |

### 4.3. Patentes

| N.º | Fuente | Autor/Institución | Año | Referencia | Estado de tecnología encontrado | Exigencia o requisito identificado | Restricción o limitación | Función principal | Aplicación al proyecto |
|---|---|---|---|---|---|---|---|---|---|
| 7 | Patente CN215607427U | Guangzhou Heijia Tech Co Ltd | 2022 | [9] | Describe una mochila de navegación con detección de distancia y respuesta vibratoria. | Transformar la proximidad detectada en una advertencia háptica. | La configuración de mochila difiere del chaleco; la patente no valida nuestro desempeño. | Detectar proximidad y emitir vibraciones. | Relacionar la medición de distancia con niveles de alerta. |
| 8 | Patente CN210091198U | East China Normal University | 2020 | [10] | Describe detección distribuida mediante dispositivos portátiles, incluido un chaleco. | Captar información en diferentes sectores del entorno. | La integración de múltiples tecnologías puede aumentar la complejidad del sistema. | Obtener información distribuida del entorno. | Evaluar la distribución frontal y lateral de los módulos. |
| 9 | Patente WO2023151351A1 | AI Guided Ltd | 2023 | [11] | Combina percepción del entorno, planificación de trayectoria y actuadores hápticos corporales. | Comunicar información direccional mediante distintas zonas de activación. | La planificación de trayectorias excede el alcance inicial del chaleco. | Transmitir indicaciones mediante estímulos hápticos. | Diseñar una correspondencia entre sector detectado y zona de vibración. |

### 4.4. Investigaciones científicas

| N.º | Fuente | Autor/Institución | Año | Referencia | Estado de tecnología encontrado | Exigencia o requisito identificado | Restricción o limitación | Función principal | Aplicación al proyecto |
|---|---|---|---|---|---|---|---|---|---|
| 10 | Metaanálisis sobre caídas en personas con baja visión | Ekemiri K et al. | 2024 | [3] | Aporta evidencia sobre caídas; no presenta un dispositivo de detección. | Considerar la seguridad durante la movilidad como parte del problema. | La prevalencia global no es una tasa del Perú ni demuestra que el chaleco reduzca caídas. | Sustentar la relevancia del problema. | Justificar el estudio de información oportuna sobre obstáculos sin prometer una reducción de accidentes no comprobada. |
| 11 | Dispositivo wearable con detección de objetos y presentación táctil | Shen J, Chen Y, Sawada H | 2022 | [4] | Combina detección en tiempo real y presentación táctil; reporta 96 % de precisión para reconocer izquierda o derecha en obstáculos estacionarios. | Comunicar el sector del obstáculo mediante señales táctiles interpretables. | El resultado corresponde a las condiciones experimentales del estudio. | Detectar objetos y comunicar su posición. | Evaluar el reconocimiento de alertas para izquierda, frente y derecha. |
| 12 | Codificación de obstáculos mediante una banda vibrotáctil | van Erp JBF, Kroon LCM, Mioch T, Paul KI | 2017 | [12] | Estudia la representación de dirección, distancia y altura mediante vibraciones. | Limitar la cantidad de información simultánea y utilizar patrones diferenciables. | La combinación de varios parámetros puede producir sobrecarga informativa. | Codificar información espacial mediante vibraciones. | Priorizar tres sectores y dos niveles de proximidad, verificando su interpretación. |

### 4.5. Tesis de repositorios

| N.º | Fuente | Autor/Institución | Año | Referencia | Estado de tecnología encontrado | Exigencia o requisito identificado | Restricción o limitación | Función principal | Aplicación al proyecto |
|---|---|---|---|---|---|---|---|---|---|
| 13 | Dispositivo basado en ultrasonido para el desplazamiento | Parra Farfán M / PUCP | 2014 | [13] | Presenta detección ultrasónica y reporta un alcance aproximado de 2,50 m. | Definir y comprobar el rango de detección del prototipo. | El alcance reportado depende del dispositivo y de sus condiciones de ensayo. | Detectar obstáculos mediante ultrasonido. | Utilizar el antecedente para orientar la meta de detección y realizar ensayos propios. |
| 14 | Bastón sensorial geolocalizador | Fernandez Llontop RJ / USAT | 2021 | [14] | Integra detección de obstáculos y ubicación en un bastón. | Integrar funciones complementarias sin afectar la detección y las alertas. | La configuración física y el contexto de uso difieren del chaleco. | Detectar obstáculos y obtener ubicación. | Comparar la integración funcional y delimitar las funciones prioritarias del prototipo. |
| 15 | Prototipo de ubicación espacial mediante IoT | Cayambe Gamarra FA / UPS | 2025 | [15] | Presenta un dispositivo corporal con sensores de proximidad, localización y respuestas táctiles y auditivas. | Transformar información espacial en señales perceptibles. | Su arquitectura y resultados requieren evaluación antes de adaptarlos al proyecto. | Captar información espacial y comunicar alertas. | Analizar la integración corporal y priorizar las señales hápticas. |

## Referencias bibliográficas

1. Instituto Nacional de Estadística e Informática. Perfil sociodemográfico del Perú: Censos Nacionales 2017. Lima: INEI; 2018.

2. Organización Mundial de la Salud. Discapacidad visual y ceguera [Internet]. Ginebra: OMS; [citado 29 sep 2026]. Disponible en: https://www.who.int/es/news-room/fact-sheets/detail/blindness-and-visual-impairment

3. Ekemiri K, Ekemiri C, Ezinne N, Virginia V, Okoendo O, Seemongal-Dass R, et al. Global burden of fall and associated factors among individual with low vision: a systematic-review and meta-analysis. PLoS One. 2024;19(7):e0302428. doi:10.1371/journal.pone.0302428.

4. Shen J, Chen Y, Sawada H. A wearable assistive device for blind pedestrians using real-time object detection and tactile presentation. Sensors (Basel). 2022;22(12):4537. doi:10.3390/s22124537.

5. Naciones Unidas. Objetivos de Desarrollo Sostenible: Objetivo 10 y Objetivo 11 [Internet]. Nueva York: Naciones Unidas; [citado 29 sep 2026]. Disponible en: https://www.un.org/sustainabledevelopment/es/sustainable-development-goals/

6. WeWALK. Smart Cane 2 [Internet]. [citado 29 sep 2026]. Disponible en: https://wewalk.io/en/product/

7. biped robotics. NOA by biped: user manual [Internet]. Versión 2024.7. [citado 29 sep 2026]. Disponible en: https://www.biped.ai/en/user-manual/

8. Glidance. Glide: intelligent guide aid [Internet]. [citado 29 sep 2026]. Disponible en: https://www.glidance.io/

9. Guangzhou Heijia Tech Co Ltd. Mochila de navegación y evitación de obstáculos para personas ciegas. Patente CN215607427U. 25 ene 2022.

10. East China Normal University. Sistema inteligente de asistencia para personas con discapacidad visual basado en tecnología de detección heterogénea de múltiples fuentes distribuidas. Patente CN210091198U. 18 feb 2020.

11. AI Guided Ltd. Haptic guiding system. Patente WO2023151351A1. 17 ago 2023.

12. van Erp JBF, Kroon LCM, Mioch T, Paul KI. Obstacle detection display for visually impaired: coding of direction, distance, and height on a vibrotactile waist band. Front ICT. 2017;4:23. doi:10.3389/fict.2017.00023.

13. Parra Farfán M. Diseño de dispositivo basado en ultrasonido para desplazamiento de personas en condición de discapacidad visual [tesis de grado en Internet]. Lima: Pontificia Universidad Católica del Perú; 2014 [citado 29 sep 2026]. Disponible en: http://hdl.handle.net/20.500.12404/6041

14. Fernandez Llontop RJ. Bastón sensorial geolocalizador inteligente para apoyar en el desplazamiento de personas invidentes en la Organización Regional de Ciegos del Perú – Chiclayo [tesis de grado en Internet]. Chiclayo: Universidad Católica Santo Toribio de Mogrovejo; 2021 [citado 29 sep 2026]. Disponible en: https://hdl.handle.net/20.500.12423/3213

15. Cayambe Gamarra FA. Diseño e implementación de un prototipo de ubicación espacial para personas con discapacidad visual mediante IoT [tesis de grado en Internet]. Guayaquil: Universidad Politécnica Salesiana; 2025 [citado 29 sep 2026]. Disponible en: https://dspace.ups.edu.ec/handle/123456789/30245

## Enlaces de las fuentes

- **[1] INEI — publicación de los Censos Nacionales 2017:** https://censo2017.inei.gob.pe/inei-difunde-base-de-datos-de-los-censos-nacionales-2017-y-el-perfil-sociodemografico-del-peru/
- **[2] OMS — discapacidad visual y ceguera:** https://www.who.int/es/news-room/fact-sheets/detail/blindness-and-visual-impairment
- **[3] Metaanálisis sobre caídas:** https://doi.org/10.1371/journal.pone.0302428
- **[4] Dispositivo wearable con presentación táctil:** https://doi.org/10.3390/s22124537
- **[5] Objetivos de Desarrollo Sostenible:** https://www.un.org/sustainabledevelopment/es/sustainable-development-goals/
- **[6] WeWALK Smart Cane 2:** https://wewalk.io/en/product/
- **[7] NOA — manual de usuario:** https://www.biped.ai/en/user-manual/
- **[8] Glide:** https://www.glidance.io/
- **[9] Patente CN215607427U:** https://patents.google.com/patent/CN215607427U/en
- **[10] Patente CN210091198U:** https://patents.google.com/patent/CN210091198U/en
- **[11] Patente WO2023151351A1:** https://patents.google.com/patent/WO2023151351A1/en
- **[12] Banda vibrotáctil:** https://doi.org/10.3389/fict.2017.00023
- **[13] Tesis PUCP:** http://hdl.handle.net/20.500.12404/6041
- **[14] Tesis USAT:** https://hdl.handle.net/20.500.12423/3213
- **[15] Tesis UPS:** https://dspace.ups.edu.ec/handle/123456789/30245
