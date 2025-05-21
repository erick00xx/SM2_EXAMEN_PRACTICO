# SM2_EXAMEN_PRACTICO - [Nombre de tu Aplicación de Alertas Ciudadanas]

<!-- Reemplaza "[Nombre de tu Aplicación de Alertas Ciudadanas]" con el nombre real o descriptivo de tu app. -->
<!-- Ejemplo: "AlertaVecinal: Seguridad Colaborativa" -->

**URL del Repositorio Público:** `https://github.com/[TU_USUARIO_GITHUB]/SM2_EXAMEN_PRACTICO`
<!-- ¡MUY IMPORTANTE! Reemplaza [TU_USUARIO_GITHUB] con tu nombre de usuario de GitHub. Esta URL es la que necesitas para tu entrega. -->

---

## 📜 Descripción del Proyecto

<!-- Describe brevemente tu aplicación. Menciona el objetivo principal y el contexto general (app móvil de alertas, mapa interactivo, zonas de peligro, etc.). -->
<!-- Ejemplo: -->
[Nombre de tu Aplicación] es una aplicación móvil diseñada para mejorar la seguridad ciudadana en [Nombre de tu Ciudad/Región]. A través de un mapa interactivo, los usuarios pueden registrar y visualizar zonas de peligro reportadas por la comunidad, contribuyendo a una red de alerta colaborativa. La aplicación busca empoderar a los ciudadanos permitiéndoles tomar decisiones informadas sobre sus rutas y estar al tanto de los incidentes en su entorno.

### ✨ Funcionalidades Implementadas (Historias de Usuario Documentadas)

En esta fase del proyecto, se han implementado y documentado las siguientes funcionalidades clave:

1.  **[Título Corto de la Historia de Usuario 1]**: Permite a los usuarios [breve descripción de la capacidad de la historia 1].
2.  **[Título Corto de la Historia de Usuario 2]**: Facilita a los usuarios [breve descripción de la capacidad de la historia 2].

<!-- Estos títulos cortos deben ser descriptivos de la funcionalidad que implementa cada historia. -->

---

## 🚀 Historias de Usuario Implementadas

A continuación, se detalla la implementación de las dos historias de usuario seleccionadas del Product Backlog.

### Historia de Usuario 1: [Nombre Completo de la Historia de Usuario 1]

<!-- Ejemplo de nombre: "Registrar Nueva Zona de Peligro en el Mapa" -->

**ID de Historia:** `HU-00X`
<!-- Asigna un ID único a tu historia si lo tienes en tu backlog -->

**Como** [Rol del Usuario - ej: "ciudadano preocupado"]
**Quiero** [Acción/Funcionalidad - ej: "marcar una ubicación en el mapa como 'zona de peligro' y añadir una descripción y tipo de incidente"]
**Para** [Beneficio/Objetivo - ej: "alertar a otros usuarios de la comunidad sobre un riesgo potencial en esa área específica"]

#### Criterios de Aceptación:

<!-- Lista los criterios que deben cumplirse para considerar esta historia como completada. -->
*   [ ] El usuario puede seleccionar un punto en el mapa interactivo.
*   [ ] Al seleccionar un punto, se abre un formulario para ingresar detalles de la alerta.
*   [ ] El formulario permite seleccionar un tipo de peligro de una lista predefinida (ej: Robo, Accidente, Vandalismo).
*   [ ] El formulario permite añadir una descripción textual del incidente.
*   [ ] Al confirmar, la nueva zona de peligro se guarda y se visualiza en el mapa para otros usuarios.
*   [ ] Se muestra una notificación de éxito al usuario tras registrar la alerta.

#### Descripción Detallada de la Implementación:

<!-- Explica cómo funciona esta característica. Puedes describir el flujo de usuario paso a paso. -->
<!-- Ejemplo: -->
Para registrar una nueva zona de peligro, el usuario primero navega al mapa principal de la aplicación. Al realizar una pulsación larga (o tocar un botón específico de "Añadir Alerta"), se activa el modo de selección de ubicación. El usuario puede entonces tocar el punto exacto en el mapa donde desea reportar el incidente.

