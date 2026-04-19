# Capítulo V: Product Implementation, Validation & Deployment.

## 5.1. Software Configuration Management. 
Para tener consistencia y seguimiento de el desarrollo de la plataforma, se ha definido una serie de herramientas y estrategias de desarrollo. El metodo cubre la configuracion del entorno de desarrollo, la gestion del codigo y el despliegue, alineado a las buenas prácticas de ingenieria de software y metodologias ágiles.
### 5.1.1. Software Development Environment Configuration. 
Para facilitar la colaboración del equipo en todas las actividades del ciclo de vida de desarrollo de Urban Safe, se ha definido un entorno de desarrollo común. Este entorno está compuesto por herramientas especializadas para la gestión del proyecto, diseño UX/UI, modelado, desarrollo, pruebas, documentación y despliegue. La selección de estas herramientas se basa en criterios de eficiencia, compatibilidad con tecnologías open-source (Java + web), y alineación con prácticas recomendadas de la industria.
|        Categoría        |      Herramienta      |                                               Propósito                                               |                                      Tipo de acceso/enlace                                      |
| :---------------------: | :-------------------: | :---------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------: |
|    Project Management   |         Trello        |           Gestión del backlog, tareas y sprints del equipo usando metodología ágil (Scrum).           |                             [https://trello.com](https://trello.com)                            |
| Requirements Management |       UXPressia       |                  Creación de User Personas, Journey Maps y artefactos de needfinding.                 |                          [https://uxpressia.com](https://uxpressia.com)                         |
|   Product UX/UI Design  |         Figma         |                Diseño de wireframes, mockups y prototipos de la aplicación web y móvil.               |                              [https://figma.com](https://figma.com)                             |
|   Modelado de Software  |    LucidChart / Miro / Structurizr     |                 Modelado de arquitectura (UML, C4, Event Storming, Bounded Contexts).                 |               [https://www.lucidchart.com/](https://www.lucidchart.com/)     / [https://miro.com/](https://miro.com/) / [https://structurizr.com/](https://structurizr.com/)               |
|   Frontend Development  |   Visual Studio Code  |                 Desarrollo del Landing Page y Web Application (HTML, CSS, JavaScript).                |                  [https://code.visualstudio.com](https://code.visualstudio.com)                 |
|   Backend Development   |     IntelliJ IDEA     |     Desarrollo del RESTful API en Java (Spring Boot) siguiendo arquitectura orientada a servicios.    |                [https://www.jetbrains.com/idea/](https://www.jetbrains.com/idea/)               |
|       API Testing       |        Postman        |                           Pruebas y validación de endpoints del API RESTful.                          |                        [https://www.postman.com](https://www.postman.com)                       |
|     Version Control     |         GitHub        | Control de versiones del código fuente y documentación colaborativa (GitFlow + Conventional Commits). |                             [https://github.com](https://github.com)                            |
|  Software Documentation |        Markdown       |                     Redacción del informe del proyecto bajo enfoque Docs-as-Code.                     |                            Compatible con GitHub / editores de texto                            |


### 5.1.2. Source Code Management. 
Los repositorios utilizados para el desarrollo de código fuente son los siguientes:

<div align="center">

| Producto Digital | URL del Repositorio | 
|:----------------:|:-------------------:|
| Landing Page | https://github.com/Aurora-startup/SupplyWok-landing-page | 
| Web Services (Backend API) |https://github.com/Aurora-startup/SupplyWok-backend  |
| Frontend Web Application | https://github.com/Aurora-startup/SupplyWok-frontend|

</div>

---

**Modelos de Ramificación**

Se implementará GitFlow, un modelo de ramificación estructurado, el cual permite separar de manera clara las etapas de desarrollo, pruebas, liberación y mantenimiento.

**La estructura de ramas en GitFlow será:**

- _Main_: Contiene el código en estado estable y listo para producción.
- _Develop_: Rama de integración para desarrollo activo.
- _Feature branches_: Para nuevas funcionalidades.
    - Convención: `feature/nombre-descriptivo`  
    - Ejemplo: `feature/US007-business-profiles`
- _Release branches_: Para preparar versiones antes de pasar a producción.
    - Convención: `release/X.Y.Z`  
    - Ejemplo: `release/1.0.0`
- _Hotfix branches_: Para correcciones urgentes.
    - Convención: `hotfix/X.Y.Z`  
    - Ejemplo: `hotfix/1.0.1`        

**Versionado Semántico (Semantic Versioning)**

- Se utiliza Semantic Versioning 2.0.0, con el esquema MAJOR.MINOR.PATCH:

    - **MAJOR:** Cambios incompatibles.
    - **MINOR:** Funcionalidades nuevas retrocompatibles.
    - **PATCH:** Correcciones retrocompatibles.

    **Ejemplos de versiones:**  
    `v1.0.0`, `v1.1.0`, `v1.1.1`.

**Convenciones para Commits**

El equipo sigue el estándar de Conventional Commits para los mensajes de commits, lo que permite claridad en el historial y facilita la generación automática de changelogs:

`<type>[optional scope]: <description>`

Tipos comunes:

- `feat`: Nueva funcionalidad.
- `fix`: Corrección de errores.
- `docs`: Cambios en documentación.
- `style`: Cambios de formato sin impacto funcional.
- `refactor`: Reestructuración del código.
- `test`: Relacionados con pruebas.
- `chore`: Tareas de mantenimiento.

Ejemplo:
```
  feat(auth): implement login via OAuth
  fix(api): handle null user tokens
```
### 5.1.3. Source Code Style Guide & Conventions. 

Esta sección define los lineamientos y estándares que se seguirán durante el desarrollo del software, con el fin de garantizar un código uniforme, comprensible y fácil de mantener, alineado con buenas prácticas de la industria.

Se adoptarán convenciones ampliamente aceptadas para los lenguajes utilizados en el proyecto: HTML, CSS, JavaScript, TypeScript y Java. Asimismo, todos los nombres de variables, funciones, clases y demás identificadores estarán escritos en inglés.

---

#### Referencias utilizadas

Las siguientes guías servirán como base para la implementación de estándares de código:

- [Angular Style Guide (oficial)](https://angular.io/guide/styleguide)
- [Google TypeScript Style Guide](https://google.github.io/styleguide/tsguide.html)
- [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)
- [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)
- [HTML Style Guide and Coding Conventions - W3Schools](https://www.w3schools.com/html/html5_syntax.asp)
- [Spring Boot Features](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/)

---

#### Estructura del código

El proyecto se organizará en módulos según sus responsabilidades, separando claramente componentes como servicios, modelos, vistas, rutas y configuraciones.  
Este enfoque permite mejorar la escalabilidad del sistema y fomenta la reutilización de código, aplicando el principio de *Separation of Concerns*.

---

#### Convenciones de nomenclatura

| Elemento                    | Convención                         | Ejemplo                    |
|---------------------------|------------------------------------|----------------------------|
| Componentes Angular       | PascalCase + `Component`           | `UserProfileComponent`     |
| Servicios Angular         | PascalCase + `Service`             | `AuthService`              |
| Interfaces TypeScript     | PascalCase                         | `User`, `CourseDetails`    |
| Archivos                  | kebab-case                         | `user-profile.component.ts`|
| Variables / funciones     | camelCase                          | `getUserData()`            |
| Constantes                | UPPER_SNAKE_CASE                   | `MAX_LOGIN_ATTEMPTS`       |
| Clases Java              | PascalCase                         | `UserController`           |
| Métodos Java             | camelCase                          | `getUserById()`            |
| Paquetes Java            | minúsculas con puntos              | `com.example.module`       |

---

#### Lineamientos por lenguaje

##### TypeScript
- Uso de tipado fuerte y explícito.
- Se emplean `let` y `const`, evitando `var`.
- La lógica compleja se delega a servicios, no a componentes.
- Orden de imports: Angular → librerías externas → módulos internos.
- No se utiliza el prefijo `I` en interfaces.

##### JavaScript
- Configuración basada en ESLint y Prettier.
- Preferencia por funciones puras y código modular.
- Uso de camelCase en nombres.
- Prioridad a `const` y `let`.

##### HTML
- Etiquetas y atributos en minúsculas.
- Indentación de 2 espacios.
- Uso de comillas dobles en atributos.
- Se prioriza semántica y accesibilidad según HTML5.

##### CSS / SCSS
- Uso de metodología BEM (Block Element Modifier) para definir las clases:

```css
.button {}
.button--primary {}
.button__icon {}
```
- Estructura modular de estilos, agrupados por componente.

- Uso de variables SCSS para colores, fuentes y tamaños.

- Están prohibidos los estilos en línea y el uso indiscriminado de !important.

###### JAVA
- Organización por capas: controller, service, repository, model, etc.

- Uso de anotaciones estándar como `@RestController`, `@Service`, `@Repository`.

- Documentación con Javadoc en clases y métodos públicos.

- Acceso a atributos mediante métodos getter y setter.

- Se sigue el https://google.github.io/styleguide/javaguide.html

##### Internacionalización

Se utiliza el paquete `@ngx-translate/core` para la internacionalización de la interfaz.

Toda cadena visible al usuario se encuentra externalizada en archivos JSON, organizados por idioma.

Las claves de traducción están en mayúsculas y separadas por puntos para reflejar su estructura jerárquica.

```css
<h1>{{ 'LOGIN.TITLE' | translate }}</h1>
```

### 5.1.4. Software Deployment Configuration.  
La configuración de despliegue define los procesos y herramientas necesarias para publicar los distintos componentes del sistema: **Landing Page**, **API REST (Backend)** y **Web Application (Frontend)**.  
Este enfoque permite asegurar consistencia, trazabilidad y facilidad de mantenimiento durante el ciclo de vida del producto.

---

#### Despliegue del Landing Page

- **Tecnologías utilizadas:**  
  HTML5, CSS3, JavaScript, enfoque responsive.

- **Repositorio:**  
  [https://github.com/Aurora-startup/SupplyWok-landing-page](https://github.com/Aurora-startup/SupplyWok-landing-page)

- **Plataforma de hosting:**  
  GitHub Pages

- **Proceso de despliegue:**  
  - La rama `main` contiene la versión pública del sitio.  
  - El contenido estático se ubica en el directorio raíz del proyecto.  
  - Los cambios se integran desde la rama `develop` mediante pull requests validados.  
  - GitHub Pages realiza la publicación automáticamente al detectar actualizaciones en la rama principal.

---

#### Despliegue del Backend (RESTful API)

- **Tecnologías utilizadas:**  
  Java + Spring Boot

- **Repositorio:**  
  [https://github.com/Aurora-startup/SupplyWok-backend](https://github.com/Aurora-startup/SupplyWok-backend)

- **Plataforma de despliegue:**  
  Servicios Cloud (ej. Render, Railway, AWS o Azure)

- **Proceso de despliegue:**  
  - La aplicación se empaqueta utilizando Maven/Gradle (`.jar` ejecutable).  
  - Se configura el despliegue automático conectado al repositorio GitHub.  
  - Las variables sensibles (credenciales, conexión a base de datos, tokens) se gestionan mediante variables de entorno.  
  - El servicio se expone a través de endpoints REST accesibles mediante HTTP/HTTPS.  
  - Se asegura la correcta comunicación con servicios externos requeridos por el sistema.

---

#### Despliegue del Frontend Web Application

- **Tecnologías utilizadas:**  
  Framework SPA (Angular / Vue / React), HTML, CSS, TypeScript/JavaScript.

- **Repositorio:**  
  [https://github.com/Aurora-startup/SupplyWok-frontend](https://github.com/Aurora-startup/SupplyWok-frontend)

- **Plataforma de despliegue:**  
  Vercel / Netlify / GitHub Pages

- **Proceso de despliegue:**  
  - La aplicación se compila en modo producción (`npm run build`).  
  - La rama `main` se utiliza como fuente de despliegue.  
  - La plataforma seleccionada detecta cambios automáticamente y publica nuevas versiones.  
  - Se configura la URL del backend mediante variables de entorno para garantizar la integración con la API REST.

---

#### Consideraciones adicionales

- Se documentarán los pasos de despliegue en el repositorio principal del proyecto.  
- Se mantendrá una separación clara entre entornos (desarrollo, testing y producción).  
- Se realizarán pruebas posteriores al despliegue para validar la disponibilidad y funcionamiento del sistema.  
- Se contempla la integración de herramientas de automatización como **GitHub Actions** para implementar flujos de integración y despliegue continuo (CI/CD).
  
## 5.2. Landing Page, Services & Applications Implementation.
### 5.2.1. Sprint 1 
#### 5.2.1.1. Sprint Planning 1