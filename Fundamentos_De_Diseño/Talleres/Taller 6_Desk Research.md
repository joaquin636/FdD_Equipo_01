# Matriz de Desk Research: chaleco inteligente

**Proyecto:** Chaleco inteligente para apoyar la movilidad de personas con discapacidad visual.

## 1. Investigaciones científicas y desarrollos tecnológicos

| N.º | Fuente | Autor/Institución | Año | Referencia | Estado de tecnología encontrado | Exigencia o requisito identificado | Restricción o limitación | Función principal | Aplicación al proyecto |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Artículo sobre un sistema portátil de detección de obstáculos | Moncada Hernandez RH, Canaca Matamoros DM, Cáceres Lagos FL | 2025 | [16] | Presenta un dispositivo integrado en gafas que utiliza sensores de tiempo de vuelo y señales vibratorias para informar sobre obstáculos. | Detectar obstáculos y transmitir su proximidad mediante señales perceptibles para el usuario. | La ubicación de los sensores en gafas difiere de su instalación en un chaleco; se debe evaluar la cobertura a distintas alturas. | Detectar obstáculos y comunicar su proximidad. | Evaluar la distribución de sensores en la parte frontal del chaleco y establecer niveles de vibración según la distancia. |
| 2 | Artículo sobre señales hápticas y auditivas para la navegación | Skulimowski P, Strumiłło P, Trygar S | 2025 | [17] | Estudia la navegación mediante información de profundidad y señales hápticas y auditivas. | Comunicar la ubicación y distancia de los obstáculos mediante señales que puedan distinguirse durante el desplazamiento. | La interpretación de las señales requiere aprendizaje y evaluación con usuarios. | Transformar información del entorno en señales comprensibles. | Diseñar patrones de vibración sencillos para diferenciar obstáculos al frente, a la izquierda y a la derecha. |
| 3 | Prepublicación sobre el dispositivo GuideTouch | Kozlov T et al. | 2026 | [24] | Propone un dispositivo de asistencia con retroalimentación táctil distribuida en la parte superior del cuerpo. | Diferenciar la dirección de un obstáculo mediante la ubicación de la señal táctil. | Es una prepublicación; sus resultados no demuestran por sí solos una reducción de accidentes en el contexto del proyecto. | Comunicar la dirección de los obstáculos. | Evaluar la ubicación de actuadores en zonas del chaleco donde las vibraciones puedan distinguirse claramente. |
| 4 | Artículo sobre detección de caídas | Aziz O et al. | 2017 | [26] | Evalúa un algoritmo de detección de caídas mediante datos de sensores de movimiento y registros de caídas reales. | Evaluar la sensibilidad del sistema y la frecuencia de falsas alarmas si se incorpora la detección de caídas. | El desempeño depende de la posición del sensor, las actividades realizadas y las características de los usuarios. | Identificar eventos compatibles con una caída. | Considerar un sensor de movimiento como función complementaria y comprobar su desempeño antes de incorporarlo al diseño final. |
| 5 | Artículo sobre detección de obstáculos y estimación de distancia | Leong X, Kanesaraj Ramasamy R | 2023 | [27] | Aborda tecnologías de visión artificial para detectar obstáculos y estimar distancias en dispositivos de asistencia. | Comparar las alternativas según precisión, tiempo de respuesta, consumo energético y cobertura. | El procesamiento de imágenes requiere recursos computacionales y puede depender de las condiciones del entorno. | Percibir obstáculos y estimar su distancia. | Comparar la visión artificial con sensores ultrasónicos o infrarrojos para seleccionar una alternativa viable para el chaleco. |

## 2. Normas y documentos técnicos

