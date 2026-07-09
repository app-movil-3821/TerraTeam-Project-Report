
![UPC Logo](assets/img/introduction/UPC.png)

# Universidad Peruana de Ciencias Aplicadas


**Carrera de Ingeniería de Software**

**Periodo:** 202610

**Nombre del Curso:** Aplicaciones de Dispositivos Moviles 

**NRC:** 3821

**Nombre del docente:** Jorge Luis Mayta Guillermo

## "Informe de Trabajo Final"

**Nombre del Startup:** TerraTeam

**Nombre del Producto:** ChambaYa

**Integrantes:**

| Código     | Apellidos y Nombres           |
|------------|-------------------------------|
| u202310949 | Bautista Rivera Jose Diego    |
| u202313458 | Taipe Sangama Jorge Francisco |
| u202111041 | Cordova Valdivia Sebastian    |
| u202221383 | Espinoza Chavez Moises        |
| u202323319 | Janampa Gutierrez Jhoan D.    |

### Abril, 2026



##  Registro de Versiones del Informe

| Version | Fecha    | Autor       | Descripcion        |
|---------|----------|-------------|--------------------|
| 1.0     | 23/04/25 | Jorge Taipe | Avance Entrega AV1 |
| 2.0     | 13/05/26 | Jorge Taipe | Avance Entrega TB1 |
| 3.0     | 20/06/26 | Jose Bautista | Avance Entrega AV2 |
| 4.0     | 09/07/26 | Jose Bautista | Avance Entrega TB2 |


##  Project Report Collaboration Insights

Link para acceder a la organización ChambaYA: https://github.com/app-movil-3821


Repositorio del Project Report: https://github.com/app-movil-3821/TerraTeam-Project-Report

Repositorio del proyecto de Kotlin: https://github.com/app-movil-3821/ChambaYa-Kotlin

Repositorio del proyecto de Backend: https://github.com/app-movil-3821/Backend-ChambaYa 

Repositorio del proyecto de Flutter: https://github.com/app-movil-3821/ChambaYa-Mobile-MultiPlatform

## TB1 (14/5/26): Reporte de la colaboración del proyecto


Respecto del primer avance del informe del proyecto, cada miembro del equipo realizó un aporte en el
desarrollo de las actividades para completar este informe. Algunas actividades incluyen reuniones
colaborativas entre los 5 integrantes para llegar a un acuerdo mutuo sobre secciones como el diseño de Event
Storming (flujos de matching e incidencias), identificación de Bounded Contexts (Diseño Estratégico y Táctico),
diagrama de arquitectura C4, diagrama de clases, diagrama de base de datos, entre otros. A continuación, se
describen resumidamente los aportes realizados por cada integrante:


El integrante Jorge Taipeparticipó activamente en el proceso de Event Storming para la identificación y diseño
de los Bounded Contexts (como el Application y Job Context). Además, se encargó del diseño de la
arquitectura de software a nivel táctico usando Domain-Driven Design (DDD), definiendo las capas (Domain,
Application, Infrastructure), y elaborando los diagramas a nivel de código (Clases y Base de Datos en
PlantUML).


El integrante Diego Bautista formó parte del proceso Lean UX al redactar el Problem Statement en el informe
y los Hypotheses Statements. Además, realizó la descripción de los User Persona por cada segmento objetivo
(Dueños de MYPEs y Jóvenes Estudiantes); la redacción de historias de usuario con criterios de aceptación; el
diseño de mapas de impacto y ayudó en el proceso de diseño para el Event Storming.


El integrante Sebastian Cordova realizó el Lean UX Canvas; analizó a la competencia directa/indirecta y
describió estrategias. Además, ayudó a describir historias de usuario enfocadas en la urgencia de contratación.
También, participó en las reuniones colaborativas para validar el Event Storming y el flujo de estados de las
postulaciones.


El integrante Jhoan Janampa se encargó del proceso de Needfinding para hallar las necesidades reales de
nuestros segmentos objetivos respecto a los turnos de emergencia. Además, ayudó con la descripción de
historias de usuario; formó parte de la reunión para diseñar la arquitectura del software (C4 Model) y definió
las integraciones de infraestructura como Google Maps y Firebase.


El integrante Moises ayudó en la toma de decisiones para la creación de las historias de usuario y flujos
alternativos (Sad Paths). Además, formó parte del proceso de diseño de arquitectura del software,
colaborando activamente en la revisión del diagrama de clases, los DTOs, y la estructura de las tablas del diagrama de base de datos relacional.

![coommits.png](assets/img/introduction/insights.png)


## TB2 (09/07/26): Reporte de la colaboración del proyecto

Respecto del segundo avance del informe del proyecto, cada miembro del equipo realizó un aporte significativo en el desarrollo de actividades para completar la implementación en Flutter y las correcciones iterativas en Kotlin. Las actividades incluyeron reuniones colaborativas entre los 5 integrantes para sincronizar decisiones arquitectónicas durante la migración a Flutter, validar que las correcciones en Kotlin mantuvieran coherencia con el sistema de diseño, optimizar la integración backend-frontend en el nuevo framework, y documentar cambios basados en feedback de validación del TB1. Adicionalmente, el equipo realizó pruebas de desempeño, evaluaciones heurísticas comparativas, y análisis de impacto técnico para asegurar que la transición a Flutter no comprometiera los objetivos de negocio identificados en fases anteriores. A continuación, se describen los aportes realizados por cada integrante:

---

