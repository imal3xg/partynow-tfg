# 👑 PartNow - TFG DAM

**Red Social y Gestión de Fiestas** | *Proyecto fin de grado - CPIFP Alan Turing*

---

## 🎥 Video Checkpoint (5 minutos)  
🔗 [Ver en Google Drive](https://drive.google.com/file/d/1WsWjC1H0qFYxM1rsJDdkgAKe8u8m9PDN/view?usp=sharing)  
Resumen del estado actual del proyecto con una demostración práctica. En el video se exponen los principales avances, funcionalidades implementadas y cómo se cumplen los requisitos de prácticamente todas las asignaturas del ciclo.

---

## 📚 Historial de cambios y bibliografía  
📁 [Acceder a Google Drive](https://drive.google.com/file/d/1n59Z1qHDvO0Hrddkcm_o-8w25rjPoBzs/view?usp=drive_link)
Contiene documentación histórica, bibliografía y enlaces complementarios.

---

## 📌 Descripción breve

PartyNow es una aplicación integral, moderna y responsiva, diseñada para descubrir, organizar y gestionar fiestas a nivel mundial. Ofrece una experiencia intuitiva y atractiva, permitiendo a los usuarios explorar eventos, gestionar perfiles y conectar en tiempo real. La app se ha desarrollado utilizando Ionic Framework y Angular, implementando prácticas avanzadas como arquitectura en capas, componentes reutilizables y formularios reactivos, junto con una integración completa con Firebase.

**Funcionalidad Principal**

La funcionalidad de PartyNow se resume en:

- 📲 **Gestión de usuarios y fiestas**: permite registrar, editar y buscar usuarios a nivel de personas o de empresas, y buscar, crear, editar y eliminar fiestas.
- 👤 **Actualización de perfil en tiempo real**: los usuarios verán los cambios que se produzcan en la web y en la app en tiempo real.
- 👥 **Buscador de usuarios**: los usuarios podrán buscar a personas y empresas, y tienen la posibilidad de ver sus fiestas y celebraciones publicadas.
- ☁️ **Sincronización en la nube completa**: disponible en versión web (Ionic Angular) y android (Kotlin Native) con datos unificados mediante Firebase.
- 🧪 **Diseño iterativo**: prototipado inicial en Balsamiq y refinamiento visual y funcional en Figma.

> 🔍 **Toda la documentación técnica y justificación del proyecto está disponible en el [Anteproyecto completo](https://www.notion.so/PartyNow-ANTEPROYECTO-1eb73c3c9fd480298e92e76e79ee7f7d?pvs=4)**

---

## **🎯Objetivos del proyecto**

PartNow busca conectar personas de cualquier parte del mundo para hacer que pasen un rato increíble mediante esta red social, donde los usuarios pueden filtrar las fiestas por país, y ponerse en contacto con el creador de la fiesta para saber más información, ya sean personas o empresas. Para ello, se plantean los siguientes objetivos:

| **Objetivo** | **Beneficio** |
| --- | --- |
| **Simplificar gestión** | Registro simplificado de personas y fiestas |
| **Autologin** | Facilidad de entrar a la web y a la app de Android sin tener que volver a iniciar sesión |
| **Multiplataforma** | Acceso desde cualquier dispositivo |
| **Reconocimiento internacional** | Personas de cualquier país del mundo puede acceder a la app |
| **Disponible en varios idiomas** | Los usuarios pueden elegir entre varios lenguajes para una mejor navegación |

---

## 💻 Tecnologías Utilizadas

### 🌐 Frontend Web  
- **Angular 18** – Framework principal de desarrollo frontend.
- **Ionic Framework 8** – Librería UI para aplicaciones móviles/web con componentes nativos.
- **Capacitor 6** – Plataforma para conectar funcionalidades nativas (como cámara, geolocalización, hápticos).
  - Plugins usados:
    - `@capacitor/camera` – acceso a la cámara.
    - `@capacitor/geolocation` – ubicación GPS.
    - `@capacitor/haptics` – vibración nativa.
    - `@capacitor/keyboard` y `@capacitor/status-bar` – personalización visual.
- **@ngx-translate/core + http-loader** – Soporte de traducción para múltiples idiomas.
- **Firebase (vía SDK JS)** – Autenticación, Firestore, y almacenamiento.
- **Axios** – Cliente HTTP ligero para comunicación con APIs externas.
- **Lottie + ngx-lottie** – Animaciones vectoriales en tiempo real.
- **Ionicons 7** – Conjunto de iconos modernos integrados con Ionic.
- **dotenv** – Gestión de variables de entorno en tiempo de desarrollo.
- **OpenAI SDK** – (opcional) SDK de interacción con modelos de IA si se utiliza.
- **RxJS** – Programación reactiva para flujos de datos.
- **Zone.js** – Integración con el detector de cambios de Angular.


### 📱 Aplicación Móvil (Android - Kotlin)
- **Android SDK 35 / Kotlin / ViewBinding / Parcelize**
- **Hilt (DI)** – Inyección de dependencias moderna para Android.  
- **Room** – Base de datos local persistente.  
- **WorkManager** – Tareas en segundo plano.  
- **Firebase (Auth, Firestore, Storage, Analytics)** – Backend completo en la nube.  
- **Google Maps** – Integración de mapas.  
- **Retrofit + GSON + OkHttp** – Cliente HTTP eficiente para servicios REST.  
- **Glide** – Carga de imágenes eficiente.  
- **CameraX** – Control avanzado de cámara nativa.  
- **CircleImageView** – Avatares e imágenes redondas.  
- **Lifecycle & ViewModel + Coroutines** – Gestión reactiva y asincronía moderna.  
- **Network monitoring** – Detección de conectividad y reconexión.
- **Doxygen** - Documentación del proyecto de Android.

### ☁️ Backend  
- **Firebase 11**  
  - **Firestore** – Base de datos NoSQL en tiempo real.  
  - **Auth** – Autenticación de usuarios.  
  - **Hosting** – Despliegue de la app web.  
  - **Storage** – Gestión de imágenes y recursos multimedia.  

### 🧪 Testing y Calidad  
- **Jasmine + Karma** – Testing unitario en frontend.  
- **ESLint + Angular ESLint** – Linting y buenas prácticas de estilo.  
- **Compodoc** – Generador de documentación automática del proyecto Angular.  


### 📊 Análisis de Datos  
- **Python + Firebase** – Script para extraer datos desde Firestore a CSV. 
- **Exportación de datos (CSV)** – Los datos de la aplicación (p. ej. información de usuarios y fiestas) se exportaron desde Firebase a archivos CSV para su posterior análisis.  
- **Microsoft Power BI** – Herramienta de inteligencia de negocios utilizada para analizar los datos exportados y crear visualizaciones e informes interactivos que apoyan la toma de decisiones y la evaluación del proyecto.

---

## 🛡️ Esquema E/R de la Base de Datos

El modelo de datos de **PartyNow** está basado en una estructura de colecciones de Firebase Firestore y sigue un diseño E/R simple pero efectivo.

Cada entidad **Person** (usuario) puede representar tanto a una **persona** como a una **empresa**. Estas entidades están relacionadas con múltiples **Party** (fiestas), lo que configura una relación de **uno a muchos**.

### 🧩 Relación principal

> Cada usuario (persona o empresa) puede crear múltiples fiestas, lo que se refleja en la relación:  
> `Person (id)` 🔗 1 — N 🔗 `Party (personId)`

Esta arquitectura facilita:
- Consultas por usuario para obtener todas sus fiestas.
- Referencias inversas de cada fiesta hacia su creador.

---

## 🗃️ Colecciones principales

1. **Usuarios Persona** – Extensión del perfil de Firebase Auth para usuarios individuales.
2. **Usuarios Empresa** – Extensión del perfil para entidades organizadoras (empresas).
3. **Fiestas** – Eventos registrados por cualquier tipo de usuario.

---

### 👤 Usuario a nivel Persona

| Campo         | Tipo             | Descripción                     | Ejemplo                                      |
|---------------|------------------|----------------------------------|----------------------------------------------|
| `id`          | string            | ID del documento                 | `"V4uBmDZlaU09XFEIvrBe"`                      |
| `name`        | string            | Nombre                           | `"Alejandro"`                                 |
| `surname`     | string            | Apellidos                        | `"Giráldez Guerrero"`                         |
| `email`       | string            | Correo electrónico               | `"alexgg888999@gmail.com"`                    |
| `phone`       | string            | Número de teléfono               | `"644493197"`                                 |
| `birthday`    | string (fecha)    | Fecha de nacimiento              | `"20/04/2004"`                                |
| `country`     | string            | País del usuario                 | `"Spain"`                                     |
| `gender`      | string            | Género                           | `"male"`                                      |
| `type`        | string            | Tipo de usuario                  | `"person"`                                    |
| `image`       | string (URL)      | URL de imagen de perfil          | `"https://..."`                               |
| `user`        | string            | UID de Firebase Auth             | `"4fIHj6INZrRqzbr5owQ3oRhto3m2"`              |

---

### 🏢 Usuario a nivel Empresa

| Campo         | Tipo             | Descripción                     | Ejemplo                                      |
|---------------|------------------|----------------------------------|----------------------------------------------|
| `id`          | string            | ID del documento                 | `"fMd4iJqoVBY226BoacAi"`                      |
| `name`        | string            | Nombre de la empresa             | `"Alan Turing"`                               |
| `email`       | string            | Email de contacto                | `"alanturing@gmail.com"`                      |
| `phone`       | string            | Teléfono                         | `"680993322"`                                 |
| `location`    | string            | Ubicación                        | `"Spain"`                                     |
| `type`        | string            | Tipo de usuario                  | `"company"`                                   |
| `image`       | string (URL)      | Imagen                           | `"https://..."`                               |
| `user`        | string            | UID de Firebase Auth             | `"4fIHj6INZrRqzbr5owQ3oRhto3m2"`              |

---

### 🎉 Fiestas

| Campo         | Tipo             | Descripción                     | Ejemplo                                      |
|---------------|------------------|----------------------------------|----------------------------------------------|
| `id`          | string            | ID de la fiesta                  | `"8RDvsz5wo7P6uFt4kp8m"`                      |
| `name`        | string            | Nombre del evento                | `"FAN FUTURA"`                                |
| `country`     | string            | País                             | `"Spain"`                                     |
| `city`        | string            | Ciudad o dirección               | `"C. P.º del Gonio Los Alcázares, Murcia"`    |
| `price`       | number            | Precio de la entrada             | `65`                                          |
| `minAge`      | string            | Edad mínima requerida            | `16`                                          |
| `startDate`   | string (ISODate)  | Fecha y hora de inicio           | `"2025-07-17T17:00:00"`                       |
| `finishDate`  | string (ISODate)  | Fecha y hora de fin              | `"2025-07-20T06:00:00"`                       |
| `description` | string            | Descripción                      | `""`                                          |
| `personId`    | string            | ID del usuario creador           | `"V4uBmDZlaU09XFEIvrBe"`                      |

---

### 🔗 Relaciones exactas

- `person.user` → UID en Firebase Auth  
- `company.user` → UID en Firebase Auth  
- `party.personId` → `person.id` (o `company.id`)  

> Esta estructura flexible permite consultar todos los eventos organizados por un usuario, identificar su tipo (persona o empresa), y mantener sincronización con el sistema de autenticación de Firebase.


---

## 🔗 Enlaces del proyecto

### 🌍 Aplicación Web

- 💻 **Repositorio (Ionic + Angular)**  
  [https://github.com/imal3xg/partynow](https://github.com/imal3xg/partynow)

- 🔗 **Demo en Netlify**  
  [https://partynow.netlify.app](https://partynow.netlify.app/)

- 🔗 **Apk para Android de la App web (Angular + Ionic)**
  [Descargar desde Google Drive](https://drive.google.com/file/d/1eXm6TIs-E5u7i6rdIIGJPPiTJbJWxjRW/view?usp=drive_link)

- 🎥 **Video Manual Detallado (Ionic + Angular)**  
  [Ver video](https://drive.google.com/file/d/1AS94PbPWDWve4Fw9Mq2cV_x49TWESoJB/view?usp=drive_link)

  [Ver video sobre la responsividad](https://drive.google.com/file/d/1VYgMvTqAa9fwqXPFVuFfLEioJCa-DISh/view)

---

### 📱 Aplicación Móvil

- 📱 **Repositorio (Kotlin)**  
  [https://github.com/imal3xg/partynowadd](https://github.com/imal3xg/partynowadd)

- 🔗 **Apk para Android de la App (Kotlin)**
  [Descargar desde Google Drive](https://drive.google.com/file/d/1urQUuNzWyq-ti8IWMqCVWdchmzt_nDj5/view?usp=drive_link)

- 🎥 **Video Manual Detallado (Kotlin)**
  [Ver video](https://drive.google.com/file/d/1jN6-MPFFnWEbdQBaTnwuiAdLWGkf1grn/view?usp=drive_link)

---

### 🧠 Procesamiento de datos

- 🐍 **API en Python para generar CSV a partir de datos de Firebase**  
  [https://github.com/imal3xg/partynow-csv](https://github.com/imal3xg/partynow-csv)

⚠️ Nota importante sobre Render (plan gratuito)

Render, al estar en su modalidad gratuita, pone las aplicaciones en estado de suspensión cuando no reciben tráfico durante un tiempo.  
Esto significa que:

- La **primera solicitud después de un rato inactivo puede tardar entre 20 y 30 segundos** en responder (Render "despierta" la instancia).
- Las siguientes solicitudes funcionarán con normalidad.

Se recomienda tener paciencia al hacer la primera llamada si la API ha estado inactiva por un tiempo.

---

### 🎨 Diseño de la interfaz

- 🖼️ **Prototipo en Balsamiq (solo visualización)**  
  [Enlace a Balsamiq](https://balsamiq.cloud/soqlapt/pkyu81e)

- 📁 **Archivos descargables de Balsamiq (Google Drive)**  
  [Enlafe a Google Drive](https://drive.google.com/drive/folders/1Kujc-XIfwvdJHCBXHMALyN4b1bIbfGtj?usp=drive_link)

- 🎯 **Diseño en Figma (modo solo visualización)**  
  [Enlace a Figma](https://www.figma.com/design/rtPK2IWOK2aN3XO6yANVgy/PartyNow?node-id=0-1&t=hswUmFDALXAt5xCC-1)

---

### 📊 Análisis de datos

- 📥 **Power BI + CSV (descarga desde Drive)**  
  Incluye el archivo `.pbix` y los CSV exportados desde la app.  
  [Enlace a Google Drive](https://drive.google.com/drive/folders/127X1JsERo1u3Pd9Nz3DxdUlcQyUu0sof?usp=drive_link)

---

# 🖥️ Presentación del Proyecto

## 📄 PDF de la Presentación
El PDF de la presentación está disponible en el repositorio del proyecto, junto al `README.md`.

## 🎥 Versión Recomendada con Vídeos y Transiciones
Se recomienda visualizar la presentación interactiva en Canva para una mejor experiencia, con vídeos incluidos:

- [Ver presentación en Canva](https://www.canva.com/design/DAGqccqNtGw/dOBe0oM2ltTMgXWDtQQ-dA/edit?utm_content=DAGqccqNtGw&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

> Contiene todos los vídeos y animaciones que enriquecen la experiencia.

---

## ✨ Características Principales

### ✍️ Registro y Perfiles  
**Regístrate** como persona o como empresa.  
**Perfiles Completos:** Cada perfil muestra tu foto, nombre (o nombre de la empresa), apellidos, género, fecha de nacimiento y el número de publicaciones (eventos creados).  
**Edita tu Perfil:** Modifica tu foto, nombre, apellidos, género y fecha de nacimiento. Si eres una empresa, también puedes actualizar tu ubicación (país, dirección o ciudad).  

### 🔑 Inicio de Sesión Continuo  
**Autologin:** Disfruta de una experiencia sin interrupciones. Una vez que inicies sesión, la aplicación recordará tus credenciales para futuras visitas, tanto en la web como en la app móvil.  

### 🎉 Gestión de Eventos (Fiestas)  
**Descubre Fiestas:** Explora y visualiza eventos y celebraciones en todo el mundo, con la opción de filtrarlos por país.  
**Crea tus Eventos:** Organiza y publica tus propias fiestas, celebraciones o eventos.  
**Edita y Elimina:** Tienes control total para modificar o borrar los eventos que hayas creado.  

### 👥 Conecta con Otros Usuarios  
**Busca Usuarios:** Encuentra fácilmente a otras personas o empresas dentro de la red.  
**Visita Perfiles:** Accede a los perfiles de otros usuarios para ver sus publicaciones y obtener más información.  
**Contacta Directamente:** Comunícate con otros usuarios por correo electrónico o llamada telefónica desde la aplicación.  

### 🌐 Soporte Multilingüe  
**Aplicación Web:** Cambia el idioma directamente entre español e inglés.  
**Aplicación Móvil (Android):** Disponible en español, inglés, francés, alemán e italiano. Para cambiar el idioma, deberás modificar la configuración de idioma de tu dispositivo.  

### 👑 Panel de Administración  
**Acceso Exclusivo:** Si eres administrador, un menú lateral te dará acceso a una sección especial.  
**Gestiona Permisos:** Otorga o retira permisos de administrador a otros usuarios.  
**Control de Cuentas:** Elimina cuentas de usuario, lo que también borrará todos los eventos asociados a esa cuenta.  

### 🏠 Portada y "Acerca de Mí"  
La página principal de la aplicación también funciona como una sección **"Acerca de"**, donde encontrarás información sobre el desarrollador y enlaces a mi **GitHub, LinkedIn y correo electrónico**.

## 🛠️ Detalles Técnicos por Plataforma

### 🌍 Aplicación Web (Ionic + Angular)  
**IA Generativa para Descripciones:** Al crear o editar una fiesta, tienes la opción de generar una descripción con Inteligencia Artificial. Un botón específico enviará un prompt a un modelo de IA (como ChatGPT) para obtener sugerencias, haciendo que tus eventos sean más atractivos y modernos.  
**Opción de compartir fiestas:** Tanto desde la página principal, como en el perfil de cada usuario (incluyendo el del usuario conectado) se podrá compartir fiestas por distintos navegadores en formato texto, incluyendo el nombre de la fiesta, los detalles, la descripción, y un enlace a la web. Dependiendo del idioma en el que esté la web en el momento de compartir, se enviarán los detalles en ese lenguaje.

### 📱 Aplicación Móvil (Kotlin)  
**Temas Claro y Oscuro:** La aplicación ofrece un diseño con temas claro y oscuro completamente contrastados para una experiencia visual personalizable.  
**Notificaciones de Creación de Fiesta:** Al momento de crear una fiesta, se envía una notificación directa al dispositivo del usuario (gestionada con NotificationManager) para confirmar la creación. Pulsando en la notificación, se redirige al usuario automáticamente a los detalles de la fiesta creada.  
**Modo Offline Robusto:** Gracias a la integración de **Room** para almacenamiento local y **WorkManager** para la gestión de tareas en segundo plano, la aplicación funciona eficazmente incluso en modo avión. Puedes visualizar las fiestas y perfiles cargados la última vez que tuviste conexión. Además, es posible **crear, modificar y eliminar fiestas**, aunque los cambios no se sincronizarán con Firebase ni serán visibles para otros usuarios hasta que se restablezca la conexión a internet.

---

## 🧑‍💻 Desarrollador Principal

**Alejandro Giráldez Guerrero**  
*Estudiante de 2º Desarrollo de Aplicaciones Multiplataforma*

🏛️ **Centro docente** CPIFP Alan Turing
✉️ **Contacto:** alexgg888999@gmail.com  
💻 **GitHub:** [imal3xg](https://github.com/imal3xg)