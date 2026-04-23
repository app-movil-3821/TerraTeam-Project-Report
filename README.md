# Universidad Peruana de Ciencias Aplicadas

![UPC Logo](assets/img/introduction/UPC.png)

**Facultad de Ingeniería**

**Carrera de Ingeniería de Software**

**Periodo:** 202610

**NRC:** 3821

**Nombre del profesor:** Jorge Luis Mayta Guillermo

### "Informe de Trabajo Final"

**Nombre del Startup:** TerraTeam

**Nombre del Producto:** ChambaYa

**Integrantes:**

| Código     | Apellidos y Nombres           |
|------------|-------------------------------|
| u202310949 | Bautista Rivera Jose Diego    |
| u202323319 | Janampa Gutierrez Jhoan D.    |
| u202313458 | Taipe Sangama Jorge Francisco |
| u202111041 | Cordova Valdivia Sebastian    |
| u202221383 | Moises Espinoza Chavez        |


### Abril, 2026


#  Project Report

---

##  Registro de Versiones del Informe

| Version   | Fecha    | Autor       | Descripcion de los cambios |
|-----------|----------|-------------|----------------------------|
| 1.0       | 23/04/25 | Jorge Taipe | Avance Entrega AV1         |

##  Project Report Collaboration Insights

---

Link para acceder a la organización ChambaYA: https://github.com/app-movil-3821

Repositorio del Project Report: https://github.com/app-movil-3821/TerraTeam-Project-Report

AV1 (Fecha de entrega): Reporte de la colaboración del proyecto

Respecto del primer avance del informe del proyecto, cada miembro del equipo realizó un aporte en el desarrollo de las actividades para completar este informe. Algunas actividades incluyen reuniones colaborativas entre los 5 integrantes para llegar a un acuerdo mutuo sobre secciones como el diseño de Event Storming (flujos de matching e incidencias), identificación de Bounded Contexts (Diseño Estratégico y Táctico), diagrama de arquitectura C4, diagrama de clases, diagrama de base de datos, entre otros. A continuación, se describen resumidamente los aportes realizados por cada integrante:

El integrante Jorge Taipeparticipó activamente en el proceso de Event Storming para la identificación y diseño de los Bounded Contexts (como el Application y Job Context). Además, se encargó del diseño de la arquitectura de software a nivel táctico usando Domain-Driven Design (DDD), definiendo las capas (Domain, Application, Infrastructure), y elaborando los diagramas a nivel de código (Clases y Base de Datos en PlantUML).

El integrante Diego Bautista formó parte del proceso Lean UX al redactar el Problem Statement en el informe y los Hypotheses Statements. Además, realizó la descripción de los User Persona por cada segmento objetivo (Dueños de MYPEs y Jóvenes Estudiantes); la redacción de historias de usuario con criterios de aceptación; el diseño de mapas de impacto y ayudó en el proceso de diseño para el Event Storming.

El integrante Sebastian Cordova realizó el Lean UX Canvas; analizó a la competencia directa/indirecta y describió estrategias. Además, ayudó a describir historias de usuario enfocadas en la urgencia de contratación. También, participó en las reuniones colaborativas para validar el Event Storming y el flujo de estados de las postulaciones.

El integrante Jhoan Janampa se encargó del proceso de Needfinding para hallar las necesidades reales de nuestros segmentos objetivos respecto a los turnos de emergencia. Además, ayudó con la descripción de historias de usuario; formó parte de la reunión para diseñar la arquitectura del software (C4 Model) y definió las integraciones de infraestructura como Google Maps y Firebase.

El integrante Moises ayudó en la toma de decisiones para la creación de las historias de usuario y flujos alternativos (Sad Paths). Además, formó parte del proceso de diseño de arquitectura del software, colaborando activamente en la revisión del diagrama de clases, los DTOs, y la estructura de las tablas del diagrama de base de datos relacional.

![Commits.png](assets/img/chapter-1/Commits.png)

##  Contenido

### Tabla de Contenidos

