# Capítulo II: Requirements Development and Software Solution Design

## 2.1. Competidores
### 2.1.1. Análisis competitivo
<table border="1" cellpadding="8" cellspacing="0" style="border-collapse:collapse; width:100%; font-family:Arial, sans-serif;">
    <tr>
        <th colspan="7" style="background-color:#d9ead3;">Competitive Analysis Landscape</th>
    </tr>
    <tr>
        <td colspan="2" rowspan="2" style="background-color:#f4cccc;"><strong>¿Por qué llevar a cabo este análisis?</strong></td>
        <td colspan="5">¿Cómo se posiciona ChambaYA frente a sus competidores en cuanto a propuesta de valor, marketing, producto y estrategia?</td>
    </tr>
    <tr>
        <td colspan="5">
            Es un análisis comparativo que permite identificar fortalezas, debilidades, oportunidades y amenazas, así como entender mejor la posición del producto frente a otros actores relevantes del mercado.
        </td>
    </tr>
    <tr>
        <td colspan="3"></td>
        <td style="text-align:center;">
            <strong>ChambaYA</strong><br>
            <img src="../assets/img/Chapter-2/CompetitiveAnalysis-Images/ChambaYa-logo.png" alt="ChambaYA" style="width:100px;">
        </td>
        <td style="text-align:center;">
            <strong>Computrabajo</strong><br>
            <img src="../assets/img/Chapter-2/CompetitiveAnalysis-Images/Computrabajo-logo.png" alt="Computrabajo" style="width:100px;">
        </td>
        <td style="text-align:center;">
            <strong>Time Jobs</strong><br>
            <img src="../assets/img/Chapter-2/CompetitiveAnalysis-Images/TimeJobs-logo.png" alt="Time Jobs" style="width:100px;">
        </td>
        <td style="text-align:center;">
            <strong>Indeed</strong><br>
            <img src="../assets/img/Chapter-2/CompetitiveAnalysis-Images/Indeed-logo.png" alt="Indeed" style="width:100px;">
        </td>
    </tr>
    <tr>
        <td rowspan="2">Perfil</td>
        <td colspan="2">Overview</td>
        <td>Plataforma móvil de contratación inmediata para MYPEs que necesitan cubrir personal temporal de forma urgente mediante geolocalización y matching en tiempo real.</td>
        <td>Bolsa de empleo líder en Perú/LATAM enfocada en vacantes formales y procesos tradicionales de contratación.</td>
        <td>Plataforma de staffing flexible orientada a cubrir necesidades de personal temporal para empresas operativas.</td>
        <td>Motor global de búsqueda de empleo con publicaciones de empresas y postulaciones masivas.</td>
    </tr>
    <tr>
        <td colspan="2">Ventaja competitiva ¿Qué valor ofrece a los clientes?</td>
        <td>Matching hiperlocal inmediato, sin CV, orientado a microturnos y contratación urgente para negocios pequeños.</td>
        <td>Gran base de candidatos y reconocimiento de marca en LATAM.</td>
        <td>Rapidez en provisión de personal temporal para empresas.</td>
        <td>Amplia suite de funcionalidades para gestión clínica y administrativa, integración con sistemas de pago.</td>
    </tr>
    <tr>
        <td rowspan="2">Perfil de Marketing</td>
        <td colspan="2">Mercado objetivo</td>
        <td>MYPEs: restaurantes, bodegas, cafeterías, negocios locales y jóvenes estudiantes/trabajadores flexibles.</td>
        <td>Empresas de todos los tamaños y postulantes de empleo formal. </td>
        <td>Empresas con alta rotación operativa y necesidad temporal estructurada.</td>
        <td>Empresas medianas/grandes y profesionales generales</td>
    </tr>
    <tr>
        <td colspan="2">Estrategias de marketing</td>
        <td>Estrategia: Penetración local en zonas comerciales, alianzas con universidades e incubadoras, marketing hipersegmentado digital.</td>
        <td>Estrategia: SEO, publicidad digital masiva, posicionamiento de marca consolidado.</td>
        <td>Estrategia: Ventas B2B directas y alianzas comerciales empresariales.</td>
        <td>Estrategia: SEO global, pauta digital y posicionamiento internacional.</td>
    </tr>
    <tr>
        <td rowspan="3">Perfil de Producto</td>
        <td colspan="2">Productos & Servicios.</td>
        <td>Productos: App móvil de matching laboral temporal con geolocalización, reputación y chat interno.</td>
        <td>Productos: Portal web/app de bolsa laboral tradicional.</td>
        <td>Productos: Plataforma de staffing / reclutamiento temporal.</td>
        <td>Productos: Portal de empleo web/app.</td>
    </tr>
    <tr>
        <td colspan="2">Precios & Costos</td>
        <td>Precios: Microcomisión por contratación / modelo freemium accesible para MYPEs.</td>
        <td>Precios: Pago por publicación / paquetes de reclutamiento.</td>
        <td>Precios: Pricing empresarial por servicio staffing.</td>
        <td>Precios: Pago por publicación / patrocinio de vacantes.</td>
    </tr>
    <tr>
        <td colspan="2">Canales de distribución (Web y/o Móvil)</td>
        <td>Canales: App móvil (iOS/Android) y plataforma web.</td>
        <td>Canales: Web + móvil.</td>
        <td>Canales: Web + móvil.</td>
        <td>Canales: Web + móvil.</td>
    </tr>
    <tr>
        <td rowspan="5">Análisis SWOT</td>
    <tr>
        <td colspan="2">Fortalezas</td>
        <td>Fortalezas: Especialización en contratación inmediata, modelo hiperlocal, pensado para MYPEs.</td>
        <td>Fortalezas: Gran penetración de mercado y confianza de marca.</td>
        <td>Fortalezas: Buen enfoque en personal temporal.</td>
        <td>Fortalezas: Amplia base de usuarios global.</td>
    </tr>
    <tr>
        <td colspan="2">Debilidades</td>
        <td>Debilidades: Startup nueva, requiere validación de mercado y adquisición de masa crítica.</td>
        <td>Debilidades: No optimizado para urgencias ni microturnos; requiere CV.</td>
        <td>Debilidades: Poco orientado a microempresas pequeñas; enfoque más corporativo.</td>
        <td>Debilidades: No especializado en contratación inmediata/local.</td>
    </tr>
    <tr>
        <td colspan="2">Oportunidades</td>
        <td>Oportunidades: Crecimiento de gig economy y digitalización de MYPEs en Perú/LATAM.</td>
        <td>Oportunidades: Expandir verticales laborales.</td>
        <td>Oportunidades: Penetrar nuevos mercados LATAM.</td>
        <td>Oportunidades: Mantener liderazgo global.</td>
    </tr>
    <tr>
        <td colspan="2">Amenazas</td>
        <td>Amenazas: Entrada de marketplaces globales / dificultad de generar liquidez inicial.</td>
        <td>Amenazas: Nuevos modelos de gig-work más ágiles.</td>
        <td>Amenazas: Nuevas apps hiperlocales especializadas.</td>
        <td>Amenazas: Plataformas nicho más adaptadas al mercado local.</td>
    </tr>
