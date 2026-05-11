#### 4.1.4. Software Deployment Configuration

En esta sección, se especifica la configuración realizada para el despliegue de los productos de software de ChambaYA. Se utilizó **GitHub Pages** para el Landing Page, **Railway** para el Backend API y **MongoDB Atlas** para la base de datos NoSQL.

---

### Despliegue de la Landing Page

- **Paso 1: Creación del repositorio**

  Como primer paso, se creó el repositorio en GitHub que aloja todo lo relacionado al Landing Page.

  ![chambalandingcreation.png](../assets/img/chapter-4/chambalandingcreation.png)

- **Paso 2: Creación del proyecto en WebStorm**

  Como segundo paso, se creó el proyecto en WebStorm, se importaron los features y se instalaron las dependencias necesarias.

  ![chambaprojectcreation.png](../assets/img/chapter-4/chambaprojectcreation.png)

- **Paso 3: Carga de archivos necesarios**

  Como tercer paso, se importaron todos los archivos necesarios para el desarrollo del Landing Page, incluyendo imágenes, archivos HTML, CSS y JavaScript.

  ![structurechamba.png](../assets/img/chapter-4/structurechamba.png)

- **Paso 4: Preparar el lanzamiento**

  Como cuarto paso, se unificaron todas las características del proyecto en una sola rama para verificar el correcto funcionamiento. Luego, se envió todo a la rama principal del repositorio.

  ![Landing-Pagestructure.png](../assets/img/chapter-4/Landing-Pagestructure.png)

- **Paso 5: Desplegar la Landing Page**

  Como quinto paso, desde la sección de Configuración del repositorio en GitHub, se seleccionó la opción "GitHub Pages" y se eligió la rama principal como fuente de despliegue.

  ![deploymentlanding.png](../assets/img/chapter-4/deploymentlanding.png)

- **Paso 6: Acceder al Landing Page**

  Como paso final, GitHub Pages generó un enlace público para acceder al proyecto desplegado.

  ![landingpagefront.png](../assets/img/chapter-4/landingpagefront.png)

---

### Despliegue de la Base de Datos NoSQL (MongoDB Atlas)

- **Paso 1: Creación del proyecto en MongoDB Atlas**

  Como primer paso, se accedió a MongoDB Atlas y se creó un nuevo proyecto denominado **ChambaYa**, donde se alojarán los clusters y colecciones de la base de datos.

  ![CreateProjectMongo.jpeg](../assets/img/chapter-4/CreateProjectMongo.jpeg)

- **Paso 2: Despliegue del cluster**

  Como segundo paso, se configuró y desplegó el cluster de base de datos. Se seleccionó el plan **Free** con proveedor **AWS** en la región **N. Virginia (us-east-1)**, nombrando el cluster como `chambaya-Cluster`.

  ![Deploycluster.jpeg](../assets/img/chapter-4/Deploycluster.jpeg)

- **Paso 3: Creación del usuario de acceso**

  Como tercer paso, se creó un usuario de acceso con credenciales para la conexión segura entre el backend y la base de datos en la nube.

  ![UserVerificationCerate.jpeg](../assets/img/chapter-4/UserVerificationCerate.jpeg)

- **Paso 4: Configuración de las credenciales MongoDB**

  Como cuarto paso, se configuraron las credenciales de acceso al cluster, las cuales serán utilizadas como variables de entorno en el backend para la cadena de conexión `MONGODB_URI`.

  ![MpngoDbCredentials.jpeg](../assets/img/chapter-4/MpngoDbCredentials.jpeg)

- **Paso 5: Verificación de datos en Atlas**

  Como paso final, se verificó en el Data Explorer de MongoDB Atlas que los documentos se almacenan correctamente en la colección `users` dentro de la base de datos `chambaya_db`, confirmando la conexión exitosa entre el backend y la base de datos.

  ![AddData.jpeg](../assets/img/chapter-4/AddData.jpeg)

---

### Despliegue del Backend API (Railway)

- **Paso 1: Creación del proyecto en Spring Initializr**

  Como primer paso, se configuró el proyecto backend usando **Spring Initializr** con las siguientes especificaciones: lenguaje **Java 21**, Spring Boot **4.0.6**, empaquetado **JAR**, y las dependencias Spring Web, Spring Data MongoDB, Validation, Lombok, Spring Boot DevTools y Spring Security.

  ![ProjectCreation.jpeg](../assets/img/chapter-4/ProjectCreation.jpeg)

- **Paso 2: Creación del proyecto en Railway**

  Como segundo paso, se accedió a la plataforma **Railway** y se creó un nuevo proyecto donde se desplegará el backend de ChambaYA.

  ![SearchRepo.jpeg](../assets/img/chapter-4/SearchRepo.jpeg)

- **Paso 3: Instalación y autorización de Railway App en GitHub**

  Como tercer paso, se instaló y autorizó la **Railway App** en la organización de GitHub `app-movil-3821`, seleccionando únicamente el repositorio `Backend-ChambaYa` para el acceso controlado.

  ![Install_ans_Auth.jpeg](../assets/img/chapter-4/Install%20ans%20Auth.jpeg)

- **Paso 4: Selección del repositorio**

  Como cuarto paso, se seleccionó el repositorio `app-movil-3821/Backend-ChambaYa` desde Railway para iniciar el proceso de despliegue automático.

  ![SelectRepo.jpeg](../assets/img/chapter-4/SelectRepo.jpeg)