### Student Outcome 
| Criterio Especifico | Acciones Realizadas                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | Conclusiones                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | 
|---------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|    Actualiza conceptos y conocimientos necesarios para su desarrollo profesional y en especial para su proyecto en soluciones de software.                 | **Jorge Taipe**<br/> <br/> **AV1:** Participó activamente en el proceso de Event Storming para la identificación y diseño de los Bounded Contexts (como el Application y Job Context). Además, se encargó del diseño de la arquitectura de software a nivel táctico usando Domain-Driven Design (DDD), definiendo las capas (Domain, Application, Infrastructure), y elaborando los diagramas a nivel de código (Clases y Base de Datos en PlantUML).  <br/> <br/> **Diego Bautista** <br/> <br/> **AV1:** Formó parte del proceso Lean UX al redactar el Problem Statement en el informe y los Hypotheses Statements. Además, realizó la descripción de los User Persona por cada segmento objetivo (Dueños de MYPEs y Jóvenes Estudiantes); la redacción de historias de usuario con criterios de aceptación; el diseño de mapas de impacto y ayudó en el proceso de diseño para el Event Storming. <br/> <br/> **Jhoan Janampa** <br/> <br/> AV1: Realizó el Lean UX Canvas; analizó a la competencia directa/indirecta y describió estrategias. Además, ayudó a describir historias de usuario enfocadas en la urgencia de contratación. También, participó en las reuniones colaborativas para validar el Event Storming y el flujo de estados de las postulaciones.  <br/> <br/> **Sebastian Cordova** <br/> <br/> **AV1:** Se encargó del proceso de Needfinding para hallar las necesidades reales de nuestros segmentos objetivos respecto a los turnos de emergencia. Además, ayudó con la descripción de historias de usuario; formó parte de la reunión para diseñar la arquitectura del software (C4 Model) y definió las integraciones de infraestructura como Google Maps y Firebase. <br/> <br/> **Moises Espinoza** <br/> <br/>  **AV1:** Ayudó en la toma de decisiones para la creación de las historias de usuario y flujos alternativos (Sad Paths). Además, formó parte del proceso de diseño de arquitectura del software, colaborando activamente en la revisión del diagrama de clases, los DTOs, y la estructura de las tablas del diagrama de base de datos relacional. | Se concluye que la actualización constante en patrones de diseño y arquitecturas modernas es fundamental para construir un sistema escalable y resiliente. La adopción de estándares de la industria (como DDD y Clean Architecture) ha permitido aislar la complejidad del negocio de emparejamiento, demostrando que aplicar estos conceptos teóricos a la práctica mejora drásticamente la calidad técnica del entregable y eleva la competitividad del estudiante frente a los estándares actuales del mercado laboral.     |
|     Reconoce la necesidad del aprendizaje permanente para el desempeño profesional y el desarrollo de proyectos en soluciones de software.                |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | Se concluye que el aprendizaje permanente es un pilar innegociable en la ingeniería de software. Las exigencias del proyecto demostraron que las tecnologías y metodologías de desarrollo están en constante evolución. Solo mediante la proactividad, la investigación continua y la disposición para adoptar nuevos paradigmas (como el modelado de Bounded Contexts), el profesional puede resolver problemas reales de negocio y ofrecer soluciones tecnológicas que sean innovadoras, seguras y perdurables en el tiempo.  |

### Objetivos SMART

---

## [Capítulo I: Presentación](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-1.md#cap%C3%ADtulo-i-presentaci%C3%B3n)

### [1.1. Startup Profile](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-1.md#11-startup-profile)
#### [1.1.1. Descripción de la Startup](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-1.md#111-descripci%C3%B3n-de-la-startup)
#### [1.1.2. Perfiles de integrantes del equipo](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-1.md#112-perfiles-de-integrantes-del-equipo)
### [1.2. Solution Profile](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-1.md#12-solution-profile)
#### [1.2.1. Antecedentes y problemática](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-1.md#121-antecedentes-y-problem%C3%A1tica)
#### [1.2.2. Lean UX Process](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-1.md#122-lean-ux-process)
##### [1.2.2.1. Lean UX Problem Statements](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-1.md#1221-lean-ux-problem-statements)
##### [1.2.2.2. Lean UX Assumptions](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-1.md#1222-lean-ux-assumptions)
##### [1.2.2.3. Lean UX Hypothesis Statements](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-1.md#1223-lean-ux-hypothesis-statements)
##### [1.2.2.4. Lean UX Canvas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-1.md#1224-lean-ux-canvas)

### [1.3. Segmentos objetivo](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-1.md#13-segmentos-objetivo)

---


## [Capítulo II: Requirements Development and Software Solution Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#cap%C3%ADtulo-ii-requirements-development-and-software-solution-design)

### [2.1. Competidores](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#21-competidores)
#### [2.1.1. Análisis competitivo](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#211-an%C3%A1lisis-competitivo)
#### [2.1.2. Estrategias y tácticas frente a competidores](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#212-estrategias-y-t%C3%A1cticas-frente-a-competidores)