</table>

### 2.1.2. Estrategias y tácticas frente a competidores

| **Análisis FODA cruzado** | **Oportunidades** | **Amenazas** |
|---|---|---|
| **Fortalezas (F)**<br>1. Especialización en contratación inmediata para MYPEs.<br>2. Matching geolocalizado en tiempo real.<br>3. Registro simplificado sin CV mediante sistema tag-based. | **Estrategia (FO) — Estrategias Ofensivas**<br>1. Posicionar a ChambaYA como la primera plataforma especializada en contratación urgente para MYPEs en Perú.<br>2. Implementar campañas de adquisición en zonas comerciales con alta concentración de negocios pequeños.<br>3. Generar alianzas con universidades e institutos para captar oferta laboral juvenil verificada.<br>4. Incentivar primeras contrataciones mediante promociones de lanzamiento y créditos gratuitos para MYPEs. | **Estrategia (FA) — Estrategias Defensivas**<br>1. Reforzar el posicionamiento de nicho especializado frente a plataformas generalistas como Computrabajo/Indeed.<br>2. Priorizar velocidad de matching como principal diferenciador competitivo.<br>3. Construir barreras de salida mediante reputación acumulativa de usuarios.<br>4. Mejorar constantemente UX/UI para reducir fricción frente a competidores más grandes.<br5. Comunicar fuertemente beneficios de inmediatez y cercanía geográfica. |
| **Debilidades (D)**<br>1. Bajo reconocimiento de marca al ser startup nueva.<br>2. Necesidad de masa crítica en ambos lados del marketplace.<br>3. Recursos limitados frente a competidores consolidados.<br>4. Dependencia inicial de adopción en mercados locales específicos.| **Estrategia (DO) — Reorientación**<br>1. Validar el modelo en una zona piloto antes de expansión masiva.<br>2. Ejecutar campañas hiperlocales para alcanzar densidad de usuarios por distrito/zona comercial.<br>3. Implementar programas de referidos para crecimiento orgánico de ambas partes del marketplace.<br>4. Generar contenido educativo para MYPEs sobre beneficios de contratación flexible digital.<br>5. Buscar incubadoras, fondos semilla y alianzas estratégicas para acelerar crecimiento. | **Estrategia (DA) — Supervivencia**<br>1. Priorizar construcción de confianza mediante validación de identidad y sistema reputacional robusto.<br>2. Mantener costos operativos lean para competir durante etapa temprana.<br>3. Enfocar recursos en verticales/rubros donde el pain point sea más fuerte.<br>4. Diseñar estrategia de retención temprana para evitar churn en ambos lados del marketplace.<br>5. Iterar rápidamente el producto con base en feedback continuo del mercado piloto. |

