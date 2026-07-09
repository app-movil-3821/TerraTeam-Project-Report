<div style="page-break-before: always;"></div>

# Conclusiones

## Conclusiones y recomendaciones

### 1. Validación de Problem Statements y Supuestos

El Problem Statement inicial identificó una desconexión estructural entre las MYPEs que necesitan personal temporal y los jóvenes que buscan ingresos flexibles. A lo largo del desarrollo de ChambaYa, esta problemática se confirmó como real y relevante. El supuesto de que las MYPEs estarían dispuestas a contratar jóvenes sin CV formal, siempre que existiera un filtro de confianza, fue validado mediante la implementación de la Insignia de Confianza universitaria basada en correo institucional (.edu.pe). Asimismo, el supuesto de que eliminar la fricción del CV aumentaría el registro de jóvenes se validó con el sistema de etiquetas de habilidades Tag-Based, que redujo significativamente la barrera de entrada al mercado laboral.

### 2. Contrastación de Hipótesis

- **Hipótesis 1 (Geolocalización):** El motor de geolocalización implementado en la app permite visualizar turnos cercanos en tiempo real. La funcionalidad fue desarrollada tanto en la versión Kotlin como Flutter, mostrando disponibilidad inmediata de turnos por zona. Su efectividad real dependerá de alcanzar masa crítica de usuarios en producción.

- **Hipótesis 2 (Registro sin CV):** El perfil Tag-Based se implementó exitosamente, permitiendo a los jóvenes registrar habilidades de forma rápida sin necesidad de documentación formal. El onboarding simplificado reduce la fricción y el abandono durante el registro.

- **Hipótesis 3 (Insignia de Confianza):** La verificación mediante correo institucional fue integrada en el backend y se muestra visualmente en el perfil del chambeador. Esta funcionalidad responde directamente a la desconfianza de las MYPEs hacia candidatos sin historial laboral formal.

- **Hipótesis 4 (Sistema de Calificaciones):** Se diseñó la arquitectura del sistema de reputación bidireccional. Su validación real requiere usuarios activos completando turnos, por lo que constituye una métrica pendiente de medición en producción.

### 3. Cumplimiento de Criterios de Éxito

Se logró desplegar una solución multiplataforma funcional (Kotlin para Android y Flutter multiplataforma) conectada a un backend en producción desplegado en Railway. Las funcionalidades core fueron implementadas: publicación de turnos, postulación, aceptación/rechazo de chambeadores, geolocalización y gestión de perfil. Sin embargo, métricas como la tasa de aceptación en menos de 2 horas o la recurrencia del 30% de MYPEs requieren validación en un entorno real con usuarios activos, lo cual constituye el siguiente paso natural del proyecto.

---

## Recomendaciones

- **Sistema de Notificaciones Push en Tiempo Real:** Durante el desarrollo se identificó que la inmediatez es el valor central de ChambaYa. Se recomienda implementar notificaciones push (Firebase Cloud Messaging) para alertar a los chambeadores cercanos en el momento exacto en que se publica un turno, reduciendo el tiempo de respuesta y acercándose a la meta del 60% de aceptaciones en menos de 2 horas.

- **Implementación del Sistema de Calificaciones:** El módulo de reseñas bidireccionales es una funcionalidad crítica pendiente. Se recomienda priorizarlo en el siguiente sprint, ya que es el pilar que sostiene la confianza del ecosistema y la recurrencia de las MYPEs, ambas métricas de éxito definidas en los Business Outcomes.

- **Chat Interno Temporal:** Se recomienda desarrollar el módulo de mensajería interna que se active únicamente cuando un turno es aceptado. Esto elimina la necesidad de compartir datos personales y profesionaliza la comunicación dentro de la plataforma, validando el supuesto de preferencia por coordinación interna sobre WhatsApp.

- **Onboarding Mejorado con Tutorial Interactivo:** Las pruebas de desarrollo mostraron que ciertas funcionalidades como la selección de ubicación en mapa o la gestión de postulantes pueden resultar poco intuitivas para usuarios nuevos. Se recomienda agregar un flujo de onboarding guiado con tooltips y pantallas de bienvenida diferenciadas por rol (Chambeador vs Contratante).

- **Módulo de Pagos y Billetera Digital:** La funcionalidad de Billetera está presente en la navegación pero pendiente de implementación. Se recomienda integrar una pasarela de pagos (como Culqi o Niubiz, orientadas al mercado peruano) para cerrar el ciclo económico dentro de la app, permitiendo que el chambeador reciba su pago el mismo día, que es uno de los User Outcomes principales definidos en el Lean UX.

## Video App Validation

Video de validacion de producto: https://shorturl.at/Xhf2v

## Video Team   