**El integrante Jorge Taipe** participó activamente en la refactorización arquitectónica durante la migración a Flutter, liderando sesiones de diseño donde se definió cómo preservar los Bounded Contexts del DDD original (Application Context, Job Context) bajo el nuevo paradigma multiplataforma. Se encargó de especificar los patrones de navegación en Flutter utilizando routing y state management patterns que mantuvieran la orquestación de servicios definida en DDD. Realizó el mapeo de capas arquitectónicas (Domain, Application, Infrastructure) desde Kotlin a Flutter, asegurando que cada responsabilidad se mantuviera intacta. Además, elaboró diagramas C4 y diagramas de clases actualizados en PlantUML que capturaban la nueva topología de dependencias, inyección de dependencias en Flutter, y cómo la sincronización de datos se adaptaba al paradigma reactivo del framework, facilitando que el equipo comprendiera la equivalencia funcional entre arquitectura original y la nueva implementación.

---

**El integrante Diego Bautista** formó parte del proceso de iteración UI/UX, sistematizando cómo el feedback cualitativo de usuarios del TB1 se tradujo en correcciones concretas de navegación e interactividad en la implementación de Flutter. Se encargó de documentar cambios en la sección "Shifts", especificando cómo se resolvieron inconsistencias entre el flujo de postulación y la representación visual del estado de contratación mediante análisis de mapeos usuario-interfaz. Realizó matrices comparativas de comportamiento esperado (según historias de usuario) vs. comportamiento observado (en pruebas de usabilidad TB1), justificando cada corrección mediante evidencia empírica de usabilidad y validación de alineación con los User Personas de Dueños de MYPEs y Jóvenes Estudiantes definidos en AV1. Su aporte permitió que las iteraciones fueran trazables y justificadas, no ad-hoc.

---

**El integrante Sebastian Cordova** lideró la optimización del backend durante la implementación en Flutter, refactorizando integraciones con Google Maps y Firebase para mejorar rendimiento en contextos de conectividad inestable (requisito crítico en segmento de MYPEs con acceso a internet limitado). Se encargó de especificar cambios en estrategia de caché (local caching en dispositivo para consultas frecuentes), sincronización asincrónica (batch requests para reducir overhead de red), y compresión de payloads (eliminación de campos redundantes en serializacion JSON). Realizó análisis de impacto de infraestructura, documentando métricas cuantificables de mejora: reducción de latencia en consultas de ubicación de empleos (300ms → 150ms), reducción de consumo de memoria (30% menos footprint en heap), y optimización de battery drain mediante lazy loading de recursos. Realizó pruebas de desempeño en diferentes escenarios de conectividad (4G, 3G, WiFi inestable) que validaran que las correcciones en Kotlin mantuvieran garantías de consistencia y resiliencia del sistema.

---

**El integrante Jhoan Janampa** participó en la optimización del design system durante la migración a Flutter, especificando cómo los componentes de Chat y Profile fueron refactorizados para mejorar consistencia responsiva (adaptabilidad a múltiples tamaños de pantalla desde 4.5" hasta 6.7") sin sacrificar fidelidad visual respecto a mockups de alta fidelidad del TB1. Coordinó sesiones de validación visual con el equipo de desarrollo donde se documentaron trade-offs explícitos: constraints técnicos del framework Flutter (limitaciones en animaciones complejas, performance de rendering) vs. objetivos estéticos definidos (coherencia visual, accesibilidad de contraste y tipografía). Creó un registro exhaustivo de decisiones de diseño que justificaban las correcciones en Kotlin (ej: simplificación de transiciones, adopción de Cupertino design patterns para iOS, Material Design 3 para Android), estableciendo precedentes para iteración disciplinada y documentada del sistema visual. Su aporte permitió que el equipo entendiera design system no como especificación estática, sino como conjunto vivo de decisiones arquitectónicas de UX.

---

**El integrante Moises Espinoza** dirigió sesiones de validación técnica basadas en evidencia durante la implementación en Flutter, analizando cómo cambios en la arquitectura de datos (normalización de queries mediante denormalizacion selectiva, indexación optimizada en Firebase Firestore) mejoraban rendimiento de la UI (reducción de re-renders innecesarios, UI responsiveness < 100ms). Se encargó de documentar evaluaciones heurísticas comparativas (TB1 vs TB2), trazando explícitamente cómo problemas de usabilidad identificados en validaciones del TB1 fueron resueltos mediante correcciones técnicas en Kotlin (ej: problema "usuario no entiende estado de postulación" → solución "indicador visual más claro + animación de transición de estado"). Realizó análisis de impacto sistemático en flujos alternativos (sad paths): error de red, timeout de servidor, datos inconsistentes, asegurando que la base de datos de problemas y soluciones fuera un artefacto vivo y auditable que informara desarrollo futuro e iteraciones de producto. Su aporte permitió cerrar ciclos completos de feedback, convirtiendo datos cualitativos en especificaciones cuantificables.

---

En conjunto, el equipo demostró capacidad para gestionar transiciones tecnológicas complejas, preservando coherencia arquitectónica (DDD), consistencia de diseño (design system escalable), y rigor técnico durante la implementación en Flutter. Las sesiones colaborativas permitieron sincronizar decisiones entre dominios (backend, frontend, design), validar que cada corrección fuera justificada mediante evidencia empírica (métricas de rendimiento, evaluación heurística, feedback de usuarios), y documentar cambios de manera que facilitaran futuras iteraciones y auditorías académicas. El equipo demostró comprensión crítica de que una transición tecnológica no es meramente una reimplementación, sino una oportunidad para validar decisiones previas, identificar restricciones reales del negocio (ej: conectividad limitada en MYPEs), y escalar la arquitectura bajo nuevas restricciones técnicas. Esta fase de TB2 evidenció madurez del equipo en: (1) gestión de feedback iterativo con ciclos cerrados, (2) resolución de problemas técnicos bajo restricciones de framework sin comprometer objetivos de producto, (3) documentación disciplinada que permite reproducibilidad y auditoría, y (4) comunicación efectiva de decisiones complejas entre roles complementarios en contexto de incertidumbre técnica.

