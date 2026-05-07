## Capítulo IV: Product Implementation & Validation

### 4.1. Software Configuration Management

En esta sección, se detalla la configuración de la tecnología a usar en el ciclo de vida de desarrollo del proyecto del curso.

#### 4.1.1. Software Development Environment Configuration

En esta sección, se explica los entornos en donde se decidió llevar a cabo el ciclo de vida de desarrollo de los productos de software relacionados al proyecto del curso.

* **Project Management**

    - Para la gestión de reuniones del equipo, se utiliza la aplicación **Google Meet** para el desarrollo de reuniones que incluyen sprint planning, daily scrum y retrospective meeting. En dichas reuniones se tratan temas de planeamiento y gestión de avances para cada sprint planificado a lo largo del ciclo de vida del proyecto.
    - Para la documentación del proyecto, se usa el lenguaje **Markdown** (.md) para la creación de archivos de documentación donde se detallan los procesos correspondientes al ciclo de vida de la solución.
    - Para el control de versiones de todos los productos de software y la documentación general del proyecto, se usa **GitHub** para almacenar los repositorios, y **Git** para el trabajo colaborativo usando ramas y control de versiones.

* **Requirements Management**

    - Para la gestión de los requisitos del producto y su avance, incluyendo historias de usuario, criterios de aceptación, product backlog y sprint backlog, se utiliza **Trello**. Esta herramienta permite estructurar y visualizar las tareas del sprint actual y el progreso del equipo.

* **Product UX/UI Design**

    - Para el diseño de interfaces de usuario, incluyendo wireframes, mockups y prototipos de la aplicación móvil y la landing page, se utiliza **Figma**. Esta herramienta permite al equipo trabajar colaborativamente con elementos visuales, colores e imágenes para diseñar las diversas pantallas de la aplicación.

* **Software Development**

    - Para el desarrollo de la aplicación móvil nativa para Android, se utiliza el IDE **Android Studio** con el lenguaje **Kotlin** y la herramienta **Jetpack Compose** para el desarrollo declarativo de interfaces de usuario. Además, se utiliza **Gradle** como sistema de empaquetado.

    - Para el desarrollo del backend de la aplicación, se utiliza **Java** con el framework **Spring Boot** y la base de datos **MongoDB**, gestionada mediante el cliente **MongoDB Compass** para la verificación de colecciones y documentos.

    - Para el desarrollo del Landing Page, se utilizan los lenguajes **HTML**, **CSS** y **JavaScript** con el IDE **WebStorm** de JetBrains.

    - Para el control de versiones de todos los productos, se utiliza **GitFlow** como workflow de trabajo colaborativo con ramas diferenciadas para el desarrollo paralelo.

* **Software Testing**

    - Las pruebas de la aplicación móvil Android se realizarán mediante el **emulador de Android Studio** y dispositivos físicos, lo que permite validar el correcto funcionamiento de la interfaz, las interacciones táctiles y el rendimiento en distintas condiciones de hardware.

    - Las pruebas del backend se realizarán mediante **Postman**, herramienta que permite ejecutar solicitudes HTTP de manera visual, verificar respuestas del servidor, analizar códigos de estado y validar el correcto funcionamiento de los endpoints expuestos. Además, se utilizará **JUnit 5** (JUnit Jupiter) junto con la anotación `@SpringBootTest` para la ejecución de pruebas unitarias e integración del contexto de Spring Boot, asegurando que cada componente funcione correctamente dentro del ciclo de vida de la aplicación.

* **Software Deployment**

    - Para el despliegue del Landing Page se utiliza el servicio **GitHub Pages**, que permite publicar el sitio web de forma sencilla y accesible mediante un enlace directo, con soporte para despliegue continuo en cada versión lista.

    - Para el despliegue de la aplicación móvil se utilizará **Firebase App Distribution**, servicio de Google que permite distribuir la aplicación a testers e invitar a personas a probarla antes del lanzamiento oficial.

    - Para el despliegue del backend se utilizará **MongoDB Atlas** para la base de datos, publicando las colecciones en un cluster en la nube y conectándolo con la API mediante la cadena de conexión del cluster.