| N.º | Fuente | Autor/Institución | Año | Referencia | Estado de tecnología encontrado | Exigencia o requisito identificado | Restricción o limitación | Función principal | Aplicación al proyecto |
|---|---|---|---|---|---|---|---|---|---|
| 6 | IEC 60529: grados de protección de envolventes | Comisión Electrotécnica Internacional — IEC | 2013 | [18] | Establece la clasificación IP para la protección de envolventes frente al ingreso de sólidos y agua. | Definir la protección requerida para los componentes según la exposición prevista a polvo y agua. | No se puede declarar un grado IP sin realizar los ensayos correspondientes. | Proteger los componentes electrónicos. | Diseñar cubiertas para sensores, batería y circuito de control, considerando las condiciones de uso del chaleco. |
| 7 | IEC 62133-2: seguridad de baterías portátiles de litio | Comisión Electrotécnica Internacional — IEC | 2021 | [19] | Establece requisitos de seguridad y ensayos para celdas y baterías secundarias portátiles de litio. | Incorporar medidas de protección y utilizar una batería y un sistema de carga adecuados. | Consultar la norma no demuestra la conformidad de la batería ni del prototipo completo. | Suministrar energía de manera segura. | Seleccionar la batería, proteger las conexiones y evaluar el calentamiento durante la carga y el funcionamiento. |
| 8 | ISO 9241-920: interacción táctil y háptica | Organización Internacional de Normalización — ISO | 2024 | [20] | Proporciona orientación ergonómica para las interacciones táctiles y hápticas. | Diseñar señales vibratorias perceptibles y diferenciables para los usuarios previstos. | No establece una intensidad universal adecuada para todas las personas; se requieren pruebas con usuarios. | Comunicar información mediante el tacto. | Evaluar la intensidad, duración y ubicación de las vibraciones, especialmente para adultos mayores. |
| 9 | Pautas de Accesibilidad para el Contenido Web, WCAG 2.2 | World Wide Web Consortium — W3C | 2024 | [21] | Establece criterios de accesibilidad para contenido e interfaces web. | Permitir el acceso mediante lectores de pantalla y teclado si el proyecto incorpora una interfaz web. | Su alcance corresponde al contenido web; no demuestra automáticamente la accesibilidad de una aplicación nativa o del chaleco. | Facilitar el acceso a información digital. | Aplicar los criterios pertinentes a una futura interfaz web de configuración o consulta del estado del dispositivo. |
| 10 | ISO 21856: requisitos generales y métodos de ensayo para productos de apoyo | Organización Internacional de Normalización — ISO | 2022 | [22] | Presenta requisitos y métodos de ensayo para productos de apoyo considerados dispositivos médicos. | Considerar riesgos de uso, información al usuario, mantenimiento y seguridad cuando resulte aplicable. | Su aplicabilidad depende de la clasificación del producto y del contexto regulatorio; no debe asumirse automáticamente. | Orientar la seguridad y evaluación del producto de apoyo. | Utilizarla como referencia para revisar riesgos, instrucciones de uso y mantenimiento del chaleco. |

## 3. Fuente institucional

| N.º | Fuente | Autor/Institución | Año | Referencia | Estado de tecnología encontrado | Exigencia o requisito identificado | Restricción o limitación | Función principal | Aplicación al proyecto |
|---|---|---|---|---|---|---|---|---|---|
| 11 | Información institucional sobre salud visual y pérdida de visión | Organización Mundial de la Salud — OMS | s. f. | [25] | Describe la discapacidad visual y la importancia de la rehabilitación y los productos de apoyo para la autonomía. | Complementar las ayudas de movilidad y considerar las necesidades de las personas con discapacidad visual. | La información institucional no valida el desempeño de un chaleco específico. | Apoyar la movilidad y autonomía del usuario. | Plantear el chaleco como una ayuda complementaria al bastón y priorizar señales que permitan mantener la percepción de los sonidos del entorno. |

**Nota:** Las aplicaciones al proyecto son propuestas de diseño derivadas del análisis de las fuentes. Su desempeño deberá comprobarse mediante pruebas del prototipo. La consulta de una norma no equivale a una certificación.

## Referencias bibliográficas — formato Vancouver

[16] Moncada Hernandez RH, Canaca Matamoros DM, Cáceres Lagos FL. Wearable obstacle detection system: enhancing indoor navigation for individuals with visual impairments. LACCEI. 2025;1(12). doi:10.18687/LACCEI2025.1.1.2028.