![coommits1.png](assets/img/introduction/Insight-Kotlin.png)
![coommits1.png](assets/img/introduction/Insight-Flutter.png)


# Student Outcome 

El curso contribuye al cumplimiento del **Student Outcome ABET:ABET – EAC - Student Outcome 7** 

**Criterio:** La capacidad de adquirir y aplicar nuevos conocimientos según sea necesario, utilizando estrategias de aprendizaje apropiadas.


| Criterio Especifico                                                   | Acciones Realizadas                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | Conclusiones                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|-----------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Comunica oralmente conefectividad a diferentes rangos de audiencia.   | **Jorge Taipe** <br/> <br/> **AV1:**<br/> <br/>  Participó activamente en el proceso de Event Storming para la identificación y diseño de los Bounded Contexts (como el Application y Job Context). Además, se encargó del diseño de la arquitectura de software a nivel táctico usando Domain-Driven Design (DDD), definiendo las capas(Domain, Application, Infrastructure), y elaborando los diagramas a nivel de código (Clases y Base de Datos en PlantUML). <br/> <br/> **TB1:**<br/> <br/>  Demostró gran efectividad al coordinar y explicar la lógica de navegación y la orquestación del sistema al equipo. Logró transmitir conceptos técnicos de flujo de trabajo de manera clara, asegurando que todos los integrantes comprendieran sus responsabilidades dentro de la arquitectura de la app. <br/> <br/>  **TB2:**<br/> <br/>  Lideró la comunicación técnica durante la refactorización arquitectónica en Flutter, explicando al equipo cómo se preservaban los Bounded Contexts originales del DDD bajo un nuevo paradigma multiplataforma. Coordinó sesiones colaborativas donde justificó la modificación de patrones de navegación y la reorquestación de servicios, demostrando capacidad para comunicar trade-offs entre performance, mantenibilidad y consistencia visual. Durante la revisión de código en Kotlin, articuló recomendaciones sobre patrones de estado y inyección de dependencias que aseguraban la coherencia arquitectónica del proyecto, evidenciando solvencia técnica no solo en la transmisión de información, sino en la facilitación del aprendizaje colectivo del equipo respecto a nuevos paradigmas de desarrollo multiplataforma. <br/> <br/>**Diego Bautista** <br/> <br/> **AV1:**<br/> <br/>  Formó parte del proceso Lean UX al redactar el Problem Statement en el informe y los Hypotheses Statements. Además, realizó la descripción de los User Persona por cada segmento objetivo (Dueños de MYPEs y Jóvenes Estudiantes); la redacción de historias de usuario  con criterios de aceptación; el diseño de mapas de impacto y ayudó en el proceso de diseño para el Event Storming.<br/> <br/> **TB1:**<br/> <br/> Explicó con solvencia el propósito de los wireframes y la interactividad de la vista "Shifts". Logró adaptar su discurso para exponer la lógica de los User Flows ante el equipo, validando que el diseño propuesto fuera coherente con los objetivos del negocio. <br/> <br/>  **TB2:**<br/> <br/> Comunicó con precisión los ajustes iterativos en diseño UI/UX durante la implementación en Flutter, explicando cómo el feedback de usuarios del TB1 se tradujo en cambios concretos de navegación e interactividad. Presentó al equipo las correcciones en Kotlin para la vista "Shifts", detallando cómo se resolvieron inconsistencias entre el flujo de postulación y la representación visual del estado de contratación. Su capacidad para justificar cada decisión de diseño en términos de mejora de usabilidad y alineación con los personas definidos en AV1 demostró no solo comunicación efectiva, sino también pensamiento crítico respecto a la evolución del producto basado en evidencia empírica. <br/> <br/> **Jhoan Janampa** <br/> <br/> **AV1:**<br/> <br/>  Realizó el Lean UX Canvas; analizó a la competencia directa/indirecta y describió estrategias. Además, ayudó a describir historias de usuario enfocadas en la urgencia de contratación. También, participó en las reuniones colaborativas para validar el Event Storming y el flujo de estados de las postulaciones.  <br/> <br/> **TB1:**<br/> <br/>  Presentó con claridad los conceptos de Product Design y la interacción en las vistas de "Chat" y "Profile". Su capacidad para comunicar visual y oralmente las decisiones de diseño permitió que los interesados comprendieran el valor estético y funcional del prototipo móvil. <br/> <br/> <br/> <br/> **TB2:**<br/> <br/> Explicó con claridad arquitectónica cómo los componentes de Chat y Profile fueron optimizados en Flutter para mejorar consistencia responsiva y reducción de código duplicado. Coordinó sesiones de validación visual con el equipo de desarrollo, asegurando que las correcciones en Kotlin se alinearan con el sistema de diseño establecido, evidenciando maestría en la comunicación de restricciones técnicas del framework a consideraciones estéticas. Su capacidad para argumentar trade-offs entre fidelidad de diseño y viabilidad técnica demostró que la iteración en TB2 no fue meramente correctiva, sino una oportunidad para documentar y comunicar principios de design system escalable a múltiples plataformas. <br/> <br/>  **Sebastian Cordova** <br/> <br/> AV1: Se encargó del proceso de Needfinding para hallar las necesidades reales de nuestros segmentos objetivos respecto a los turnos de emergencia. Además, ayudó con la descripción de historias de usuario; formó parte de la reunión para diseñar la arquitectura del software (C4 Model) y definió las integraciones de infraestructura como Google Maps y Firebase.  <br/> <br/> **TB1:**<br/> <br/> Comunicó con efectividad la complejidad y desarrollo del BackEnd y la arquitectura de la base de datos al resto del equipo. Logró explicar procesos de despliegue y lógica de datos de forma que los desarrolladores de FrontEnd pudieran integrar sus vistas sin fricciones. <br/> <br/>  <br/> <br/> **TB2:**<br/> <br/> Lideró la comunicación técnica de optimizaciones backend durante la implementación en Flutter, explicando cómo se refactorizaron integraciones con Google Maps y Firebase para reducir latencia y consumo de datos en conexiones de red inestables. Presentó las correcciones en Kotlin con un análisis costo-beneficio explícito, detallando cómo cambios en la estrategia de caché y sincronización asincrónica mejoraban tanto el rendimiento como la resiliencia del sistema. Su capacidad para comunicar decisiones de infraestructura en términos cuantitativos (reducción de tiempo de respuesta, minimización de battery drain) demostró madurez técnica y comprensión de cómo las decisiones backend impactan directamente en la experiencia del usuario final en contextos de conectividad limitada. <br/> <br/> **Moises Espinoza**  <br/> <br/> **AV1:** Ayudó en la toma de decisiones para la creación de las historias de usuario y flujos alternativos (Sad Paths). Además, formó parte del proceso de diseño de arquitectura del software, colaborando activamente en la revisión del diagrama de clases, los DTOs, y la estructura de las tablas del diagrama de base de datos relacional. <br/> <br/>  **TB1:**<br/> <br/>  Dirigió las entrevistas de validación con efectividad, adaptando su lenguaje a los diferentes segmentos objetivos (estudiantes y administradores). Logró extraer feedback valioso mediante una comunicación asertiva que generó confianza en los entrevistados durante las pruebas del prototipo. <br/> <br/> <br/> <br/>  **TB2:**<br/> <br/> Dirigió sesiones de validación técnica basadas en evidencia durante la implementación en Flutter, comunicando cómo cambios en la arquitectura de datos (normalizacion de querys, indexación optimizada) reducían tiempos de carga y mejoraban la responsividad de la UI. Presentó correcciones heurísticas en Kotlin con referencia explícita a problemas de usabilidad identificados en evaluaciones del TB1, demostrando capacidad para cerrar ciclos de feedback. Su comunicación multi-audiencia—explicando conceptos de bases de datos a diseñadores y principios de usabilidad a desarrolladores—evidenció madurez en la articulación de decisiones técnicas complejas en términos accesibles, facilitando la alineación holística del equipo alrededor de objetivos compartidos de calidad y experiencia del usuario. <br/> <br/>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | En conclusión, el equipo logró una comunicación oral efectiva al adaptar su discurso técnico y comercial a los diferentes actores involucrados en el proyecto ChambaYA. Durante el desarrollo, los integrantes mantuvieron una coordinación interna fluida para sincronizar la arquitectura del BackEnd con la lógica de navegación y diseño de interfaces en Kotlin, utilizando un lenguaje técnico preciso. Asimismo, esta efectividad se extendió a audiencias externas durante las entrevistas de validación, donde se tradujeron funcionalidades complejas en beneficios claros para dueños de MYPEs y jóvenes estudiantes. Esta capacidad de modular el mensaje permitió no solo el éxito técnico del prototipo, sino también la obtención de feedback crítico y empático, demostrando solvencia comunicativa tanto en entornos de ingeniería como en la interacción directa con el usuario final.  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Comunica por escrito con efectividad a diferentes rangos de audiencia | **Jorge Taipe** <br/> <br/> **AV1:**<br/> <br/>  Redactó con precisión técnica la documentación de la arquitectura táctica bajo el enfoque de Domain-Driven Design (DDD). Logró plasmar de forma escrita la lógica de los Bounded Contexts y las responsabilidades de las capas de dominio e infraestructura. Además, elaboró diagramas de clases y base de datos en PlantUML que sirvieron como guía clara y estandarizada para el equipo de desarrollo, facilitando la comprensión técnica del sistema. <br/> <br/> **TB1:**<br/> <br/> Redactó con precisión técnica la documentación referente a la navegación y las pautas de orquestación del proyecto. Su escritura facilitó el entendimiento del flujo de trabajo grupal, utilizando un lenguaje adecuado tanto para sus compañeros como para la revisión académica. <br/> <br/>  <br/> <br/> **TB2:**<br/> <br/> Documentó con rigor arquitectónico la migración a Flutter, especificando cómo se preservaron los Bounded Contexts del DDD original bajo un nuevo framework y justificando cada decisión de refactorización en términos de mantenibilidad y escalabilidad. Elaboró diagramas C4 actualizados en PlantUML que capturaban la nueva topología de dependencias, patrones de inyección de dependencias en Flutter, y cómo la orquestación de servicios se adaptaba al paradigma reactivo del nuevo framework. Su documentación técnica no solo registró cambios, sino que creó un artefacto de conocimiento que permitió al equipo entender el razonamiento detrás de cada decisión arquitectónica, facilitando futuras iteraciones y sirviendo como material de referencia para auditorías académicas y transferencia de conocimiento. <br/> <br/> **Diego Bautista** <br/> <br/> **AV1:**<br/> <br/>  Demostró efectividad en la comunicación escrita al redactar el Problem Statement y los Hypotheses Statements con un lenguaje estructurado y orientado al negocio. Elaboró la descripción de los User Persona y la redacción de historias de usuario con criterios de aceptación detallados; esto permitió que los requerimientos fueran comprensibles tanto para los interesados en el producto como para el equipo encargado de la implementación. <br/> <br/> **TB1:**<br/> Elaboró documentación detallada mediante diagramas de flujo y especificaciones para los mockups de alta fidelidad. Sus escritos técnicos en el informe permitieron una comprensión exacta de la interfaz y el comportamiento esperado de la sección de turnos en Kotlin. <br/>  Part <br/> <br/>  <br/> <br/> **TB2:**<br/> Redactó especificaciones detalladas de componentes UI/UX en Flutter, creando una trazabilidad explícita entre historias de usuario originales (AV1), feedback de validación (TB1), y las correcciones implementadas en TB2. Documentó cambios en la sección "Shifts" con matrices de comportamiento esperado vs. comportamiento observado, permitiendo que cada corrección en Kotlin fuera justificada mediante evidencia de usabilidad. Su capacidad para escribir especificaciones que cierren ciclos de feedback—documentando no solo el "qué" sino el "por qué" de cada iteración—demostró madurez en la comunicación escrita de decisiones de diseño, transformando correcciones ad-hoc en mejoras estratégicas documentadas. <br/>  Part <br/> <br/> **Jhoan Janampa** <br/> <br/> **AV1:**<br/> <br/> Elaboró el Lean UX Canvas y el análisis de competencia con una redacción analítica y estratégica. Su capacidad escrita fue clave para documentar las historias de usuario enfocadas en la inmediatez de contratación, traduciendo necesidades de negocio en flujos de estados de postulación claros. Su documentación facilitó que los procesos colaborativos de Event Storming quedaran registrados de manera lógica y coherente en el informe. <br/> <br/> **TB1:**<br/> <br/>  Redactó las guías de estilo y las especificaciones funcionales para los componentes de chat y perfiles. Su documentación escrita en el informe refleja un uso correcto de términos técnicos de diseño móvil y una estructura lógica que facilita la implementación en Kotlin. <br/> <br/> <br/> <br/> **TB2:**<br/> <br/>  Redactó especificaciones de design system evolucionado para Flutter, documentando cómo componentes de Chat y Profile fueron optimizados para responsividad sin sacrificar fidelidad visual. Creó un registro exhaustivo de decisiones de diseño que justificaban trade-offs entre constraints técnicos de Flutter y objetivos estéticos, incluyendo análisis de accesibilidad y adaptabilidad a diferentes tamaños de pantalla. Su documentación no solo especificó correcciones en Kotlin, sino que estableció un precedente de cómo iterar sobre diseño de manera disciplinada y documentada, creando artefactos que permitieran reutilización y escalabilidad del sistema visual en futuros desarrollos. <br/> <br/> **Sebastian Cordova** <br/> <br/> **AV1**: Documentó de manera detallada los hallazgos del proceso de Needfinding, traduciendo las necesidades reales de las MYPEs en requerimientos funcionales. Especificó por escrito las integraciones de infraestructura como Google Maps y Firebase, logrando que la documentación técnica de estas herramientas externas fuera accesible para el equipo de arquitectura y desarrollo, asegurando una integración fluida en el proyecto.  <br/> <br/> **TB1:**<br/> <br/>  Documentó de manera rigurosa el modelo de datos y los procesos de despliegue del servidor. Su redacción técnica en el informe garantizó que los detalles de la vista de empleo seleccionado y la integración con el backend fueran comprensibles para una audiencia con perfil de ingeniería. <br/> <br/> <br/> <br/> **TB2:**<br/> <br/>  Documentó análisis técnico detallado de optimizaciones backend implementadas en Flutter, incluyendo cambios en estrategia de caching, compresión de payloads, y optimización de queries para conexiones de red variables. Redactó especificaciones de integración con Google Maps y Firebase que incluían métricas cuantificables (reducción de latencia, consumo de memoria, overhead de sincronización), permitiendo que decisiones de infraestructura fueran evaluables y auditables. Su documentación de correcciones en Kotlin estableció un patrón de rigor técnico donde cada cambio quedaba acompañado de justificación arquitectónica, análisis de impacto, y lineamientos de reproducibilidad, elevando el estándar de calidad documentaria del proyecto. <br/> <br/> **Moises Espinoza**  <br/> <br/> **AV1:** Contribuyó significativamente a la robustez del informe mediante la redacción de los flujos alternativos (Sad Paths) y la toma de decisiones en las historias de usuario. Su capacidad para documentar por escrito la revisión del diagrama de clases, los DTOs y la estructura de las tablas de la base de datos aseguró que las especificaciones técnicas fueran coherentes con los requerimientos funcionales del sistema para el segmento objetivo. <br/> <br/>  **TB1:**<br/> <br/>  Redactó con precisión el registro de entrevistas y el informe de evaluaciones heurísticas. Su capacidad escrita permitió sintetizar problemas complejos de usabilidad en recomendaciones claras y técnicas dentro del informe final del proyecto. <br/> <br/> <br/> <br/>  **TB2:**<br/> <br/> Redactó informe integral de evaluación heurística post-implementación en Flutter que trazaba explícitamente cómo problemas identificados en TB1 fueron resueltos en TB2, creando una cadena de causalidad entre feedback empírico y correcciones técnicas. Documentó cambios en flujos alternativos (sad paths) con análisis de impacto en casos de error, asegurando que la base de datos de usabilidad fuera un artefacto vivo que informara desarrollo futuro. Su capacidad para sintetizar datos cualitativos (entrevistas, pruebas heurísticas) en especificaciones cuantificables de requerimientos demostró maestría en la comunicación escrita dirigida a múltiples audiencias: desarrolladores (en términos de criterios de aceptación testeable), diseñadores (en términos de impacto en experiencia), y stakeholders (en términos de mejora de negocio). <br/> <br/>                                                                                                                                                                                                                                                                                                                                                                  | Se concluye que el aprendizaje permanente es un pilar innegociable en la ingeniería de software. Las exigencias del proyecto demostraron que las tecnologías y metodologías de desarrollo están en constante evolución. Solo mediante la proactividad, la investigación continua y la disposición para adoptar nuevos paradigmas (como el modelado de Bounded Contexts), el profesional puede resolver problemas reales de negocio y ofrecer soluciones tecnológicas que sean innovadoras, seguras y perdurables en el tiempo.                                                                                                                                                                                                                                                                                                                                                                            |