## 2.2. Entrevistas
### 2.2.1. Diseño de entrevistas
<h4 id="Segment" >Segmento objetivo: Contratantes (MYPEs)</h4> 
<h4 id="PreguntPersonal">Preguntas Personales:</h4> 

¿Cuál es su nombre?

¿Cuál es su edad?

¿Cuál es su cargo dentro del negocio?

¿Qué tipo de negocio administra?

¿Cuántos años lleva operando el negocio?

¿Cuántos trabajadores tiene actualmente?


<h4 id="PreguntEspe">Preguntas específicas:</h4> 

¿Con qué frecuencia enfrenta faltas de personal o necesidad de apoyo temporal en su negocio?

¿Cuando necesita cubrir un turno urgente, ¿cómo busca personal actualmente?

¿Cuánto tiempo suele tardar en encontrar a alguien disponible?

¿Qué problemas o frustraciones enfrenta con ese proceso?

¿Qué factores considera más importantes al momento de contratar personal temporal? (confianza, cercanía, experiencia, rapidez, costo, etc.)

¿Ha contratado anteriormente personas sin experiencia formal? ¿Cómo fue esa experiencia?

¿Qué nivel de confianza le generaría contratar mediante una aplicación móvil?

¿Qué funcionalidades consideraría indispensables en una plataforma de contratación inmediata?

¿Estaría dispuesto a pagar una comisión por una contratación rápida y confiable? ¿Bajo qué condiciones?

<h4 id="Segment" >Segmento objetivo: Jóvenes / Trabajadores Temporales </h4> 
<h4 id="PreguntPersonal">Preguntas Personales:</h4> 

¿Cuál es su nombre?

¿Cuál es su edad?

¿Actualmente estudia, trabaja o ambos?

¿Cuál es su ocupación?

¿Dónde reside actualmente?

¿Cuenta con experiencia laboral previa? ¿En qué rubros?


<h4 id="PreguntESP">Preguntas específicas :</h4> 

¿Ha buscado trabajos temporales o de medio tiempo anteriormente?

¿Qué dificultades ha encontrado al buscar este tipo de empleo?

¿Qué tan importante es para usted la flexibilidad horaria al momento de trabajar?

¿Qué tan dispuesto estaría a aceptar trabajos de corta duración por turnos o días?

¿Qué tipo de trabajos operativos estaría dispuesto a realizar? (atención, reparto, inventario, limpieza, etc.)

¿Qué factores considera más importantes al aceptar un trabajo temporal? (pago, cercanía, horario, seguridad, reputación del negocio, etc.)

¿Qué tan cómodo se sentiría usando una app para postular a trabajos rápidos sin CV?

<div style="page-break-after: always;"></div>

### 2.2.2. Registro de entrevistas

#### Segmento 1: 
* Entrevista 1:

| Nombre                         |     |      
|--------------------------------|-----|
| Apellido                       |     |      
| Edad                           |     |      
| Distrito                       |     |      
| Evidencia                      |     |      
| URL                            |     |      
| Inicio de Entrevista           |     |      
| Fin de entrevista              |     |      
| Estado Civil                   |     |      
| Ocupacion                      |     |      
| Dispositivo de preferencia     |     |      
| Canales de interaccion digital |     |     

