<div style="page-break-before: always;"></div>

# Conclusiones

## Conclusiones y recomendaciones

El desarrollo del proyecto ChambaYA permitió validar que el problema planteado inicialmente es real y relevante: tanto las entrevistas de Needfinding (Capítulo II) como las entrevistas de validación del prototipo (Capítulo IV) confirmaron que las MYPEs pierden tiempo y oportunidades de venta al cubrir turnos de emergencia mediante métodos informales (conocidos, WhatsApp, carteles), mientras que los jóvenes enfrentan barreras de acceso al mercado laboral por la exigencia de un CV o de experiencia previa. El 100% de los contratantes entrevistados manifestó dificultades de confianza y lentitud al buscar personal, y el 100% de los jóvenes entrevistados valoró la rapidez y flexibilidad como factores decisivos, lo que confirma la pertinencia del modelo de matching hiperlocal sin CV propuesto por la startup.

En cuanto a la propuesta de solución, las hipótesis de Lean UX definidas en el Capítulo I se vieron parcialmente validadas durante las entrevistas de validación del prototipo en el Sprint 1. Los entrevistados destacaron positivamente el sistema de perfiles basado en habilidades (tags) en lugar de CV, la geolocalización para encontrar turnos cercanos, el chat interno para coordinar sin compartir datos personales y la "Insignia de Confianza" universitaria como mecanismo de seguridad para las MYPEs al contratar desconocidos. Esto respalda la dirección estratégica del producto y sugiere que, de cara a los siguientes sprints, se debe seguir reforzando estos diferenciadores frente a competidores generalistas como Computrabajo, Indeed o Time Jobs, identificados en el análisis competitivo del Capítulo II.

A nivel de implementación, el equipo logró desplegar una primera versión funcional de los tres componentes del producto: el Landing Page en GitHub Pages, el Backend API en Railway con Java, Spring Boot y MongoDB Atlas, y las pantallas principales de la aplicación móvil nativa en Kotlin con Jetpack Compose. El diseño táctico bajo Domain-Driven Design, con bounded contexts diferenciados para IAM, Jobs, Enrollments/Application y Communication, permitió distribuir el trabajo entre los integrantes y mantener una arquitectura desacoplada que facilita la incorporación de nuevas funcionalidades en sprints futuros, como el Payment Context, que aún no fue implementado.

Por otro lado, la evaluación heurística realizada sobre el prototipo (Capítulo IV) identificó tres problemas de usabilidad que deben atenderse antes de avanzar con nuevas funcionalidades: sobrecarga de información en la vista de turnos, falta de una vía de retorno clara en pantallas de nivel superior y una iconografía ambigua en la barra de navegación inferior (particularmente el ícono de "Shifts"). Se recomienda priorizar estas correcciones en el próximo sprint, ya que afectan directamente la libertad y el control del usuario, dos heurísticas de usabilidad fundamentales para la retención de ambos segmentos.

Como recomendaciones generales para la continuidad del proyecto, se sugiere: (1) ampliar la suite de pruebas del backend más allá del test de contexto inicial, incorporando Unit Tests por bounded context y Acceptance Tests en Gherkin como se planificó en el Capítulo IV; (2) iniciar la medición de los Business y User Outcomes definidos en el Lean UX Canvas (tiempo de cobertura de turnos, tasa de recurrencia mensual, calificación promedio) una vez la aplicación esté en un entorno con usuarios reales; y (3) mantener la coordinación lograda entre los subequipos de Landing Page, Backend y Aplicación Móvil mediante GitFlow, ya que fue un factor clave para entregar un avance funcional e integrado en el primer sprint. En conjunto, el equipo demostró capacidad para validar un problema real, diseñar una solución coherente con DDD y Lean UX, e implementar un primer incremento de producto desplegado y verificado, sentando una base sólida para los sprints restantes del proyecto.

## Video App Validation

## Video About the Product

El video "About the Product" presenta de manera clara y atractiva la propuesta de valor de ChambaYa, los problemas que resuelve y cómo funciona la solución para ambos segmentos objetivo.



| Titulo del Video        | Foundly Product               |
|-------------------------|-------------------------------|
| Duracion                | 1 miunto                      |
| Fecha de Grabacion      | 21/06/2026                    |
| URL de Youtube          | https://youtu.be/WrObe5WUI10  |
| URL de Microsoft Stream | https://shorturl.at/NwXQ7    |

Screenshot del video "About the Product" :

![aboutChamba.png](../assets/img/conclusiones/aboutChamba.png)
## Video About the Team

El video "About the team" presenta de manera clara y concisa, la sinceridad de los integrantes en la participacion del proyecto.

| Titulo del Video        | Foundly Product              |
|-------------------------|------------------------------|
| Duracion                | 7 minutos 39 segundos        |
| Fecha de Grabacion      | 21/06/2026                   |
| URL de Youtube          | https://youtu.be/QSkAFHBTf2k |
| URL de Microsoft Stream | https://shorturl.at/6QJte    |

Screenshot del video "About the Team" :

![about.png](../assets/img/conclusiones/about.png)

---

# Glosario

Para la definición de los términos del dominio (Chambeador, Contratante, Turno, Match, Tags de habilidades, Insignia de confianza, entre otros) se utilizó el Ubiquitous Language definido en la sección [2.3.5](../docs/chapter-2.md#235-ubiquitous-language) del reporte. A continuación, se listan los enlaces de referencia a los repositorios, herramientas y entornos desplegados del proyecto que sirven como respaldo y fuente de consulta de dichos términos:

- Organización en GitHub: https://github.com/app-movil-3821
- Repositorio del Project Report: https://github.com/app-movil-3821/TerraTeam-Project-Report
- Repositorio de la aplicación móvil (ChambaYa-Kotlin): https://github.com/app-movil-3821/ChambaYa-Kotlin
- Repositorio del Backend API (Backend-ChambaYa): https://github.com/app-movil-3821/Backend-ChambaYa
- Landing Page desplegado: https://app-movil-3821.github.io/LandingPageChambaYa/
- Backend API desplegado / Swagger UI: https://backend-chambaya-production-b2e5.up.railway.app/swagger-ui/index.html
- Tablero de Trello (Product Backlog): 
---

# Bibliografía

A continuación, se listan las fuentes citadas en el Capítulo I para sustentar la problemática y los antecedentes del proyecto:


- Arcos Dorados. (2025). *Estudio sobre empleabilidad juvenil en Lima*.


- ComexPerú. (2025). *Reporte MYPE: estructura empresarial, empleo e informalidad en el Perú*. Sociedad de Comercio Exterior del Perú.


- Ministerio de la Producción [PRODUCE]. (2023). *Estadísticas de la micro y pequeña empresa: informalidad por segmento empresarial*.


- Ministerio de la Producción [PRODUCE]. (2025). *Estadísticas de la MYPE: participación en el empleo y en el tejido empresarial del Perú*.