[17] Skulimowski P, Strumiłło P, Trygar S. Haptic and auditory cues: a study on independent navigation for visually impaired individuals. J Multimodal User Interfaces. 2025;19:363-373. doi:10.1007/s12193-025-00463-2.

[18] International Electrotechnical Commission. IEC 60529:1989+AMD1:1999+AMD2:2013 CSV. Degrees of protection provided by enclosures (IP Code) [Internet]. Geneva: IEC; 2013 [citado 29 sep 2026]. Disponible en: https://webstore.iec.ch/en/publication/2452

[19] International Electrotechnical Commission. IEC 62133-2:2017+AMD1:2021 CSV. Secondary cells and batteries containing alkaline or other non-acid electrolytes: safety requirements for portable sealed secondary cells, and for batteries made from them, for use in portable applications. Part 2: Lithium systems [Internet]. Geneva: IEC; 2021 [citado 29 sep 2026]. Disponible en: https://webstore.iec.ch/en/publication/70017

[20] International Organization for Standardization. ISO 9241-920:2024. Ergonomics of human-system interaction. Part 920: Tactile and haptic interactions [Internet]. Geneva: ISO; 2024 [citado 29 sep 2026]. Disponible en: https://www.iso.org/standard/80751.html

[21] World Wide Web Consortium. Web Content Accessibility Guidelines (WCAG) 2.2 [Internet]. W3C; 2024 [citado 29 sep 2026]. Disponible en: https://www.w3.org/TR/WCAG22/

[22] International Organization for Standardization. ISO 21856:2022. Assistive products: general requirements and test methods [Internet]. Geneva: ISO; 2022 [citado 29 sep 2026]. Disponible en: https://www.iso.org/standard/71986.html

[24] Kozlov T, Trandofilov A, Gazaryan G, Tokmurziyev I, Altamirano Cabrera M, Tsetserukou D. GuideTouch: an obstacle avoidance device with tactile feedback for visually impaired [prepublicación en Internet]. arXiv; 2026 [citado 29 sep 2026]. Disponible en: https://arxiv.org/abs/2601.13813

[25] World Health Organization. Eye care, vision impairment and blindness [Internet]. Geneva: WHO; [s. f.] [citado 29 sep 2026]. Disponible en: https://www.who.int/health-topics/blindness-and-vision-loss

[26] Aziz O, Klenk J, Schwickert L, Chiari L, Becker C, Park EJ, et al. Validation of accuracy of SVM-based fall detection system using real-world fall and non-fall datasets. PLoS One. 2017;12(7):e0180318. doi:10.1371/journal.pone.0180318.

[27] Leong X, Kanesaraj Ramasamy R. Obstacle detection and distance estimation for visually impaired people. IEEE Access. 2023;11:136609-136629. doi:10.1109/ACCESS.2023.3338154.

## Enlaces de las fuentes

- **[16] Sistema portátil de detección de obstáculos:** https://doi.org/10.18687/LACCEI2025.1.1.2028
- **[17] Señales hápticas y auditivas:** https://doi.org/10.1007/s12193-025-00463-2
- **[18] IEC 60529:** https://webstore.iec.ch/en/publication/2452
- **[19] IEC 62133-2:** https://webstore.iec.ch/en/publication/70017
- **[20] ISO 9241-920:** https://www.iso.org/standard/80751.html
- **[21] WCAG 2.2:** https://www.w3.org/TR/WCAG22/
- **[22] ISO 21856:** https://www.iso.org/standard/71986.html
- **[24] GuideTouch:** https://arxiv.org/abs/2601.13813
- **[25] OMS — salud visual:** https://www.who.int/health-topics/blindness-and-vision-loss
- **[26] Detección de caídas:** https://doi.org/10.1371/journal.pone.0180318
- **[27] Detección de obstáculos y estimación de distancia:** https://doi.org/10.1109/ACCESS.2023.3338154