- **Paso 5: Configuración de variables de entorno**

  Como quinto paso, se configuró la variable de entorno `MONGODB_URI` en Railway con la cadena de conexión proporcionada por MongoDB Atlas, permitiendo que el backend se conecte correctamente a la base de datos en la nube.

  ![AtlasConnection.jpeg](../assets/img/chapter-4/AtlasConnection.jpeg)

- **Paso 6: Generación del dominio público**

  Como sexto paso, desde la sección de configuración de Networking en Railway, se generó un dominio público para acceder al backend desplegado externamente.

  ![DomainGeneration.jpeg](../assets/img/chapter-4/DomainGeneration.jpeg)

- **Paso 7: Verificación del despliegue**

  Como séptimo paso, se verificó que el backend se encuentra correctamente desplegado y en estado **Online** dentro de Railway, con conexión activa al repositorio en GitHub y despliegue automático configurado desde la rama `main`.

  ![Conect.jpeg](../assets/img/chapter-4/Conect.jpeg)

- **Paso 8: Verificación de los endpoints con Swagger**

  Como paso final, se verificó el correcto funcionamiento de los endpoints del backend accediendo a la documentación **Swagger UI** generada automáticamente. Se confirmó que el endpoint `GET /api/v1/users` retorna correctamente los datos de los usuarios registrados en la base de datos con código de respuesta **200 OK**.

  ![DeployVerification.jpeg](../assets/img/chapter-4/DeployVerification.jpeg)

#### 4.2.1. Sprint `1`

En esta sección se explican los procesos para el desarrollo de la solución de software en el primer sprint. Se incluyen secciones de planeamiento, desarrollo, prueba y despliegue de la aplicación móvil Android nativa, el backend API y el Landing Page.


##### 4.2.1.1. Sprint Planning `1`

A continuación, se detalla la información sobre el planeamiento del primer sprint. El objetivo de este sprint se centra en el desarrollo y despliegue de la primera versión del Landing Page de ChambaYA, las primeras pantallas funcionales de la aplicación móvil nativa Android y los endpoints principales del backend API con un avance aproximado del 70%.


| Sprint #                   | Sprint 1                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------| 
| Sprint planning Background | --                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | 
| Date                       | 2026/05/11                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | 
| Time                       | 5:00 pm                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | 
| Location                   | Reunion en meet                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | 
| Prepared By                | Taipe Sangama Jorge Francisco                                                                                                                                                                                                                                                                                                                                                                                                                                                                | 
| Attendes                   | Taipe Sangama Jorge Francisco / Cordova Valdivia Sebastian / 	Janampa Gutierrez Jhoan D.  / Bautista, Jose Diego /  Espinoza Chavez Moises                                                                                                                                                                                                                                                                                                                                                   | 
| Sprint Goal & User Stories |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | 
| Sprint 1 Goal              | Nuestro enfoque está en desarrollar y desplegar el Landing Page de ChambaYA, implementar las pantallas principales de navegación de la aplicación móvil Android y avanzar en un 70% los endpoints del backend API. Creemos que esto entrega una base funcional y visible del producto a los stakeholders. Esto se confirmará cuando el Landing Page esté desplegado, la app muestre navegación entre pantallas clave y el backend responda correctamente a las solicitudes HTTP principales. | 
| Sprint 1 Velocity          | 40                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | 
| Sums of Story Points       | 40                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | 


**Aspect Liders and Colaborators**

En esta sección se incluye la matriz de liderazgo y colaboración para este sprint. La letra "L" indica que el miembro es líder del aspecto y se encarga de avanzar y revisar el trabajo de los colaboradores. La letra "C" indica que el miembro es colaborador y se encarga de desarrollar las funcionalidades asignadas.

| Team Member                    | GitHub Usernames | Landing Page | App Android | Backend API | Reporte |
|--------------------------------|------------------|--------------|-------------|------------|---------|
| Cordova Valdivia Sebastian     | Sevas04          |              | C           | C          | C       |
| Bautista Rivera Jose Diego     | Gogotes17        | L            | C           |            | C       |
| Janampa Gutierrez Jhoan D.     | orraiAKBDFSK     | C            | C           |            | C       |
| Taipe Sangama Jorge Francisco  | CamotinFurious   | L            | L           |            | L       |
| Espinoza Chavez Moises         | MoisesECh        |              |             |            | C       |




##### 4.2.1.2. Sprint Backlog `1`

El objetivo principal de este sprint es tener una versión funcional y desplegada del Landing Page, la navegación principal de la aplicación móvil Android con las pantallas core implementadas, y los endpoints principales del backend funcionando y documentados en Swagger.