Una vez seleccionada la ubicación, aparece un modal o una nueva pantalla con un formulario. Este formulario solicita:
1.  **Tipo de Peligro:** Un desplegable con opciones como "Robo", "Accidente de Tráfico", "Actividad Sospechosa", "Infraestructura Dañada", etc.
2.  **Descripción:** Un campo de texto para que el usuario detalle lo ocurrido o el peligro observado.
3.  **(Opcional) Fecha y Hora:** Pueden tomarse automáticamente o permitir al usuario especificarlas.

Al presionar el botón "Registrar" o "Guardar", la información se envía al backend (o se almacena localmente si es una prueba sin backend) y, si el registro es exitoso, se muestra un marcador distintivo en el mapa en la ubicación seleccionada, visible para todos los usuarios. Además, se presenta un mensaje de confirmación al usuario que registró la alerta.

#### Evidencia Visual (Capturas de Pantalla):

<!-- Añade aquí las capturas de pantalla. Asegúrate de que las imágenes estén en una carpeta (ej. `assets/images/`) dentro de tu repositorio. -->

**Paso 1: Selección de ubicación en el mapa.**
![Descripción de la imagen del paso 1 para la HU1](assets/images/HU1_Paso1_SeleccionMapa.png)
<!-- Reemplaza `HU1_Paso1_SeleccionMapa.png` con el nombre real de tu imagen. Añade una descripción útil en el `alt text`. -->

**Paso 2: Formulario de registro de alerta.**
![Descripción de la imagen del paso 2 para la HU1](assets/images/HU1_Paso2_FormularioAlerta.png)

**Paso 3: Alerta registrada visible en el mapa.**
![Descripción de la imagen del paso 3 para la HU1](assets/images/HU1_Paso3_AlertaEnMapa.png)

<!-- Añade más pasos e imágenes según sea necesario para documentar completamente la historia. -->

---

### Historia de Usuario 2: [Nombre Completo de la Historia de Usuario 2]

<!-- Ejemplo de nombre: "Visualizar Detalles de una Zona de Peligro Existente" -->

**ID de Historia:** `HU-00Y`

**Como** [Rol del Usuario - ej: "usuario de la app"]
**Quiero** [Acción/Funcionalidad - ej: "tocar un marcador de zona de peligro en el mapa"]
**Para** [Beneficio/Objetivo - ej: "ver los detalles de la alerta, como tipo, descripción y fecha del reporte, para estar informado"]

#### Criterios de Aceptación:

*   [ ] El usuario puede ver los marcadores de zonas de peligro en el mapa.
*   [ ] Al tocar un marcador de zona de peligro, se muestra una ventana emergente (o se navega a una pantalla de detalle) con la información de la alerta.
*   [ ] La información mostrada incluye: tipo de peligro, descripción, fecha/hora del reporte, y (opcionalmente) quién lo reportó (de forma anónima o con alias).
*   [ ] El usuario puede cerrar la ventana de detalles para volver al mapa.

#### Descripción Detallada de la Implementación:

<!-- Explica cómo funciona esta característica. Puedes describir el flujo de usuario paso a paso. -->
<!-- Ejemplo: -->
Cuando un usuario abre la aplicación y visualiza el mapa, las zonas de peligro registradas por otros miembros de la comunidad (o por él mismo) aparecen como marcadores distintivos. Si el usuario está interesado en obtener más información sobre una alerta específica, puede simplemente tocar (hacer clic) sobre el marcador correspondiente.

Al tocar el marcador, se despliega una ventana de información (puede ser un "InfoWindow" de Google Maps, un BottomSheet modal, o una pantalla de detalle). Esta ventana muestra:
*   **Icono y Tipo de Peligro:** Un ícono representativo y el texto del tipo de peligro (ej: "Robo").
*   **Descripción:** El texto completo proporcionado por quien reportó la alerta.
*   **Fecha y Hora del Reporte:** Para que el usuario sepa cuán reciente es la información.
*   **(Opcional) Distancia:** Distancia aproximada desde la ubicación actual del usuario hasta la alerta.