Resumen: 


* Entrevista 2:

| Nombre                         |     |      
|--------------------------------|-----|
| Apellido                       |     |      
| Edad                           |     |      
| Distrito                       |     |      
| Evidencia                      |     |      
| URL                            |     |      
| Inicio de Entrevista           |     |      
| Fin de entrevista              |     |      
| Estado Civil                   |     |      
| Ocupacion                      |     |      
| Dispositivo de preferencia     |     |      
| Canales de interaccion digital |     |  


#### Segmento 2:
* Entrevista 1:

| Campo                          | Información                                      |
|--------------------------------|--------------------------------------------------|
| Nombre                         | jimena                                           |
| Apellido                       | Bartolo                                         |
| Edad                           | 25 años                                         |
| Distrito                       | La Molina, Lima, Perú                           |
| Evidencia                      | Entrevista grabada (audio/transcripción)        |
| URL                            | *(agregar enlace)*                              |
| Inicio de Entrevista           | ----                                            |
| Fin de entrevista              | ----                                            |
| Estado Civil                   | Soltero                                         |
| Ocupacion                      | Administradora de Mypes                         |
| Dispositivo de preferencia     | Smartphone / Laptop                             |
| Canales de interaccion digital | whatsap                                         |     

Resumen:
Jimena, dueña de un pequeño negocio, mencionó que enfrenta dificultades cuando necesita cubrir turnos de manera urgente, ya que actualmente busca personal a través de conocidos o WhatsApp, lo que le toma entre uno y dos días. Señala que uno de los principales problemas es la falta de confianza y referencias de los trabajadores, además de la pérdida de tiempo en el proceso. Considera importante contar con una solución que le permita encontrar personal disponible de forma rápida, cercana y con buenas calificaciones, y estaría dispuesta a pagar por este servicio si realmente le garantiza eficiencia y confiabilidad


* Entrevista 2:

| Campo                          | Información                                      |
|--------------------------------|--------------------------------------------------|
| Nombre                         | Josué                                           |
| Apellido                       | Arunategui                                      |
| Edad                           | 22 años                                         |
| Distrito                       | Chorrillos, Lima, Perú                          |
| Evidencia                      | Entrevista grabada (audio/transcripción)        |
| URL                            | *(agregar enlace)*                              |
| Inicio de Entrevista           | ----                                            |
| Fin de entrevista              | ----                                            |
| Estado Civil                   | Soltero                                         |
| Ocupacion                      | Administrador de Base de Datos                  |
| Dispositivo de preferencia     | Smartphone / Laptop                             |
| Canales de interaccion digital | Discord                                         |    

Resumen: 
El entrevistado, Josué Arunategui, de 22 años y residente en Chorrillos, trabaja como administrador de base de datos con experiencia en ciencia de datos y retail. Ha buscado trabajos temporales, pero encontró dificultades como falta de confianza en las ofertas, poca claridad en pagos y procesos largos. Valora la flexibilidad horaria y está dispuesto a realizar trabajos cortos si las condiciones son claras y bien remuneradas, prefiriendo actividades relacionadas a TI. Considera importantes la cercanía, seguridad, horario flexible y reputación del empleador. Además, se sentiría cómodo usando una app para postular, siempre que sea confiable y transparente.



### 2.2.3. Análisis de entrevistas

## 2.3. Needfinding
### 2.3.1. User Personas
### 2.3.2. User Task Matrix
|                  |                    |                    |
|------------------|--------------------|--------------------|
|                  |                    |                    |
|                  |                    |                    |
|                  |                    |                    |
|                  |                    |                    |
|                  |                    |                    |
|                  |                    |                    |
|                  |                    |                    |
|                  |                    |                    |
|                  |                    |                    |
|                  |                    |                    |
|                  |                    |                    |
### 2.3.3. User Journey Mapping
### 2.3.4. Empathy Mapping
### 2.3.5. Ubiquitous Language
En el presente proyecto, orientado a optimizar la conexión entre micro y pequeñas empresas (MYPEs) y jóvenes que buscan oportunidades laborales temporales mediante una plataforma digital, se ha definido un lenguaje ubicuo que permite establecer una comprensión común entre todos los actores involucrados, incluyendo usuarios, desarrolladores y stakeholders.