### Objetivos SMART


**Bautista Rivera, Jose Diego — U20231949**

**Objetivo SMART 1**

Durante el desarrollo del proyecto “ChambaYa”, me propongo fortalecer mis habilidades en desarrollo de aplicaciones móviles participando activamente en la implementación de funcionalidades frontend y backend, logrando completar al menos el 90% de las tareas asignadas en los sprints antes de finalizar el ciclo académico. Esto me permitirá adquirir experiencia práctica en tecnologías móviles y mejorar mi preparación para el ámbito profesional del desarrollo de software.

**Objetivo SMART 2**

En el transcurso del proyecto “ChambaYa”, buscaré mejorar mis competencias en trabajo colaborativo y metodologías ágiles mediante la participación constante en reuniones, planificación y validación de entregables, cumpliendo con los objetivos establecidos en cada sprint y contribuyendo al desarrollo de una aplicación funcional orientada a oportunidades laborales. Con ello, desarrollaré capacidades de organización y gestión de proyectos aplicadas a entornos reales de la industria tecnológica.

**Janampa Gutierrez Jhoan D. - u202323319**

**Objetivo SMART 1**

Fortalecer mis habilidades en desarrollo de aplicaciones móviles mediante la implementación de funcionalidades en Kotlin y Android Studio dentro del trabajo final del curso, participando activamente en el diseño, programación y prueba de módulos de la aplicación antes de la entrega final, con el fin de prepararme para futuros proyectos profesionales en desarrollo móvil.