Proyecto en Enlace al tablero de Trello: [Link de TRELLO](https://trello.com/invite/b/69e581bada404d81ccde530d/ATTI42a1d93366631bcc58f2fbcf4f6b8734D6B33942/product-backlog-chambaya)

![Trello Sprint1.png](../assets/img/chapter-4/Trello%20Sprint1.png)


A continuación, se presenta la tabla con las User Stories y tareas del Sprint 1:



| Sprint 1     | Sprint Backlog1 |                  |        |                                                                      |                    |              |        |
|--------------|-----------------|------------------|--------|----------------------------------------------------------------------|--------------------|--------------|--------|
| User Stories |                 | Work-Item / Task | Title  | Description                                                          | Estimation (Hours) | Assigned to  | Status |
| US01         |                 | T01              |  | Implementar pantalla de registro de chambeador                       | 4h                 | Jorge Taipe| Done |
| US01         |                 | T02              |  | Implementar endpoint POST /api/v1/users (registro)                   | 3h                 | Sebastián Córdova|  Done|
| US02         |                 | T03              |  | Implementar pantalla de perfil con selección de habilidades (Skills) | 4h                 | Jorge Taipe| Done |
| US03         |                 | T04              |  | Implementar pantalla Home Feed con lista de turnos cercanos          | 4h                 | Jorge Taipe| Done |
| US03         |                 | T05              |  | Implementar endpoint GET /api/v1/jobs (listado de turnos)            | 3h                 |Sebastián Córdova |  Done|
| US04         |                 | T06              |  | Implementar pantalla Job Details y botón de aceptar turno            | 4h                 |Sebastián Córdova |  Done|
| US04         |                 | T07              |  | Implementar pantalla Active Shift (turno en progreso)                | 3h                 | Sebastián Córdova|  Done|
| US05         |                 | T08              |  | Implementar pantalla Apply y confirmación de postulación             | 4h                 | Jhoan Janampa| Done |
| US05         |                 | T09              |  | Implementar endpoint POST /api/v1/enrollments                        | 3h                 | Sebastián Córdova|  Done|
| US11         |                 | T010             |  | Implementar pantalla Chat interno entre usuarios                     | 4h                 | Jhoan Janampa| Done |
| US12         |                 | T011             |  | Implementar pantalla Shift Summary con calificación del turno        | 4h                 | Jhoan Janampa| Done |
| US12         |                 | T012             |  | Implementar endpoint POST /api/v1/reviews                            | 3h                 | Sebastián Córdova| Done |
| US16         |                 | T013             |  | Implementar pantalla My Shifts (lista de turnos del usuario)         | 4h                 |Jose Diego Bautista | Done |
| US18         |                 | T014             |  | Implementar pantalla de detalle de trabajo con mapa y descripción    | 3h                 | Jose Diego Bautista|  Done|
| US29         |                 | T015             |  | Implementar endpoint GET /api/v1/users (listado de usuarios)         | 2h                 | Sebastián Córdova| Done |
| TP01         |                 | T016             |  | Desarrollar y desplegar Landing Page completo en GitHub Pages        | 6h                 |Jorge Taipe |Done  |
| TP01         |                 | T017             |  | Implementar pantalla de inicio (Start/Splash) y Login                | 3h                 |Jorge Taipe | Done |
| TP02         |                 | T018             |  | Documentar sección 4.3 Validation Interviews del reporte             | 4h                 | Moisés Espinoza| Done |


##### 4.2.1.3. Development Evidence for Sprint Review

En esta sección, se describen los principales avances de implementación realizados en este primer sprint. Se tienen como principales avances la implementación del Backend, el desarrollo de la aplicación nativa para Android, y la creación del Landing Page.

Cada miembro del equipo avanzó progresivamente en las diferentes áreas del proyecto: en el Backend se implementaron los endpoints principales y la lógica de negocio usando C# y ASP.NET Core; en la aplicación Android se desarrollaron las pantallas principales y la navegación entre secciones usando Kotlin y Jetpack Compose; y en el Landing Page se implementaron todas las secciones informativas respecto a los mockups en Figma.

A continuación, se muestra una tabla que contiene la información sobre los commits realizados que contienen las funcionalidades implementadas para completar el primer sprint.

|  Repository         | Branch | Commit Id | Commit Message                                                | Committed On |
|---------------------|--------|-----------|---------------------------------------------------------------|---|
| Backend-ChambaYa    | main   | -         | chore: initialize Spring Boot backend project                 | 2026/05/06 |
| Backend-ChambaYa    | main   | -         | feat(iam): add user registration and authentication endpoints | 2026/05/07 |
| Backend-ChambaYa    | main   | -         | feat(jobs): add job posting and listing endpoints             | 2026/05/07 |
| Backend-ChambaYa    | main   | -         | feat(enrollments): add enrollment management endpoints        | 2026/05/08 |
| Backend-ChambaYa    | main   | -         | feat(reviews): add reviews endpoints                          | 2026/05/08 |
| ChambaPe-kotlin     | main   | -         | feat(auth): add login and register screens                    | 2026/05/07 |
| ChambaPe-kotlin     | main   | -         | feat(home): add home feed and job listing screens             | 2026/05/08 |
| ChambaPe-kotlin     | main   | -         | feat(profile): add skills and profile view screens            | 2026/05/08 |
| ChambaPe-kotlin     | main   | -         | feat(shifts): add active shift and shift summary screens      | 2026/05/09 |
| ChambaPe-kotlin     | main   | -         | feat(chat): add chat screen                                   | 2026/05/09 |
| LandingPageChambaYa | main   | -         | feat: add complete landing page sections                      | 2026/05/10 |


##### 4.2.1.4. Testing Suite Evidence for Sprint Review

En esta sección se presenta el conjunto de pruebas implementadas para los Web Services relacionados con las User Stories del Sprint 1. Se utilizó **JUnit 5** con la anotación `@SpringBootTest` para las pruebas de integración del backend, verificando el comportamiento de los endpoints implementados.

Para los Acceptance Tests bajo el enfoque BDD, se elaboraron archivos `.feature` usando el lenguaje **Gherkin**, relacionados directamente con las User Stories implementadas en este sprint.

Repositorio de Testing: [Backend-ChambaYa](https://github.com/app-movil-3821/Backend-ChambaYa)

| Repository | Branch | Commit Id | Commit Message | Committed On |
|---|---|---|---|---|
| Backend-ChambaYa | main | - | test(iam): add unit tests for user registration | 2026/05/08 |
| Backend-ChambaYa | main | - | test(jobs): add acceptance tests for job listing | 2026/05/09 |
| Backend-ChambaYa | main | - | test(enrollments): add BDD feature files for enrollment | 2026/05/09 |
##### 4.2.1.5. Execution Evidence for Sprint Review

En esta sección se presenta la evidencia de ejecución de los productos implementados en este sprint. Los logros incluyen el desarrollo y despliegue del Landing Page, las pantallas principales de la aplicación Android y los endpoints del backend API desplegado en Railway.

A continuación, se muestran las capturas de pantalla y enlaces de acceso a cada producto implementado. Estas evidencias reflejan el progreso realizado en el sprint y sirven como comprobante del trabajo completado.

### Landing Page

---

Se adjuntan los enlaces para acceder al sitio web estático desplegado y al vídeo de demostración. El vídeo muestra el funcionamiento de cada sección del sitio web y su visualización en navegador web.

Sitio web estático desplegado: https://app-movil-3821.github.io/LandingPageChambaYa/
Vídeo de ejecución: StockSip Landing Page - Sprint 1


Home:

![homelanding.png](../assets/img/chapter-4/LandingPageUIDesign/homelanding.png)

Services:

![serviceslanding.png](../assets/img/chapter-4/LandingPageUIDesign/serviceslanding.png)

How it Works:

![howitworkslanding.png](../assets/img/chapter-4/LandingPageUIDesign/howitworkslanding.png)

Pricing:

![pricinglanding.png](../assets/img/chapter-4/LandingPageUIDesign/pricinglanding.png)

About us:

![aboutuslanding.png](../assets/img/chapter-4/LandingPageUIDesign/aboutuslanding.png)

Contact us:

![contactlanding.png](../assets/img/chapter-4/LandingPageUIDesign/contactlanding.png)

Footer:

![footerlanding.png](../assets/img/chapter-4/LandingPageUIDesign/footerlanding.png)


### Aplicación Android

---

Se adjuntan los enlaces para acceder a la aplicación móvil nativa desplegada y al vídeo de demostración. El vídeo muestra el funcionamiento de cada sección de la aplicación y su visualización en un dispositivo Android.

![Active Shift.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/Active%20Shift.png)
![Apply.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/Apply.png)
![Home Feed.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/Home%20Feed.png)
![Chat.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/Chat.png)
![Job Details.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/Job%20Details.png)
![login.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/login.png)
![My Shift.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/My%20Shift.png)
![Profile View.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/Profile%20View.png)
![Register.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/Register.png)
![Shift Summary.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/Shift%20Summary.png)
![Skills.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/Skills.png)
![Start.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/Start.png)

### Backend Application

Se adjuntan los enlaces para acceder a la API desplegada y al vídeo de demostración. El vídeo muestra el funcionamiento de los endpoints implementados y cómo interactúan con la aplicación móvil y la base de datos.

Aplicación Backend desplegada: https://backend-chambaya-production.up.railway.app/swagger-ui/index.html#/
Vídeo de ejecución de la Aplicación Backend: StockSip Backend - Sprint 1: 


User Controller:

![usercontrollerapi.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/usercontrollerapi.png)
Job Controller:
![jobcontroller.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/jobcontroller.png)
Enrollment Controller:
![enrollmentscontroller.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/enrollmentscontroller.png)
Reviews Controller:
![reviewcontroller.png](../assets/img/chapter-4/MobileApplicationsUXUIDesign/cap4documentation/reviewcontroller.png)


##### 4.2.1.6. Services Documentation Evidence for Sprint Review


##### 4.2.1.7. Software Deployment Evidence for Sprint Review


### Despliegue de la Landing Page

- **Paso 1: Creación del repositorio**

  Como primer paso, se creó el repositorio en GitHub que aloja todo lo relacionado al Landing Page.

  ![chambalandingcreation.png](../assets/img/chapter-4/chambalandingcreation.png)

- **Paso 2: Creación del proyecto en WebStorm**

  Como segundo paso, se creó el proyecto en WebStorm, se importaron los features y se instalaron las dependencias necesarias.

  ![chambaprojectcreation.png](../assets/img/chapter-4/chambaprojectcreation.png)

- **Paso 3: Carga de archivos necesarios**

  Como tercer paso, se importaron todos los archivos necesarios para el desarrollo del Landing Page, incluyendo imágenes, archivos HTML, CSS y JavaScript.

  ![structurechamba.png](../assets/img/chapter-4/structurechamba.png)

- **Paso 4: Preparar el lanzamiento**

  Como cuarto paso, se unificaron todas las características del proyecto en una sola rama para verificar el correcto funcionamiento. Luego, se envió todo a la rama principal del repositorio.

  ![Landing-Pagestructure.png](../assets/img/chapter-4/Landing-Pagestructure.png)

- **Paso 5: Desplegar la Landing Page**

  Como quinto paso, desde la sección de Configuración del repositorio en GitHub, se seleccionó la opción "GitHub Pages" y se eligió la rama principal como fuente de despliegue.

  ![deploymentlanding.png](../assets/img/chapter-4/deploymentlanding.png)

- **Paso 6: Acceder al Landing Page**

  Como paso final, GitHub Pages generó un enlace público para acceder al proyecto desplegado.

  ![landingpagefront.png](../assets/img/chapter-4/landingpagefront.png)

---

### Despliegue de la Base de Datos NoSQL (MongoDB Atlas)

- **Paso 1: Creación del proyecto en MongoDB Atlas**

  Como primer paso, se accedió a MongoDB Atlas y se creó un nuevo proyecto denominado **ChambaYa**, donde se alojarán los clusters y colecciones de la base de datos.

  ![CreateProjectMongo.jpeg](../assets/img/chapter-4/CreateProjectMongo.jpeg)

- **Paso 2: Despliegue del cluster**

  Como segundo paso, se configuró y desplegó el cluster de base de datos. Se seleccionó el plan **Free** con proveedor **AWS** en la región **N. Virginia (us-east-1)**, nombrando el cluster como `chambaya-Cluster`.

  ![Deploycluster.jpeg](../assets/img/chapter-4/Deploycluster.jpeg)

- **Paso 3: Creación del usuario de acceso**

  Como tercer paso, se creó un usuario de acceso con credenciales para la conexión segura entre el backend y la base de datos en la nube.

  ![UserVerificationCerate.jpeg](../assets/img/chapter-4/UserVerificationCerate.jpeg)

- **Paso 4: Configuración de las credenciales MongoDB**

  Como cuarto paso, se configuraron las credenciales de acceso al cluster, las cuales serán utilizadas como variables de entorno en el backend para la cadena de conexión `MONGODB_URI`.

  ![MpngoDbCredentials.jpeg](../assets/img/chapter-4/MpngoDbCredentials.jpeg)

- **Paso 5: Verificación de datos en Atlas**

  Como paso final, se verificó en el Data Explorer de MongoDB Atlas que los documentos se almacenan correctamente en la colección `users` dentro de la base de datos `chambaya_db`, confirmando la conexión exitosa entre el backend y la base de datos.

  ![AddData.jpeg](../assets/img/chapter-4/AddData.jpeg)

---

### Despliegue del Backend API (Railway)

- **Paso 1: Creación del proyecto en Spring Initializr**

  Como primer paso, se configuró el proyecto backend usando **Spring Initializr** con las siguientes especificaciones: lenguaje **Java 21**, Spring Boot **4.0.6**, empaquetado **JAR**, y las dependencias Spring Web, Spring Data MongoDB, Validation, Lombok, Spring Boot DevTools y Spring Security.

  ![ProjectCreation.jpeg](../assets/img/chapter-4/ProjectCreation.jpeg)

- **Paso 2: Creación del proyecto en Railway**

  Como segundo paso, se accedió a la plataforma **Railway** y se creó un nuevo proyecto donde se desplegará el backend de ChambaYA.

  ![SearchRepo.jpeg](../assets/img/chapter-4/SearchRepo.jpeg)

- **Paso 3: Instalación y autorización de Railway App en GitHub**

  Como tercer paso, se instaló y autorizó la **Railway App** en la organización de GitHub `app-movil-3821`, seleccionando únicamente el repositorio `Backend-ChambaYa` para el acceso controlado.

  ![Install_ans_Auth.jpeg](../assets/img/chapter-4/Install%20ans%20Auth.jpeg)

- **Paso 4: Selección del repositorio**

  Como cuarto paso, se seleccionó el repositorio `app-movil-3821/Backend-ChambaYa` desde Railway para iniciar el proceso de despliegue automático.

  ![SelectRepo.jpeg](../assets/img/chapter-4/SelectRepo.jpeg)

- **Paso 5: Configuración de variables de entorno**

  Como quinto paso, se configuró la variable de entorno `MONGODB_URI` en Railway con la cadena de conexión proporcionada por MongoDB Atlas, permitiendo que el backend se conecte correctamente a la base de datos en la nube.

  ![AtlasConnection.jpeg](../assets/img/chapter-4/AtlasConnection.jpeg)

- **Paso 6: Generación del dominio público**

  Como sexto paso, desde la sección de configuración de Networking en Railway, se generó un dominio público para acceder al backend desplegado externamente.

  ![DomainGeneration.jpeg](../assets/img/chapter-4/DomainGeneration.jpeg)

- **Paso 7: Verificación del despliegue**

  Como séptimo paso, se verificó que el backend se encuentra correctamente desplegado y en estado **Online** dentro de Railway, con conexión activa al repositorio en GitHub y despliegue automático configurado desde la rama `main`.

  ![Conect.jpeg](../assets/img/chapter-4/Conect.jpeg)

- **Paso 8: Verificación de los endpoints con Swagger**

  Como paso final, se verificó el correcto funcionamiento de los endpoints del backend accediendo a la documentación **Swagger UI** generada automáticamente. Se confirmó que el endpoint `GET /api/v1/users` retorna correctamente los datos de los usuarios registrados en la base de datos con código de respuesta **200 OK**.

  ![DeployVerification.jpeg](../assets/img/chapter-4/DeployVerification.jpeg)



##### 4.2.1.8. Team Collaboration Insights during Sprint 1

En esta sección se detalla cómo se llevaron a cabo las actividades de implementación durante el primer sprint, así como la participación de cada miembro del equipo. Para este sprint, el equipo se organizó en torno a los tres principales productos: Landing Page, Aplicación Móvil Android Nativa y Backend API. Cada integrante asumió responsabilidades específicas en uno o más de estos componentes, trabajando mediante ramas individuales y siguiendo la estrategia GitFlow para la integración del código.

El proyecto se gestionó utilizando una organización en GitHub llamada **app-movil-3821**, donde se crearon repositorios separados para cada producto. Esto permitió una mejor gestión del código y facilitó la colaboración entre los miembros del equipo.

---

### Landing Page

- El integrante **Jorge Taipe** desarrolló e integró todas las secciones del Landing Page de ChambaYA, incluyendo Home, Services, How it Works, Pricing, About Us, Contact Us y Footer. Además, se encargó del despliegue del sitio web estático en GitHub Pages.

A continuación, se adjunta el gráfico con la cantidad de commits realizados por cada integrante durante este sprint para el desarrollo del Landing Page. Cada barra indica la cantidad de commits realizados, reflejando el progreso del equipo en el desarrollo de las diferentes secciones del sitio web.

![landing-commits.png](../assets/img/chapter-4/TeamCollaboration/landing-commits.png)

También, se adjunta el gráfico del avance realizado por cada rama de funcionalidades en el Landing Page. En este gráfico se puede observar el flujo de desarrollo del sitio web estático, donde cada rama representa una sección específica implementada durante el sprint.

![landing-network.png](../assets/img/chapter-4/TeamCollaboration/landing-network.png)

---

### Backend API

- El integrante **Sebastián Córdova** lideró el desarrollo del backend, implementando los endpoints principales de la aplicación usando Java con Spring Boot y MongoDB. Desarrolló los controllers de usuarios (IAM Context), trabajos (Job Context), postulaciones (Enrollment) y reseñas (Reviews). Además, se encargó del despliegue del backend en **Railway** y la configuración de la base de datos en **MongoDB Atlas**.

A continuación, se muestra el gráfico que detalla la cantidad de commits realizados por cada miembro durante este sprint para el backend. El gráfico refleja el aporte de cada integrante en el avance de la primera versión del Backend API.

![backend-commits.png](../assets/img/chapter-4/TeamCollaboration/backend-commits.png)

También, se adjunta el gráfico del avance por ramas en el repositorio del backend, donde cada rama representa una funcionalidad específica implementada durante el sprint, incluyendo los bounded contexts de IAM, Jobs, Enrollments y Reviews.

![backend-network.png](../assets/img/chapter-4/TeamCollaboration/backend-network.png)

---

### Aplicación Móvil Android

- El integrante **Jorge Taipe** desarrolló las pantallas de Start (Splash), Login, Register, Skills y Home Feed, estableciendo la navegación principal de la aplicación.
- El integrante **Sebastián Córdova** desarrolló las pantallas de Job Details y Active Shift, relacionadas con la visualización y gestión de turnos activos.
- El integrante **Jhoan Janampa** desarrolló las pantallas de Apply, Shift Summary, My Shifts y Chat, cubriendo el flujo de postulación y comunicación entre usuarios.
- El integrante **Jose Diego Bautista** desarrolló las pantallas de detalle de trabajo con mapa y la vista de lista de turnos del usuario.
- El integrante **Moisés Espinoza** colaboró en la documentación del reporte, específicamente en la sección 4.3 de Validation Interviews.

A continuación, se muestra el gráfico que detalla la cantidad de commits realizados por cada miembro durante este sprint para la aplicación móvil Android. El gráfico refleja el aporte de cada integrante en el avance de la primera versión de la aplicación.

![android-commits.png](../assets/img/chapter-4/TeamCollaboration/android-commits.png)

También, se adjunta el gráfico del avance por ramas en el repositorio de la aplicación Android, donde cada rama representa las pantallas y funcionalidades implementadas durante el sprint.

![android-network.png](../assets/img/chapter-4/TeamCollaboration/android-network.png)

---

### Reflexión del equipo

Finalmente, el equipo realizó una reflexión sobre el primer sprint, destacando la buena coordinación y comunicación constante entre los miembros, lo que permitió el desarrollo simultáneo y eficiente de los tres componentes principales: el Backend API, la aplicación móvil nativa para Android y el Landing Page.

Se identificaron áreas de mejora en la planificación de la integración entre la aplicación móvil y el backend, así como la necesidad de realizar pruebas más exhaustivas de los endpoints antes de cada entrega. El equipo valoró positivamente el uso de herramientas como **GitHub** para el control de versiones, **Railway** para el despliegue del backend, **MongoDB Atlas** para la base de datos y **GitHub Pages** para el Landing Page, lo que facilitó la colaboración y el seguimiento del progreso del proyecto.

El equipo considera este avance como fundamental para la continuidad del proyecto, destacando la importancia de haber implementado exitosamente las pantallas principales de navegación de la app, los endpoints core del backend y el Landing Page completo. Se reconoce que aún quedan funcionalidades por implementar, pero se tiene confianza en que el proyecto ha sentado bases sólidas al cumplir con los objetivos establecidos para este sprint, demostrando capacidad efectiva de trabajo en equipo y gestión de diversas tecnologías.

### 4.3. Validation Interviews
#### 4.3.1. Diseño de Entrevistas

En esta sección se definen los elementos y procesos que serán evaluados por los usuarios de ambos segmentos objetivos (Jóvenes y Contratantes) durante las sesiones de validación. El objetivo es medir la claridad de la propuesta de valor y la usabilidad del prototipo.

Elementos a incluir en la validación

- Landing Page: Se presentará para validar si el mensaje de "solución de urgencias laborales" y el modelo "sin CV" se entiende correctamente en los primeros segundos.

- Aplicación Móvil (Prototipo ChambaYA): Se evaluará el prototipo de alta fidelidad, permitiendo al usuario interactuar con las interfaces diseñadas para ambos roles (Trabajador y Contratante).

Flujos a validar:

- User Flow 1: Registro e Inicio de Sesión <br>
Validación de la creación de cuenta, verificación telefónica y, especialmente, la personalización del perfil basada en habilidades (tags) en lugar de carga de archivos.

- User Flow 2: Publicación de Trabajos: <br>
Uso del mapa con geolocalización, búsqueda de vacantes y proceso de postulación rápida.

- User Flow 3: Comunicación (chat) <br>
Interacción en tiempo real entre ambos segmentos para coordinar detalles del turno una vez aceptada la aplicación.

- User Flow 4: Gestión de Perfil <br>
Visualización y edición de información personal, habilidades y experiencia acumulada dentro de la app.

- User Flow 5: Gestión de Turnos <br>
Control de turnos activos, historial de trabajos pasados y visualización de compromisos futuros.

- User Flow 6: Notificaciones y Soporte <br>
Recepción de alertas críticas (nuevas vacantes o aplicaciones) y acceso al centro de ayuda para resolución de problemas o contacto con soporte.


#### 4.3.2. Registro de Entrevistas

En esta sección se muestran los registros de las entrevistas de validación. Cada una de ellas contiene informacion correspondiente a los elementos incluidos, como información acerca del entrevistador, entrevistado, duración y resumen.

<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2">Entrevista #1<br></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Jeremy</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Parra </td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>23</td>
  </tr>
 
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="../assets/img/chapter-4/entrevista1.png" alt="Entrevista1"></td>
  </tr>
  <tr>
    <td>Link</td>
    <td>
      <a href="https://upcedupe-my.sharepoint.com/:v:/g/personal/u202221383_upc_edu_pe/IQDksrENwL3wTLRQoxOlBtDFAYArj3d1noK5p6hLne6LxSo?e=Smw6ML&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifSwicGxheWJhY2tPcHRpb25zIjp7fX0%3D" target="_blank">
    Videos entrevistas
  </a>
</td>
  </tr>
    <td>Timing donde inicia la entrevista<br></td>
    <td>00:00 min</td>
  </tr>
  <tr>
    <td>Duración de la entrevista<br></td>
    <td>11:11 min</td>
  <tr>
    <td>Resumen</td>
    <td> La entrevista se realizó a Jeremy Parra (23 años), para validar y dar a conocer los flujos de nuestra propuesta, flujos como el registro, el de la aplicacion al trabajo, chat, gestión de turnos y notificaciones. El entrevistado mencionó que la información mostrada en el flujo de la aplicacion a un trabajo es suficiente para elegir postular, destacó la funcionalidad de la ubicación, que era útil para dirigirnos al lugar y ubcarnos de manera rápida. También destacó el apartado de chat, ya que la comunicación era directa con el empleador. También mencionó, que es muy necesario que la aplicación te notifique acerca de turnos nuevos cercanos a tu ubicación. Asimismo, destacó el apartado de turnos, que era información importante que se debería mostrar para que se lleve un registro o control de los trabajos completados.
</td>
  </tr>
</tbody>
</table>


<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2">Entrevista #2<br></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Eirthon</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Reyes</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>25</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="../assets/img/chapter-4/entrevista2.png" alt="Entrevista2"></td>
  </tr>
  <tr>
    <td>Link</td>
    <td>
      <a href="https://upcedupe-my.sharepoint.com/:v:/g/personal/u202221383_upc_edu_pe/IQDksrENwL3wTLRQoxOlBtDFAYArj3d1noK5p6hLne6LxSo?e=NwmZUg&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifSwicGxheWJhY2tPcHRpb25zIjp7InN0YXJ0VGltZUluU2Vjb25kcyI6NjcyLjc3fX0%3D" target="_blank">
    Videos entrevistas
     </a>
    </td>
  </tr>
    <td>Timing donde inicia la entrevista<br></td>
    <td>11:12 min</td>
  </tr>
  <tr>
    <td>Duración de la entrevista<br></td>
    <td>08:26 min</td>
  <tr>
    <td>Resumen</td>
    <td> Se realizó la entrevista de validacion a Eirthon Reyes (25 años), con el objetivo de presentar y validar los flujos de gestion de turnos, perfil de trabajador, chat y notificaciones. Mencionó que al ingresar al apartado de gestión de turnos se sintió un poco abrumado por la cantidad de elementos que aparecen. lo que le dificultaba una lectura rápida, por lo que sería útil ajustar el contenido para mejorar la visualización. Destacó que le generaba confianza el perfil del trabajador sin necesidad de cv, ya que ha tenido que estar registrado para poder postular y trabajar en la app, además de la visualización de sus habilidades.También notó que no existe una flecha de retroceso ni una opción clara para "ir hacia atrás" en el apartado de mis turnos, por lo que sería recomendable una flecha de retorno visible en la esquina, que permita regresar a la pantalla anterior de forma intuitiva. Asimismo, identificó que los iconos de Home, Chat y Perfil eran intuitivos, pero que el icono de "Shifts" (Turnos) en la barra inferior no se entendía tan bien por sí solo, ya que intentaba abarcar demasiadas funciones, lo que genera incertidumbre sobre qué se encontrará al hacer clic, a lo que recomendó separar las funciones en iconos más específicos para evitar la ambigüedad.
</td>
  </tr>
</tbody>
</table>


<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2">Entrevista #3<br></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td></td>
    <td> </td>
  </tr>
  <tr>
    <td>Edad</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="../assets/img/chapter-2/entrevista3.png" alt="Entrevista3"></td>
  </tr>
  <tr>
    <td>Link</td>
  
  </tr>
    <td>Timing donde inicia la entrevista<br></td>
    <td> </td>
  </tr>
  <tr>
    <td>Duración de la entrevista<br></td>
    <td> </td>
  <tr>
    <td>Resumen</td>
    <td> 
</td>
  </tr>
</tbody>
</table>

#### 4.3.3. Evaluaciones según Heurísticas


**SITE o APP A EVALUAR:**
ChambaYa

El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas:
Registro de usuario nuevo basado en etiquetas de habilidades.

Personalización del perfil (descripción y experiencia).

1. Búsqueda de ofertas de trabajo mediante mapa con geolocalización.
2. Postulación a un turno laboral de emergencia.
3. Publicación de una vacante urgente (flujo del contratante).
4. Uso del chat interno para coordinación.
5. Visualización y gestión de turnos activos/pasados.
6. Envío de reporte de problemas en la sección de ayuda.

No están incluidas en esta versión de la evaluación las siguientes tareas:
1. Pasarela de pagos y facturación electrónica.
2. Sistema de referidos o bonos por cumplimiento.
3. Verificación de antecedentes penales automatizada.
4. Configuración avanzada de privacidad y datos.



**ESCALA DE SEVERIDAD:**
Los errores serán puntuados tomando en cuenta la siguiente escala de severidad
| Nivel | Descripción |
|-----|-----------|
| 1 | Problema superficial: puede ser fácilmente superador por el usuario ó ocurre con muy poco frecuencia. No necesita ser arreglado a no ser que exista disponibilidad de tiempo. |
| 2 | Problema menor: puede ocurrir un poco más frecuentemente o es un poco más difícil de superar para el usuario. Se le debería asignar una prioridad baja resolverlo de cara al siguiente release |
| 3 | Problema mayor: ocurre frecuentemente o los usuarios no son capaces de resolverlos. Es importante que sean corregidos y se les debe asignar una prioridad alta. |
| 4 | Problema muy grave: un error de gran impacto que impide al usuario continuar con el uso de la herramienta. Es imperativo que sea corregido antes del lanzamiento. |



**TABLA RESUMEN:**
| # | Problema | Escala de severidad | Heurística/Principio violado(a) |
|--|-------|-------------------|-------------------------------|
| 1 | Sobrecarga de información y falta de jerarquía visual  | 2 | Usabilidad - Diseño estético y minimalista. |
| 2 | Ausencia de controles de navegación de retorno (Back button) | 3 | Usabilidad - Libertad y control del usuario |
| 3 | Iconografía ambigua y falta de estándares en la barra de navegación  | 2 | Usabilidad - Consistencia y estándares. |



**DESCRIPCIÓN DE PROBLEMAS:**

PROBLEMA 1: Sobrecarga de información y falta de jerarquía visual

Severidad: 2

Heurística violada: Usabilidad - Diseño estético y minimalista.

Problema: Al interactuar con la pantalla, el usuario manifestó sentirse abrumado por la cantidad de elementos que aparecen de golpe al entrar al apartado. Indicó que la información no está categorizada, lo que dificulta una lectura rápida y genera confusión visual.

Recomendación: Aplicar una mejor arquitectura de información separando el contenido en áreas o secciones claramente diferenciadas. Utilizar el principio de "progresividad" para no mostrar todo el contenido en una sola vista.

---


PROBLEMA 2: Ausencia de controles de navegación de retorno (Back button)

Severidad: 3

Heurística violada: Usabilidad - Libertad y control del usuario.

Problema: En el flujo evaluado, el usuario notó que no existe una flecha de retroceso ni una opción clara para "ir hacia atrás". Esto genera una sensación de encierro en la pantalla actual, obligando al usuario a reiniciar la app o usar botones externos del sistema que podrían romper el flujo.

Recomendación: Incluir una flecha de retorno visible en la esquina superior izquierda (TopAppBar) que permita al usuario regresar a la pantalla anterior de forma intuitiva.

---

PROBLEMA 3: Iconografía ambigua y falta de estándares en la barra de navegación

Severidad: 2

Heurística violada: Usabilidad - Consistencia y estándares.

Problema: El usuario identificó correctamente los iconos de Home, Chat y Perfil, pero reportó que el icono de "Shifts" (Turnos) en la barra inferior es demasiado complejo y no se entiende por sí solo. Mencionó que el icono intenta abarcar demasiadas funciones, lo que genera incertidumbre sobre qué se encontrará al hacer clic.

Recomendación: Rediseñar el icono de "Shifts" utilizando una metáfora visual más simple y estándar (como un calendario o reloj de turno). Alternativamente, separar las funciones en iconos más específicos para evitar la ambigüedad.