Video Exposicion: https://short-url.cc/1tgKH


## Video About the Product

El video "About the Product" presenta de manera clara y atractiva la propuesta de valor de ChambaYa, los problemas que resuelve y cómo funciona la solución para ambos segmentos objetivo.



| Titulo del Video        | Foundly Product               |
|-------------------------|-------------------------------|
| Duracion                | 1 minuto                      |
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
- Backend API desplegado / Swagger UI: https://backend-chambaya-production-a24a.up.railway.app/swagger-ui/index.html
- Tablero de Trello (Product Backlog): 
---

# Bibliografía

A continuación, se listan las fuentes citadas en el Capítulo I para sustentar la problemática y los antecedentes del proyecto:

<ul>
  <li>
    Adzic, G. (s.f.). <em>Impact Mapping</em>. 
    Recuperado de <a href="https://www.impactmapping.org/">https://www.impactmapping.org/</a>
  </li>
  <li>
    Angular. (s.f.). <em>Angular Coding Style Guide</em>. 
    Recuperado de <a href="https://angular.io/guide/styleguide">https://angular.io/guide/styleguide</a>
  </li>
  <li>
    Brandolini, A. (s.f.). <em>Introducing EventStorming</em>. 
    Recuperado de <a href="https://www.eventstorming.com/">https://www.eventstorming.com/</a>
  </li>
  <li>
    CareerFoundry. (s.f.). <em>What are User Flows in User Experience (UX) Design?</em>. 
    Recuperado de <a href="https://careerfoundry.com/en/blog/ux-design/what-are-user-flows/">https://careerfoundry.com/en/blog/ux-design/what-are-user-flows/</a>
  </li>
  <li>
    Cohn, M. (s.f.). <em>User Stories</em>. Mountain Goat Software. 
    Recuperado de <a href="https://www.mountaingoatsoftware.com/agile/user-stories">https://www.mountaingoatsoftware.com/agile/user-stories</a>
  </li>
  <li>
    Cone, M. (s.f.). <em>The Markdown Guide</em>. 
    Recuperado de <a href="https://www.markdownguide.org/">https://www.markdownguide.org/</a>
  </li>
  <li>
    Conventional Commits. (s.f.). <em>Conventional Commits</em>. 
    Recuperado de <a href="https://www.conventionalcommits.org/">https://www.conventionalcommits.org/</a>
  </li>
  <li>
    Cucumber. (s.f.). <em>Gherkin Reference</em>. 
    Recuperado de <a href="https://cucumber.io/docs/gherkin/reference/">https://cucumber.io/docs/gherkin/reference/</a>
  </li>
  <li>
    Driessen, V. (2010). <em>A successful Git branching model</em>. nvie.com. 
    Recuperado de <a href="https://nvie.com/posts/a-successful-git-branching-model/">https://nvie.com/posts/a-successful-git-branching-model/</a>
  </li>
  <li>
    DZone. (s.f.). <em>Acceptance Criteria in Scrum: Explanation, Examples, and Template</em>. 
    Recuperado de <a href="https://dzone.com/articles/acceptance-criteria-in-software-explanation-exampl">https://dzone.com/articles/acceptance-criteria-in-software-explanation-exampl</a>
  </li>
  <li>
    Evans, E. (2004). <em>Domain-Driven Design: Tackling Complexity in the Heart of Software</em>. Addison-Wesley Professional.
    Recuperado de <a href="https://www.oreilly.com/library/view/domain-driven-design-tackling/0321125215/">https://www.oreilly.com/library/view/domain-driven-design-tackling/0321125215/</a>
  </li>
  <li>
    Fowler, M. (2006). <em>Ubiquitous Language</em>. 
    Recuperado de <a href="https://martinfowler.com/bliki/UbiquitousLanguage.html">https://martinfowler.com/bliki/UbiquitousLanguage.html</a>
  </li>
  <li>
    Google. (s.f.). <em>Google HTML/CSS Style Guide</em>. 
    Recuperado de <a href="https://google.github.io/styleguide/htmlcssguide.html">https://google.github.io/styleguide/htmlcssguide.html</a>
  </li>
  <li>
    Google. (s.f.). <em>Google JavaScript Style Guide</em>. 
    Recuperado de <a href="https://google.github.io/styleguide/jsguide.html">https://google.github.io/styleguide/jsguide.html</a>
  </li>
  <li>
    Google. (s.f.). <em>Google TypeScript Style Guide</em>. 
    Recuperado de <a href="https://google.github.io/styleguide/tsguide.html">https://google.github.io/styleguide/tsguide.html</a>
  </li>
  <li>
    Google. (s.f.). <em>Google Java Style Guide</em>. 
    Recuperado de <a href="https://google.github.io/styleguide/javaguide.html">https://google.github.io/styleguide/javaguide.html</a>
  </li>
  <li>
    Gothelf, J., & Seiden, J. (2021). <em>Lean UX: Designing Great Products with Agile Teams</em> (3rd ed.). O'Reilly Media.
    Recuperado de <a href="https://www.oreilly.com/library/view/lean-ux-2nd/9781491953594/">https://www.oreilly.com/library/view/lean-ux-2nd/9781491953594/</a>
  </li>
  <li>
    HubSpot. (s.f.). <em>Full List of Meta Tags, Why They Matter for SEO & How to Write Them</em>. 
    Recuperado de <a href="https://blog.hubspot.com/marketing/meta-tags">https://blog.hubspot.com/marketing/meta-tags</a>
  </li>
  <li>
    IBM Design. (s.f.). <em>Empathy Map</em>. Enterprise Design Thinking. 
    Recuperado de <a href="https://www.ibm.com/design/thinking/page/toolkit/activity/empathy-map">https://www.ibm.com/design/thinking/page/toolkit/activity/empathy-map</a>
  </li>
  <li>
    IBM Design. (s.f.). <em>As-is Scenario Map</em>. Enterprise Design Thinking. 
    Recuperado de <a href="https://www.ibm.com/design/thinking/page/toolkit/activity/as-is-scenario-map">https://www.ibm.com/design/thinking/page/toolkit/activity/as-is-scenario-map</a>
  </li>
  <li>
    Martin, R. C. (2017). <em>Clean Architecture: A Craftsman's Guide to Software Structure and Design</em>. Prentice Hall.
    Recuperado de <a href="https://www.oreilly.com/library/view/clean-architecture-a/9780134494272/">https://www.oreilly.com/library/view/clean-architecture-a/9780134494272/</a>
  </li>
  <li>
    Mendel, J. (s.f.). <em>Seriously, what's your (startup's) problem?</em>. Medium. 
    Recuperado de <a href="https://medium.com/@jakemendel/seriously-whats-your-startup-s-problem-b3a884c54ab4">https://medium.com/@jakemendel/seriously-whats-your-startup-s-problem-b3a884c54ab4</a>
  </li>
  <li>
    Nielsen Norman Group. (1994). <em>10 Usability Heuristics for User Interface Design</em>. 
    Recuperado de <a href="https://www.nngroup.com/articles/ten-usability-heuristics/">https://www.nngroup.com/articles/ten-usability-heuristics/</a>
  </li>
  <li>
    Nielsen Norman Group. (2016). <em>The Four Dimensions of Tone of Voice</em>. 
    Recuperado de <a href="https://www.nngroup.com/articles/tone-of-voice-dimensions/">https://www.nngroup.com/articles/tone-of-voice-dimensions/</a>
  </li>
  <li>
    Preston-Werner, T. (s.f.). <em>Semantic Versioning 2.0.0</em>. 
    Recuperado de <a href="https://semver.org/">https://semver.org/</a>
  </li>
  <li>
    Progressa Lean. (s.f.). <em>5W+2H - Técnica de análisis de problemas</em>. 
    Recuperado de <a href="https://www.progressalean.com/5w2h-tecnica-de-analisis-de-problemas/">https://www.progressalean.com/5w2h-tecnica-de-analisis-de-problemas/</a>
  </li>
  <li>
    Refactoring.Guru. (s.f.). <em>Design Patterns</em>. 
    Recuperado de <a href="https://refactoring.guru/es/design-patterns">https://refactoring.guru/es/design-patterns</a>
  </li>
  <li>
    Spring. (s.f.). <em>Spring Boot Reference Documentation</em>. 
    Recuperado de <a href="https://docs.spring.io/spring-boot/docs/current/reference/html/">https://docs.spring.io/spring-boot/docs/current/reference/html/</a>
  </li>
  <li>
    UXPressia. (s.f.). <em>User vs. Buyer Persona: Differences and free template</em>. 
    Recuperado de <a href="https://uxpressia.com/blog/user-persona-vs-buyer-persona-difference">https://uxpressia.com/blog/user-persona-vs-buyer-persona-difference</a>
  </li>
  <li>
    Vernon, V. (2016). <em>Domain-Driven Design Distilled</em>. Addison-Wesley Professional.
    Recuperado de <a href="https://www.oreilly.com/library/view/domain-driven-design-distilled/9780134434964/">https://www.oreilly.com/library/view/domain-driven-design-distilled/9780134434964/</a>
  </li>
  <li>
    Vernon, V. (s.f.). <em>Domain-Driven Design Reference</em>. 
    Recuperado de <a href="https://domainlanguage.com/ddd/reference/">https://domainlanguage.com/ddd/reference/</a>
  </li>
</ul>