La adopción de este lenguaje compartido resulta fundamental para describir de manera clara y consistente los conceptos clave del dominio, reduciendo posibles ambigüedades y facilitando la comunicación a lo largo de todo el proceso de desarrollo del sistema.

A continuación, se presentan los principales términos definidos:

| Término | Descripción |
|--------|------------|
| Chambeador | Usuario joven o estudiante que se registra en la plataforma para encontrar trabajos temporales o turnos cortos. |
| Contratante | Dueño, administrador o representante de una MYPE que publica turnos de trabajo en la plataforma. |
| Turno | Trabajo temporal o tarea específica que debe ser cubierta en un periodo corto de tiempo. |
| Mini-job | Trabajo de corta duración, generalmente por horas o por un día, enfocado en tareas operativas. |
| Match | Proceso mediante el cual la plataforma conecta un turno publicado con un chambeador disponible. |
| Tags de habilidades | Etiquetas que representan las habilidades del chambeador (ej. atención al cliente, inventario, reparto). |
| Insignia de confianza | Verificación del perfil del usuario mediante correo institucional u otro mecanismo de validación. |
| Geolocalización | Funcionalidad que permite ubicar a los usuarios en tiempo real para conectar ofertas y demandas cercanas. |
| Sistema de reputación | Mecanismo de calificación basado en estrellas que permite evaluar la experiencia entre usuarios. |
| Chat interno | Canal de comunicación dentro de la plataforma que permite coordinar detalles del turno sin compartir datos personales. |
| Publicación de turno | Acción realizada por el contratante para registrar un nuevo trabajo disponible en la plataforma. |
| Aceptación de turno | Acción mediante la cual un chambeador selecciona y confirma su participación en un turno. |

## 2.4. Requirements Specification
### 2.4.1. User Stories

En esta sección se presentan las historias de usuario que permiten describir las principales funcionalidades del sistema desde la perspectiva de sus usuarios. Estas historias se construyen a partir del análisis del problema, los segmentos objetivo y las necesidades identificadas en el contexto de la plataforma.

Las historias de usuario han sido organizadas en épicas para facilitar la comprensión de los distintos componentes funcionales del sistema. De esta manera, se agrupan funcionalidades relacionadas con la gestión de los chambeadores, los contratantes y los mecanismos de interacción y confianza dentro de la plataforma. Cada historia refleja situaciones reales que buscan resolverse, como la necesidad de cubrir turnos de manera inmediata, acceder a oportunidades laborales cercanas y garantizar una experiencia segura para ambas partes.