El usuario puede interactuar con esta ventana (por ejemplo, hacer scroll si la descripción es larga) y luego cerrarla, usualmente tocando fuera de ella o mediante un botón "X" o "Cerrar", para regresar a la vista completa del mapa y poder explorar otras áreas o alertas.

#### Evidencia Visual (Capturas de Pantalla):

**Paso 1: Mapa con múltiples alertas visibles.**
![Mapa con marcadores de alerta](assets/images/HU2_Paso1_MapaConAlertas.png)
<!-- Reemplaza con tus nombres de archivo y descripciones. -->

**Paso 2: Usuario tocando un marcador específico.**
![Usuario interactuando con un marcador](assets/images/HU2_Paso2_SeleccionMarcador.png)

**Paso 3: Ventana de detalle de la alerta mostrada.**
![Detalle de la alerta visible](assets/images/HU2_Paso3_DetalleAlerta.png)

<!-- Añade más pasos e imágenes según sea necesario. -->

---

## 🛠️ Tecnologías Utilizadas

<!-- Lista las tecnologías, frameworks, librerías y herramientas principales que has usado. -->
*   **Lenguaje de Programación:** [Ej: Dart, Java, Kotlin, Swift, JavaScript]
*   **Framework de Desarrollo Móvil:** [Ej: Flutter, React Native, Android Nativo (Java/Kotlin), iOS Nativo (Swift)]
*   **Mapas:** Google Maps Platform (API de Google Maps para Android/iOS/Flutter)
*   **Base de Datos (si aplica):** [Ej: Firebase Firestore, SQLite, Realm, PostgreSQL]
*   **Autenticación (si aplica, aunque login no se documenta aquí):** [Ej: Firebase Authentication]
*   **Gestión de Estado (si aplica):** [Ej: Provider, BLoC, Redux, ViewModel]
*   **Otras Librerías Clave:**
    *   [Nombre de Librería 1] - [Breve descripción de su uso]
    *   [Nombre de Librería 2] - [Breve descripción de su uso]

---

## 🔗 Enlaces y Referencias

<!-- Si has utilizado recursos externos significativos (APIs de terceros, tutoriales clave, librerías específicas con documentación relevante), menciónalos aquí. -->

*   **Documentación de Google Maps Platform:**
    *   Para Android: [URL a la documentación de Google Maps Android SDK]
    *   Para iOS: [URL a la documentación de Google Maps iOS SDK]
    *   Para Flutter (`google_maps_flutter`): [https://pub.dev/packages/google_maps_flutter](https://pub.dev/packages/google_maps_flutter)
*   **[Nombre de otra API/Librería]:** [URL a su documentación o sitio web]
*   **[Tutorial o Artículo Inspirador]:** [URL si alguno fue fundamental]

---

## 🧑‍💻 Autor

*   **[Tu Nombre Completo]**
*   **Usuario GitHub:** `[TU_USUARIO_GITHUB]`
*   **Correo Electrónico (Opcional):** `[tu_correo@ejemplo.com]`

---

<!-- Nota para ti:
    - Asegúrate de crear la carpeta `assets/images/` en la raíz de tu repositorio y colocar ahí todas tus capturas de pantalla.
    - Reemplaza TODOS los placeholders como `[Texto]` o `[URL]` con tu información real.
    - Verifica que la URL del repositorio en la parte superior sea correcta.
    - Antes de convertir a PDF, visualiza este README en GitHub para asegurarte de que el formato es correcto y las imágenes se cargan.
    - Para convertir a PDF, puedes usar la función de "Imprimir" de tu navegador y seleccionar "Guardar como PDF", o usar herramientas online/extensiones de navegador que convierten Markdown a PDF. Asegúrate de que las imágenes se incluyan en el PDF.
-->