---

#### 4.1.2. Source Code Management

En esta sección, se describe el esquema de organización para el seguimiento efectivo de las modificaciones realizadas al código fuente de los productos de software de ChambaYA. Para ello, se usa **GitHub** como plataforma para el sistema de versiones de cada producto. Además, se usa **GitFlow** como workflow para el control de versiones y el uso de ramas diferenciadas para el trabajo paralelo del proyecto.

### Repositorios

A continuación, se presentan los enlaces públicos para acceder a los repositorios en GitHub donde se almacenan los archivos y avances del proyecto:

* **Informe del Proyecto:** https://github.com/app-movil-3821/TerraTeam-Project-Report
* **Mobile Android Native Application (Kotlin):** https://github.com/app-movil-3821/ChambaPe-kotlin
* **Backend API:** https://github.com/app-movil-3821/Backend-ChambaYa

### GitFlow

Para el desarrollo de este proyecto se utiliza **GitFlow**, herramienta que ayuda al equipo de desarrollo a gestionar efectivamente las versiones de cada producto de software. A continuación, se detallan los tipos de ramas utilizadas:

#### Ramas Principales

* **Main Branch**: Rama creada por defecto al inicializar el repositorio en GitHub. En ella se publican las versiones funcionales al finalizar cada sprint de desarrollo. No se realizan modificaciones directamente en esta rama; los cambios solo llegan desde ramas de tipo `hotfix` o `release`.

* **Develop Branch**: Rama principal para el desarrollo del proyecto. Contiene las funcionalidades integradas desde las ramas de tipo `feature`. Es equivalente a la etapa de pre-producción. Los cambios directos no se realizan en esta rama, sino que provienen de ramas `feature` o `bugfix`.

#### Ramas de Soporte

* **Feature Branch**: En esta rama se desarrollan todas las funcionalidades del producto. Se crea una rama por cada funcionalidad para permitir el desarrollo paralelo. Las ramas se nombran con el prefijo `feature/` seguido de la temática: por ejemplo, `feature/auth`, `feature/job-posting`, `feature/geolocation`.

* **Release Branch**: En esta rama se prepara una nueva versión de despliegue. Solo recibe cambios desde `develop` luego de haber sido revisados y verificados.

* **Hotfix Branch**: En esta rama se realizan correcciones urgentes de errores críticos detectados en producción (`main`). Su objetivo es mantener la estabilidad del proyecto.

* **Bugfix Branch**: En esta rama se corrigen errores antes del despliegue. Se crean desde `develop` y los cambios regresan a la misma rama al finalizar la corrección.

### Release Versioning Conventions

Para la nomenclatura de los lanzamientos se utiliza **Semantic Versioning** con la siguiente estructura:

* **Número principal:** Incrementa cuando se realiza un cambio mayor al proyecto. Cada sprint finalizado suma uno a este número. Por ejemplo: al finalizar el Sprint 1, la versión será `v1.0.0`; al finalizar el Sprint 2, `v2.0.0`.
* **Número secundario:** Incrementa cuando se agrega una funcionalidad menor o se corrige un error entre sprints. Por ejemplo: `v1.1.0`.
* **Número terciario:** Incrementa cuando se aplica un parche o corrección de bugs visuales o de comportamiento. Por ejemplo: `v1.1.1`.

### Commits Conventions

Para los mensajes de los commits del proyecto en Git, se utiliza **Conventional Commits**, que establece mensajes claros y fáciles de entender por todos los colaboradores. La estructura es la siguiente:

```
<type>(<scope>): <description>
```

Los tipos de commit utilizados son:

* `feat`: Implementación de una nueva funcionalidad.
* `fix`: Corrección de errores.
* `docs`: Cambios en la documentación.
* `style`: Cambios de formato o estilo sin afectar la lógica.
* `refactor`: Reestructuración del código sin cambios funcionales.
* `chore`: Actualizaciones de dependencias o tareas de mantenimiento.
* `test`: Adición o modificación de pruebas.