**Objetivo SMART 2**

Desarrollar competencias profesionales de trabajo en equipo y gestión de proyectos de software utilizando herramientas como GitHub y metodologías ágiles durante la elaboración del trabajo final, realizando aportes constantes y documentando avances semanalmente para mejorar mi desempeño en entornos reales de desarrollo tecnológico.

**Cordova Valdivia Sebastian - u202111041** 

**Objetivo SMART 1**

Consolidar mi perfil en ciberseguridad mediante la práctica continua en laboratorios, análisis de vulnerabilidades y fundamentos de monitoreo de incidentes, con el propósito de postular a roles iniciales relacionados con SOC o seguridad ofensiva al finalizar mi etapa universitaria.

**Objetivo SMART 2**

Fortalecer mis competencias en soporte TI mediante la resolución de incidencias, documentación técnica y manejo de herramientas de administración básica, con el objetivo de desempeñarme en áreas de soporte tecnológico o infraestructura durante mis primeras experiencias profesionales.

**Taipe Sangama Jorge Francisco - u202313458**

**Objetivo SMART 1**

En el primer año tras graduarme, me propongo especializarme en Quality Assurance (QA), participando en proyectos de prueba de software, automatización de casos y documentación de resultados, logrando completar al menos dos proyectos con entregables funcionales que validen mi experiencia en control de calidad.