| Story ID | Título | Descripción | Criterios de Aceptación (Gherkin) |
|----------|--------|------------|-----------------------------------|
| **EP01** | **Título:** Gestión de Chambeadores | **Descripción:** Permite a los jóvenes registrarse, crear su perfil basado en habilidades y acceder a oportunidades laborales temporales cercanas de manera rápida y sin necesidad de un CV. | |
| US01 | Registro ágil de chambeador | Como chambeador, quiero registrarme de forma rápida en la plataforma, para acceder inmediatamente a oportunidades laborales sin procesos complejos. | Escenario 1: Registro exitoso  Dado que el usuario ingresa sus datos correctamente  Cuando confirma el registro  Entonces su cuenta se crea exitosamente  Escenario 2: Error en datos  Dado que el usuario ingresa datos incompletos  Cuando intenta registrarse  Entonces el sistema muestra un mensaje de error |
| US02 | Perfil sin CV basado en habilidades | Como chambeador, quiero crear un perfil mediante etiquetas de habilidades sin necesidad de un CV, para acceder a trabajos sin barreras de experiencia formal. | Escenario 1: Creación de perfil  Dado que el usuario selecciona sus habilidades  Cuando guarda su perfil  Entonces el sistema registra correctamente las etiquetas |
| US03 | Visualización de turnos cercanos en tiempo real | Como chambeador, quiero visualizar turnos disponibles en un radio cercano a mi ubicación en tiempo real, para reducir el tiempo de traslado y acceder a oportunidades inmediatas. | Escenario 1: Turnos disponibles  Dado que existen turnos cercanos  Cuando el usuario accede a la plataforma  Entonces visualiza las opciones en su zona |
| US04 | Aceptación inmediata de turnos | Como chambeador, quiero aceptar turnos disponibles de forma inmediata, para generar ingresos el mismo día de manera flexible. | Escenario 1: Aceptación exitosa  Dado que el turno está disponible  Cuando el usuario lo acepta  Entonces queda asignado al turno |
| US05 | Evaluación del contratante | Como chambeador, quiero visualizar la reputación del contratante antes de aceptar un turno, para asegurar una experiencia laboral confiable. | Escenario 1: Visualización de reputación  Dado que el contratante tiene calificaciones  Cuando el usuario revisa el perfil  Entonces puede ver su puntuación |
| **EP02** | **Título:** Gestión de Contratantes (MYPEs) | **Descripción:** Permite a las micro y pequeñas empresas registrarse, publicar turnos de trabajo de manera ágil y encontrar trabajadores disponibles cercanos para cubrir necesidades urgentes. | |
| US06 | Registro de contratante | Como contratante, quiero registrarme en la plataforma, para poder gestionar la contratación de personal temporal. | Escenario 1: Registro exitoso  Dado que el usuario completa sus datos  Cuando confirma el registro  Entonces su cuenta es creada correctamente |
| US07 | Publicación rápida de turnos | Como contratante, quiero publicar turnos en pocos pasos, para cubrir ausencias inesperadas sin afectar la operación del negocio. | Escenario 1: Publicación exitosa  Dado que el usuario ingresa los datos del turno  Cuando lo publica  Entonces el turno es visible en la plataforma |
| US08 | Búsqueda de trabajadores cercanos | Como contratante, quiero visualizar trabajadores disponibles cercanos en tiempo real, para contratar a alguien que pueda llegar rápidamente. | Escenario 1: Trabajadores disponibles  Dado que existen trabajadores cercanos  Cuando accede a la plataforma  Entonces puede ver perfiles disponibles |
| US09 | Selección basada en confianza | Como contratante, quiero seleccionar trabajadores basándome en su reputación y habilidades, para asegurar un servicio confiable. | Escenario 1: Selección exitosa  Dado que el trabajador tiene calificaciones visibles  Cuando el contratante lo selecciona  Entonces queda asignado al turno |
| US10 | Reducción del tiempo de contratación | Como contratante, quiero cubrir un turno en el menor tiempo posible, para evitar pérdidas operativas durante picos de demanda. | Escenario 1: Cobertura rápida  Dado que el turno es urgente  Cuando se publica  Entonces es aceptado en corto tiempo |
| **EP03** | **Título:** Comunicación y Confianza | **Descripción:** Permite la interacción entre usuarios mediante herramientas de comunicación y un sistema de reputación que garantiza confianza y seguridad en la plataforma. | |
| US11 | Comunicación mediante chat interno | Como usuario, quiero comunicarme mediante un chat interno, para coordinar detalles del turno sin compartir información personal. | Escenario 1: Chat habilitado  Dado que el turno fue aceptado  Cuando los usuarios acceden  Entonces pueden intercambiar mensajes |
| US12 | Sistema de reputación bidireccional | Como usuario, quiero calificar al otro usuario después de finalizar el turno, para contribuir a un sistema de confianza dentro de la plataforma. | Escenario 1: Calificación registrada  Dado que el turno ha finalizado  Cuando el usuario califica  Entonces la puntuación se guarda correctamente |

### 2.4.2. Impact Mapping
### 2.4.3. Product Backlog

## 2.5. Strategic-Level Domain-Driven Design
### 2.5.1. EventStorming
##### 2.5.1.1. Candidate Context Discovery
##### 2.5.1.2. Domain Message Flows Modeling
##### 2.5.1.3. Bounded Context Canvases
### 2.5.2. Context Mapping
### 2.5.3. Software Architecture
##### 2.5.3.1. Software Architecture Context Level Diagrams
##### 2.5.3.2. Software Architecture Container Level Diagrams
##### 2.5.3.3. Software Architecture Deployment Diagrams

## 2.6. Tactical-Level Domain-Driven Design
### 2.6.x. Bounded Context: `<Nombre del Contexto>`
##### 2.6.x.1. Domain Layer
##### 2.6.x.2. Interface Layer
##### 2.6.x.3. Application Layer
##### 2.6.x.4. Infrastructure Layer
##### 2.6.x.5. Bounded Context Software Architecture Component Level Diagrams
##### 2.6.x.6. Bounded Context Software Architecture Code Level Diagrams
###### 2.6.x.6.1. Bounded Context Domain Layer Class Diagrams
###### 2.6.x.6.2. Bounded Context Database Design Diagram
