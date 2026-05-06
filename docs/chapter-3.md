## Capítulo III: Solution UI/UX Design

### 3.1. Product Design
#### 3.1.1. Style Guidelines

En esta sección, el equipo establece un repositorio organizado y central de elementos comunes (assets, fonts, colores, iconografía) para mantener una presentación visual consistente y enfocada, alineada con el espíritu de ChambaYa: dinámico, confiable y cercano a la cultura popular peruana.

##### 3.1.1.1. General Style Guidelines

##### Branding
- Identidad visual moderna y profesional que transmite **confiabilidad**, **rapidez** y **energia juvenil**.
- Iconografía clara e intuitiva: íconos simples y reconocibles para acciones principales.
 ##### Typography
 - Tipografías Inter de alta legibilidad optimizadas para dispositivos móviles.
- Sistema de jerarquía tipográfica:
  - **Títulos principales**: Semi Bold, tamaño grande para encabezados de pantalla
  - **Subtítulos**: Medium para secciones y tarjetas
  - **Texto general**: Regular para contenido de lectura
  - **Labels**: Regular para etiquetas de formularios

  ##### Colors
- Paleta de colores basada en tonos azules como color principal:
  - **Primario**: azul (#2563EB aproximadamente) - botones principales, elementos activos
  - **Secundarios**: Verde dinámico(#22C55E aproximadamente) tonos claros de verde para turno disponible, aceptado
  - **Neutros**: Negro suave (#0F172A), Gris oscuro(#334155), Gris claro(#E2E8F0) y Blanco (#FFFFFF)
  - **Accentos**: HEX (#F97316 aproximadamente) para turnos urgentes, alertas, “Se necesita YA”
  - Los colores transmiten **profesionalismo, confianza y rapidez**
 
   ![colors](/assets/img/introduction/colors.png)

##### Spacing
- Sistema de espaciado consistente:
  - Padding interno de tarjetas: 16px - 24px
  - Separación entre elementos: 12px - 16px
  - Márgenes laterales: 16px - 20px
  - Espacios que mantienen sensación de **orden y claridad visual**

##### Communication Tone
- Tono de comunicación:
  - **Claro y directo** en instrucciones
  - **Amigable pero profesional** en mensajes
  - **Conciso** en labels y descripciones
  - Uso de lenguaje **accesible** para usuarios urbanos

##### Dimension Guidelines
- Componentes de UI con dimensiones estándar:
  - **Botones principales**: Altura 48px - 56px (óptimo para touch)
  - **Íconos**: 24px - 32px
  - **Inputs de texto**: Altura 48px - 56px
  - **Tarjetas de información**: Width: full screen con padding lateral
  - **Bottom Navigation Bar**: Altura 56px - 64px

#### 3.1.2. Information Architecture
##### 3.1.2.1. Organization Systems


**Jerárquico (Visual Hierarchy):**

Se prioriza la información crítica para la toma rápida de decisiones. En la pantalla principal (Home), los elementos más destacados son:

- Turnos disponibles cercanos
- Pago por turno
- Distancia
- Estado (Disponible / Urgente)

**Secuencial (Step-by-Step):**
Implementado en:
- Registro de chambeador o contratante
- Creación de perfil basado en habilidades
- Publicación de turnos (MYPEs)
- Confirmación de llegada y finalización

**Por Tópicos:**
La información se agrupa en secciones claras:
- **Home**: Turnos disponibles y recomendaciones
- **Map**: Visualización geolocalizada de trabajos
- **Chat**: Comunicación entre usuario y contratante
- **Profile**: Configuración y reputación del usuario

**Según Audiencia:**
- **Chambeadores**: Acceso a visualización de mapa, turnos y Chat
- **Contratantes**: Acceso a creacion de turnos, búsqueda y Gestionar turnos

##### 3.1.2.2. Labelling Systems

Etiquetas diseñadas para ser claras y autoexplicativas:

**Ejemplos de Etiquetas:**
- "Welcome" / "Create your account" (pantallas de autenticación)
- "Edit Profile" (acciones de edición)
- "Name" / "Email" / "Password" / "National ID" (campos de formulario)

##### 3.1.2.3. SEO Tags and Meta Tags

**Landing Page:**
- **Title:** ""ChambeaYa""
- **Meta Description:** "Conecta con trabajos temporales cerca de ti. Encuentra turnos flexibles o cubre necesidades de personal en minutos."
- **Keywords:** trabajos temporales, empleo por horas, trabajos cerca, MYPEs, empleo juvenil, turnos flexibles, trabajo rápido
- **Author:** Equipo ChambeaYa

**Aplicación Móvil:**
- **Title (Routes):** "ChambeaYa"
- **Meta Description:** "Explora turnos cercanos, postula y trabaja en minutos"

##### 3.1.2.4. Searching Systems

Sistema de búsqueda implementado en:

**Búsqueda por Filtros:**
- Distancia 
- Tipo de trabajo
- Horarios disponibles
- Estado

**Resultados de Búsqueda:**
Mostrados en tarjetas con información clave:
- Tipo de trabajo
- Pago
- Ubicación y distancia
- Estado

**Navegación por Mapa:**
Visualización de rutas y paradas en mapa interactivo (visible en las pantallas de mapas del Figma)

##### 3.1.2.5. Navigation Systems

Sistema de navegación diseñado para acceso rápido y uso intuitivo.

**Navegacion principal:**
- **Home**
- **Mapa**
- **Turnos**
- **Perfil**

**Navegacion contextual:**
- Desde Home
- Desde Detalle
- Desde turno activo
- Desde notificación

#### 3.1.3. Landing Page UI Design
##### 3.1.3.1. Landing Page Wireframe
Para el desarrollo del Landing Page de ChambaYa, se realizaron diversos bosquejos de baja fidelidad en la aplicación de diseño de interfaz Figma para crear la estructura de las pantallas del Landing Page de la solución.

![Wireframe Landing Page](/assets/img/Chapter-3/LandingPageUIDesign/Wireframe-LandingPage.png)
##### 3.1.3.2. Landing Page Mock-up
Para el desarrollo del Landing Page de ChambaYa, se realizaron bosquejos de alta fidelidad en la aplicación Figma. Para el desarrollo de estas pantallas, se tomó como base los Wireframes previamente diseñados, sin embargo, estas pantallas poseen colores adecuados y la tipografía definida para las distintas secciones del Landing Page.

![Mock-up Landing Page](/assets/img/Chapter-3/LandingPageUIDesign/Mockup-LandingPage.png)

#### 3.1.4. Mobile Applications UX/UI Design
##### 3.1.4.1. Mobile Applications Wireframes
En esta sección se presentarán los wireframes de la aplicación, los cuales son bosquejos de baja fidelidad sobre las funcionalidades principales de nuestra solución. Finalmente, se dividieron estos wireframes en doce secciones.

Sección registro e inicio de sesión

![Wireframe Mobile App - Registro e Inicio de Sesión](/assets/img/Chapter-3/MobileApplicationWireframes/Wireframe-RegistroeIniciodeSesión.png)

Esta imagen presenta el flujo completo de usuario para el sistema ChambaYa, mostrando seis pantallas consecutivas. La primera pantalla muestra un formulario de inicio de sesión con campos para email y contraseña,junto con un botón de "Login" y un enlace para crear una cuenta. La segunda pantalla es el formulario de registro, que incluye campos para nombre completo, email, contraseña y número de teléfono, junto con un botón de "Sing Up". La tercera pantalla es la verificación de número de teléfono. La cuarta pantalla es el Login en caso de que ya se tenga una cuenta, te redirige a Iniciar Sesión. La quinta pantalla es personalizar tu perfil con descripción. Finalmente, la sexta pantalla sigues con la personalización de tus habilidades.

Sección Aplicacion de trabajos

![Wireframe Mobile App - Aplicación de Trabajos](/assets/img/Chapter-3/MobileApplicationWireframes/Wireframe-AplicacionTrabajo.png)

Esta imagen presenta el flujo completo de usuario para el sistema ChambaYa, mostrando cuatro pantallas consecutivas. La primera pantalla muestra la pantalla de inicio con un mapa y una barra de búsqueda en la parte superior también muestra una lista de trabajos disponibles. La segunda pantalla es el detalle del trabajo, que proporciona información más detallada sobre el trabajo seleccionado. La tercera pantalla es la aplicación al trabajo, donde el usuario puede postularse para el trabajo. Finalmente, la cuarta pantalla es la confirmación de aplicación, que muestra un mensaje de éxito después de postularse. 

##### 3.1.4.2. Mobile Applications Wireflow Diagrams
##### 3.1.4.3. Mobile Applications Mock-ups
##### 3.1.4.4. Mobile Applications User Flow Diagrams
##### 3.1.4.5. Mobile Applications Prototyping