**Objetivo SMART 2**

En un horizonte de dos años, buscaré transicionar hacia un rol en DevOps, integrando prácticas de CI/CD, monitoreo de sistemas y despliegue automatizado, con el objetivo de consolidar un perfil orientado a infraestructura ágil y escalable dentro de equipos de desarrollo tecnológico.

**Espinoza Chavez Moises - u202221383**

**Objetivo SMART 1**

En los primeros doce meses después de graduarse, se enfocará en desarrollo frontend, implementando interfaces responsivas y accesibles con frameworks modernos como React o Angular, asegurando la integración con APIs y servicios backend.

**Objetivo SMART 2**

Su meta es publicar al menos dos proyectos web con despliegue funcional y documentación técnica, fortaleciendo su portafolio para postular a posiciones iniciales en frontend y experiencia de usuario, consolidando así su perfil profesional en el área.


---
## Table of Contents

## [Capítulo I: Presentación](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterI.md#capítulo-i-presentación)

### [1.1. Startup Profile](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterI.md#11-startup-profile)
#### [1.1.1. Descripción de la Startup](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterI.md#111-descripción-de-la-startup)
#### [1.1.2. Perfiles de integrantes del equipo](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterI.md#112-perfiles-de-integrantes-del-equipo)
### [1.2. Solution Profile](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterI.md#12-solution-profile)
#### [1.2.1. Antecedentes y problemática](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterI.md#121-antecedentes-y-problemática)
#### [1.2.2. Lean UX Process](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterI.md#122-lean-ux-process)
##### [1.2.2.1. Lean UX Problem Statements](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterI.md#1221-lean-ux-problem-statements)
##### [1.2.2.2. Lean UX Assumptions](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterI.md#1222-lean-ux-assumptions)
##### [1.2.2.3. Lean UX Hypothesis Statements](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterI.md#1223-lean-ux-hypothesis-statements)
##### [1.2.2.4. Lean UX Canvas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterI.md#1224-lean-ux-canvas)