---

#### 4.1.3. Source Code Style Guide & Conventions

En esta sección, se definen las convenciones y referencias adoptadas para la nomenclatura de elementos de programación en los lenguajes utilizados en la solución ChambaYA. En general, la nomenclatura de archivos y secciones de código se realizará en inglés.

* **Convenciones para HTML:** Para la codificación del Landing Page en HTML, se utiliza como referencia el artículo "HTML Style Guide and Coding Conventions" de W3Schools (https://www.w3schools.com/html/html5_syntax.asp). Las convenciones adoptadas son:
    * Los nombres de elementos y atributos deben escribirse en **minúsculas**.
    * Las etiquetas deben siempre cerrarse correctamente.
    * Los valores de los atributos deben ir entre comillas.
    * Utilizar metadatos esenciales como `charset` y `name=viewport` para diseño responsivo.
    * Los nombres de archivos deben estar en minúsculas.

* **Nomenclatura en CSS:** Para los estilos del Landing Page, se utiliza como referencia el artículo "Google HTML/CSS Style Guide" (https://google.github.io/styleguide/htmlcssguide.html). Las convenciones adoptadas son:
    * Todos los estilos deben estar en un archivo CSS separado, por ejemplo `styles.css`.
    * Usar clases en lugar de IDs para aplicar estilos CSS.
    * Los nombres de clases deben ser descriptivos, en minúsculas y con guiones. Por ejemplo: `nav-bar`, `job-card`.

* **Nomenclatura en JavaScript:** Para la codificación en JavaScript del Landing Page, se utiliza como referencia el artículo "Google JavaScript Style Guide" (https://google.github.io/styleguide/jsguide.html). Las convenciones adoptadas son:
    * Evitar el uso de `var`; preferir `let` y `const` según el caso.
    * Usar la convención K&R para llaves: la llave de apertura va en la misma línea que la declaración.
    * Cada línea de código debe limitarse a 80 caracteres.

* **Nomenclatura para Kotlin:** Para el desarrollo de la aplicación móvil Android nativa, se usa Kotlin como lenguaje principal. La guía de referencia es la guía oficial de convenciones de Kotlin (https://kotlinlang.org/docs/coding-conventions.html). Las convenciones adoptadas son:
    * Los nombres de paquetes deben estar siempre en minúsculas y sin guiones bajos. Por ejemplo: `com.chambaya.app`.
    * Los nombres de clases deben usar UpperCamelCase. Por ejemplo: `JobPostingViewModel`.
    * Las funciones, propiedades y variables locales deben comenzar con letra minúscula y usar camelCase. Por ejemplo: `fetchNearbyJobs`.
    * Preferir `val` sobre `var` cuando la variable no cambiará después de inicializarse.

* **Nomenclatura en Java / Spring Boot:** Para el desarrollo del backend, se usa Java con Spring Boot siguiendo las convenciones estándar de Java (https://www.oracle.com/java/technologies/javase/codeconventions-introduction.html). Las convenciones adoptadas son:
    * Las clases deben usar UpperCamelCase. Por ejemplo: `JobPostingService`, `UserRepository`.
    * Los métodos y variables locales deben usar camelCase. Por ejemplo: `findNearbyJobs()`, `jobTitle`.
    * Las interfaces deben nombrarse con UpperCamelCase y pueden comenzar con `I`. Por ejemplo: `IJobRepository`.
    * Los paquetes deben estar en minúsculas. Por ejemplo: `com.chambaya.backend.jobs`.
    * Las constantes deben usar UPPER_SNAKE_CASE. Por ejemplo: `MAX_DISTANCE_KM`.

* **Nomenclatura para RESTful API:** Para los endpoints del backend de ChambaYA, se usa como referencia el artículo "REST API URI Naming Conventions and Best Practices" (https://restfulapi.net/resource-naming/). Las convenciones adoptadas son:
    * Las URIs deben usar sustantivos que representen recursos. Por ejemplo: `api/jobs`, `api/users`.
    * Las acciones se indican mediante verbos HTTP (GET, POST, PUT, DELETE), no en la URI.
    * Las URIs deben estar en minúsculas y usar guiones (`-`) para separar palabras.
    * No agregar barra `/` al final de la URI.
    * Usar parámetros de consulta para filtrar o paginar. Por ejemplo: `api/jobs?location=miraflores&limit=10`.

* **Convenciones para MongoDB:** Para la base de datos no relacional del proyecto, se utiliza como referencia la documentación oficial de MongoDB (https://www.mongodb.com/docs/manual/reference/limits/#naming-restrictions). Las convenciones adoptadas son:
    * Los nombres de colecciones no deben comenzar con el prefijo `system`.
    * Cada documento debe tener un campo `_id` único dentro de su colección.
    * Usar camelCase para los nombres de los campos. Por ejemplo: `jobTitle`, `postedAt`, `workerName`.
    * No almacenar documentos con campos duplicados.

#### 4.1.4. Software Deployment Configuration
En esta sección, se especifica la configuración para realizar el despliegue de la solución en el repositorio. Para realizar esto, se usó Github Pages para desplegar el landing page,********* para la aplicación Backend y Base de Datos NoSQL.

### 4.2. Landing Page & Mobile Application Implementation

### Despliegue de la Landing Page

- **Paso 1: Creacion del repositorio**

    Como primer paso, se debe crear el repositorio en GitHub que será el lugar donde se aloja todo lo relacionado al Landing Page.

![chambalandingcreation.png](../assets/img/chapter-4/chambalandingcreation.png)


- **Paso 2: Creación del Proyecto en WebStorm**

  Como segundo paso, se creara el proyecto en WebStorm, importamos nuestros features e instalamos las dependencias necesarias.

![chambaprojectcreation.png](../assets/img/chapter-4/chambaprojectcreation.png)


- **Paso 3: Carga de archivos necesarios**

    Como tercer paso, se importan todos los archivos necesarios para el desarrollo de la landing page como imágenes, archivos HTML, CSS y JavaScript.


![structurechamba.png](../assets/img/chapter-4/structurechamba.png)

- **Paso 4: Preparar el lanzamiento**

  Como cuarto paso, se juntan todas las características del proyecto en una sola para verificar el correcto funcionamiento de cada una. Luego, se envía todo a la rama principal donde se encuentra, por defecto, el proyecto.

![Landing-Pagestructure.png](../assets/img/chapter-4/Landing-Pagestructure.png)

- **Paso 5: Desplegar la Landing Page**

  Como quinto paso, cuando todo se encuentre en la rama principal, se accede a la sección Configuración del repositorio, luego, se selecciona la opción “GitHub Pages” y se seleccionará la rama principal que es la que se desea desplegar.

![deploymentlanding.png](../assets/img/chapter-4/deploymentlanding.png)


- **Paso 6: Acceder al Landing Page**

  Como paso final, el entorno otorgará un enlace para poder acceder al proyecto desplegado.

![landingpagefront.png](../assets/img/chapter-4/landingpagefront.png)


#### 4.2.1. Sprint `1`
##### 4.2.1.1. Sprint Planning `1`
##### 4.2.1.2. Sprint Backlog `1`
##### 4.2.1.3. Development Evidence for Sprint Review
##### 4.2.1.4. Testing Suite Evidence for Sprint Review
##### 4.2.1.5. Execution Evidence for Sprint Review
##### 4.2.1.6. Services Documentation Evidence for Sprint Review
##### 4.2.1.7. Software Deployment Evidence for Sprint Review
##### 4.2.1.8. Team Collaboration Insights during Sprint

### 4.3. Validation Interviews
#### 4.3.1. Diseño de Entrevistas
#### 4.3.2. Registro de Entrevistas
#### 4.3.3. Evaluaciones según Heurísticas