### [2.2. Entrevistas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#22-entrevistas)
#### [2.2.1. Diseño de entrevistas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#221-dise%C3%B1o-de-entrevistas)
#### [2.2.2. Registro de entrevistas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#222-registro-de-entrevistas)
#### [2.2.3. Análisis de entrevistas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#223-an%C3%A1lisis-de-entrevistas)

### [2.3. Needfinding](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#23-needfinding)
#### [2.3.1. User Personas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#231-user-personas)
#### [2.3.2. User Task Matrix](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#232-user-task-matrix)
#### [2.3.3. User Journey Mapping](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#233-user-journey-mapping)
#### [2.3.4. Empathy Mapping](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#234-empathy-mapping)
#### [2.3.5. Ubiquitous Language](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#235-ubiquitous-language)

### [2.4. Requirements Specification](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#24-requirements-specification)
#### [2.4.1. User Stories](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#241-user-stories)
#### [2.4.2. Impact Mapping](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#242-impact-mapping)
#### [2.4.3. Product Backlog](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#243-product-backlog)

### [2.5. Strategic-Level Domain-Driven Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#25-strategic-level-domain-driven-design)
#### [2.5.1. EventStorming](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#251-eventstorming)
##### [2.5.1.1. Candidate Context Discovery](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#2511-candidate-context-discovery)
##### [2.5.1.2. Domain Message Flows Modeling](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#2512-domain-message-flows-modeling)
##### [2.5.1.3. Bounded Context Canvases](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#2513-bounded-context-canvases)
#### [2.5.2. Context Mapping](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#252-context-mapping)
#### [2.5.3. Software Architecture](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#253-software-architecture)
##### [2.5.3.1. Software Architecture Context Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#2531-software-architecture-context-level-diagrams)
##### [2.5.3.2. Software Architecture Container Level Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#2532-software-architecture-container-level-diagrams)
##### [2.5.3.3. Software Architecture Deployment Diagrams](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#2533-software-architecture-deployment-diagrams)

### [2.6. Tactical-Level Domain-Driven Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#26-tactical-level-domain-driven-design)
#### [2.6.x. Bounded Context: ](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-2.md#26x-bounded-context)

---

## [Capítulo III: Solution UI/UX Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-3.md#cap%C3%ADtulo-iii-solution-uiux-design)

### [3.1. Product Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-3.md#31-product-design)
#### [3.1.1. Style Guidelines](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-3.md#311-style-guidelines)
##### [3.1.1.1. General Style Guidelines](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-3.md#3111-general-style-guidelines)
#### [3.1.2. Information Architecture](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-3.md#312-information-architecture)
##### [3.1.2.1. Organization Systems](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-3.md#3121-organization-systems)
##### [3.1.2.5. Navigation Systems](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-3.md#3125-navigation-systems)
#### [3.1.3. Landing Page UI Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-3.md#313-landing-page-ui-design)
##### [3.1.3.1. Landing Page Wireframe](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-3.md#3131-landing-page-wireframe)
##### [3.1.3.2. Landing Page Mock-up](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-3.md#3132-landing-page-mock-up)
#### [3.1.4. Mobile Applications UX/UI Design](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-3.md#314-mobile-applications-uxui-design)
##### [3.1.4.3. Mobile Applications Mock-ups](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-3.md#3143-mobile-applications-mock-ups)
##### [3.1.4.5. Mobile Applications Prototyping](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-3.md#3145-mobile-applications-prototyping)

---

## [Capítulo IV: Product Implementation & Validation](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-4.md#cap%C3%ADtulo-iv-product-implementation--validation)

### [4.1. Software Configuration Management](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-4.md#41-software-configuration-management)
#### [4.1.1. Software Development Environment Configuration](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-4.md#411-software-development-environment-configuration)
#### [4.1.4. Software Deployment Configuration](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-4.md#414-software-deployment-configuration)

### [4.2. Landing Page & Mobile Application Implementation](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-4.md#42-landing-page--mobile-application-implementation)
#### [4.2.1. Sprint 1](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-4.md#421-sprint-1)
##### [4.2.1.1. Sprint Planning 1](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-4.md#4211-sprint-planning-1)

### [4.3. Validation Interviews](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-4.md#43-validation-interviews)
#### [4.3.1. Diseño de Entrevistas](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/chapter-4.md#431-dise%C3%B1o-de-entrevistas)

---

## Conclusiones

### [Conclusiones y recomendaciones](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/conclusion.md)

---



## [Bibliografía](https://github.com/app-movil-3821/TerraTeam-Project-Report/blob/main/docs/Bibliograpgy.md)