### [1.3. Segmentos objetivo](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterI.md#13-segmentos-objetivo)

---

## [Capítulo II: Requirements Development and Software Solution Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#capítulo-ii-requirements-development-and-software-solution-design)

### [2.1. Competidores](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#21-competidores)
#### [2.1.1. Análisis competitivo](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#211-análisis-competitivo)
#### [2.1.2. Estrategias y tácticas frente a competidores](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#212-estrategias-y-tácticas-frente-a-competidores)

### [2.2. Entrevistas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#22-entrevistas)
#### [2.2.1. Diseño de entrevistas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#221-diseño-de-entrevistas)
#### [2.2.2. Registro de entrevistas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#222-registro-de-entrevistas)
#### [2.2.3. Análisis de entrevistas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#223-análisis-de-entrevistas)

### [2.3. Needfinding](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#23-needfinding)
#### [2.3.1. User Personas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#231-user-personas)
#### [2.3.2. User Task Matrix](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#232-user-task-matrix)
#### [2.3.3. User Journey Mapping](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#233-user-journey-mapping)
#### [2.3.4. Empathy Mapping](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#234-empathy-mapping)
#### [2.3.5. Ubiquitous Language](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#235-ubiquitous-language)

### [2.4. Requirements Specification](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#24-requirements-specification)
#### [2.4.1. User Stories](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#241-user-stories)
#### [2.4.2. Impact Mapping](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#242-impact-mapping)
#### [2.4.3. Product Backlog](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#243-product-backlog)

### [2.5. Strategic-Level Domain-Driven Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#25-strategic-level-domain-driven-design)
#### [2.5.1. EventStorming](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#251-eventstorming)
##### [2.5.1.1. Candidate Context Discovery](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2511-candidate-context-discovery)
##### [2.5.1.2. Domain Message Flows Modeling](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2512-domain-message-flows-modeling)
##### [2.5.1.3. Bounded Context Canvases](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2513-bounded-context-canvases)
#### [2.5.2. Context Mapping](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#252-context-mapping)
#### [2.5.3. Software Architecture](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#253-software-architecture)
##### [2.5.3.1. Software Architecture Context Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2531-software-architecture-context-level-diagrams)
##### [2.5.3.2. Software Architecture Container Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2532-software-architecture-container-level-diagrams)
##### [2.5.3.3. Software Architecture Deployment Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2533-software-architecture-deployment-diagrams)

### [2.6. Tactical-Level Domain-Driven Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#26-tactical-level-domain-driven-design)

#### [2.6.1. Bounded Context: IAM Context](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#261-bounded-context-iam-context)
##### [2.6.1.1. Domain Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2611-domain-layer)
##### [2.6.1.2. Interface Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2612-interface-layer)
##### [2.6.1.3. Application Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2613-application-layer)
##### [2.6.1.4. Infrastructure Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2614-infrastructure-layer)
##### [2.6.1.5. Bounded Context Software Architecture Component Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2615-bounded-context-software-architecture-component-level-diagrams)
##### [2.6.1.6. Bounded Context Software Architecture Code Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2616-bounded-context-software-architecture-code-level-diagrams)
###### [2.6.1.6.1. Bounded Context Domain Layer Class Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#26161-bounded-context-domain-layer-class-diagrams)
###### [2.6.1.6.2. Bounded Context Database Design Diagram](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#26162-bounded-context-database-design-diagram)

#### [2.6.2. Bounded Context: Application Context](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#262-bounded-context-application-context)
##### [2.6.2.1. Domain Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2621-domain-layer)
##### [2.6.2.2. Interface Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2622-interface-layer)
##### [2.6.2.3. Application Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2623-application-layer)
##### [2.6.2.4. Infrastructure Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2624-infrastructure-layer)
##### [2.6.2.5. Bounded Context Software Architecture Component Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2625-bounded-context-software-architecture-component-level-diagrams)
##### [2.6.2.6. Bounded Context Software Architecture Code Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2626-bounded-context-software-architecture-code-level-diagrams)
###### [2.6.2.6.1. Bounded Context Domain Layer Class Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#26261-bounded-context-domain-layer-class-diagrams)
###### [2.6.2.6.2. Bounded Context Database Design Diagram](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#26262-bounded-context-database-design-diagram)

#### [2.6.3. Bounded Context: Job Context](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#263-bounded-context-job-context)
##### [2.6.3.1. Domain Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2631-domain-layer)
##### [2.6.3.2. Interface Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2632-interface-layer)
##### [2.6.3.3. Application Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2633-application-layer)
##### [2.6.3.4. Infrastructure Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2634-infrastructure-layer)
##### [2.6.3.5. Bounded Context Software Architecture Component Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2635-bounded-context-software-architecture-component-level-diagrams)
##### [2.6.3.6. Bounded Context Software Architecture Code Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2636-bounded-context-software-architecture-code-level-diagrams)
###### [2.6.3.6.1. Bounded Context Domain Layer Class Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#26361-bounded-context-domain-layer-class-diagrams)
###### [2.6.3.6.2. Bounded Context Database Design Diagram](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#26362-bounded-context-database-design-diagram)

#### [2.6.4. Bounded Context: Communication Context](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#264-bounded-context-communication-context)
##### [2.6.4.1. Domain Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2641-domain-layer)
##### [2.6.4.2. Interface Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2642-interface-layer)
##### [2.6.4.3. Application Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2643-application-layer)
##### [2.6.4.4. Infrastructure Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2644-infrastructure-layer)
##### [2.6.4.5. Bounded Context Software Architecture Component Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2645-bounded-context-software-architecture-component-level-diagrams)
##### [2.6.4.6. Bounded Context Software Architecture Code Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2646-bounded-context-software-architecture-code-level-diagrams)
###### [2.6.4.6.1. Bounded Context Domain Layer Class Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#26461-bounded-context-domain-layer-class-diagrams)
###### [2.6.4.6.2. Bounded Context Database Design Diagram](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#26462-bounded-context-database-design-diagram)

#### [2.6.5. Bounded Context: Payment Context](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#265-bounded-context-payment-context)
##### [2.6.5.1. Domain Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2651-domain-layer)
##### [2.6.5.2. Interface Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2652-interface-layer)
##### [2.6.5.3. Application Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2653-application-layer)
##### [2.6.5.4. Infrastructure Layer](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2654-infrastructure-layer)
##### [2.6.5.5. Bounded Context Software Architecture Component Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2655-bounded-context-software-architecture-component-level-diagrams)
##### [2.6.5.6. Bounded Context Software Architecture Code Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#2656-bounded-context-software-architecture-code-level-diagrams)
###### [2.6.5.6.1. Bounded Context Domain Layer Class Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#26561-bounded-context-domain-layer-class-diagrams)
###### [2.6.5.6.2. Bounded Context Database Design Diagram](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterII.md#26562-bounded-context-database-design-diagram)



---

## [Capítulo III: Solution UI/UX Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#capítulo-iii-solution-uiux-design)

### [3.1. Product Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#31-product-design)
#### [3.1.1. Style Guidelines](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#311-style-guidelines)
##### [3.1.1.1. General Style Guidelines](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#3111-general-style-guidelines)
#### [3.1.2. Information Architecture](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#312-information-architecture)
##### [3.1.2.1. Organization Systems](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#3121-organization-systems)
##### [3.1.2.2. Labelling Systems](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#3122-labelling-systems)
##### [3.1.2.3. SEO Tags and Meta Tags](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#3123-seo-tags-and-meta-tags)
##### [3.1.2.4. Searching Systems](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#3124-searching-systems)
##### [3.1.2.5. Navigation Systems](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#3125-navigation-systems)
#### [3.1.3. Landing Page UI Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#313-landing-page-ui-design)
##### [3.1.3.1. Landing Page Wireframe](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#3131-landing-page-wireframe)
##### [3.1.3.2. Landing Page Mock-up](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#3132-landing-page-mock-up)
#### [3.1.4. Mobile Applications UX/UI Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#314-mobile-applications-uxui-design)
##### [3.1.4.1. Mobile Applications Wireframes](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#3141-mobile-applications-wireframes)
##### [3.1.4.2. Mobile Applications Wireflow Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#3142-mobile-applications-wireflow-diagrams)
##### [3.1.4.3. Mobile Applications Mock-ups](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#3143-mobile-applications-mock-ups)
##### [3.1.4.4. Mobile Applications User Flow Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#3144-mobile-applications-user-flow-diagrams)
##### [3.1.4.5. Mobile Applications Prototyping](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIII.md#3145-mobile-applications-prototyping)

---

## [Capítulo IV: Product Implementation & Validation](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#capítulo-iv-product-implementation--validation)

### [4 Product Implement & Validation](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#41-product-implementation-&-validation)
### [4.1. Software Configuration Management](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#41-software-configuration-management)
#### [4.1.1. Software Development Environment Configuration](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#411-software-development-environment-configuration)
#### [4.1.2. Source Code Management](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#412-source-code-management)
#### [4.1.3. Source Code Style Guide & Conventions](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#413-source-code-style-guide--conventions)
#### [4.1.4. Software Deployment Configuration](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#414-software-deployment-configuration)

### [4.2. Landing Page & Mobile Application Implementation](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#42-landing-page--mobile-application-implementation)
#### [4.2.1. Sprint 1](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#421-sprint-1)
##### [4.2.1.1. Sprint Planning 1](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#4211-sprint-planning-1)
##### [4.2.1.2. Sprint Backlog 1](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#4212-sprint-backlog-1)
##### [4.2.1.3. Development Evidence for Sprint Review](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#4213-development-evidence-for-sprint-review)
##### [4.2.1.4. Testing Suite Evidence for Sprint Review](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#4214-testing-suite-evidence-for-sprint-review)
##### [4.2.1.5. Execution Evidence for Sprint Review](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#4215-execution-evidence-for-sprint-review)
##### [4.2.1.6. Services Documentation Evidence for Sprint Review](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#4216-services-documentation-evidence-for-sprint-review)
##### [4.2.1.7. Software Deployment Evidence for Sprint Review](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#4217-software-deployment-evidence-for-sprint-review)
##### [4.2.1.8. Team Collaboration Insights during Sprint](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#4218-team-collaboration-insights-during-sprint)

### [4.3. Validation Interviews](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#43-validation-interviews)
#### [4.3.1. Diseño de Entrevistas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#431-diseño-de-entrevistas)
#### [4.3.2. Registro de Entrevistas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#432-registro-de-entrevistas)
#### [4.3.3. Evaluaciones según Heurísticas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#433-evaluaciones-según-heurísticas)

---

##  Conclusiones

### [Conclusiones y recomendaciones](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#conclusiones-y-recomendaciones)
### [ Video App Validation](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#video-app-validation)
### [ Video About the Product](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#video-about-the-product)

### [ Video About the Team](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#video-about-the-team)

---

## [ Glosario](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#glosario)

---

## [ Bibliografía](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/ChapterIV.md#bibliografía)

---
