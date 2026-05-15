# Capítulo IV: Product Design.
## 4.1. Style Guidelines
### 4.1.1. General Style Guidelines.

En esta sección se detallan los lineamientos de estilo que hemos decidido seguir para mantener la coherencia visual de la plataforma, la cual incluye la landing page, web y versiones mobile. Se detallaran el branding, paleta de colores y tipografias a utilizar en el proyecto.

#### 4.1.1.1. Branding.

El logo de nuestra plataforma está compuesto por los caracteres 'S' y 'W' provenientes del nombre SuppylWok, puestos de forma creativa para mantener una relacion con nuestro público objetivo. La 'S' encontrandose en forma de humo que sale de un recipiente que tiene la forma de 'W'. Transmitiendo una conexion con el entorno de un restaurante chifa generando familiaridad con nuestros usuarios.

![](../assets/images/supplywok-logo.png)

#### 4.1.1.2. Paleta de Colores.

La identidad visual de SupplyWok busca mantener una relacion con el entorno de un restaurante chifa clásico por lo que nuestro colores predominan rojos y amarillos, combinado con blancos y negros para un contraste optimo.

- **Rojo (#C21204):** Este color en la cultura china esta realacionado con la suerte y la prosperidad en los negocios[^1] que buscamos transmitir mediante el uso de nuestra paltaforma, además de ser un color que genera impacto visual. por lo que se usará en botones principales, alertas y elementos que requieran atención.
- **Amarillo (#E9B824):** Este color lo usamos como contraste al rojo y para resaltar textos en caso se requiera.
- **Mostaza o Amarillo oscuro (#AO7832):** Siendo una variante mas oscura del amarillo que tenemos se usaran en detalles para ayudar a armonizar la vista de nuestro usuarios.
- **Blanco (#FFFFFF):** Color neutro para mantener un balance en la paleta de colores.
- **Negro (#000000):** Color neutro para mantener un balance en la paleta de colores.

![](../assets/images/paleta_colores.png)

#### 4.1.1.3. Tipografía.

La tipografia que se ha decidido usar en nuestra plataforma son dos, Poppins y Monserrat. Estas elecciones fueron hechas pensando en la comodidad de lectura de nuestros usuarios, junto a un diseño moderno que se quiere lograr.

- **Títulos:** Para los titulos se usaran Poppins en pesos de Bold o semibold dependiendo del titulo, esto para dar una fuerza y relevancia necesarias en titulos.

![](../assets/images/poppins_example.png)

- **Párrafos o cuerpo del texto:** Se usara Monserrat en pesos variados como bold, regular o light dependiendo de la intencion del parrafo. Pensado en la legibilidad necesaria para los usuarios al momento de leer.

![](../assets/images/monserrat_example.png)


### 4.1.2. Web Style Guidelines.
## 4.2. Information Architecture

La arquitectura de información de SupplyWok está diseñada para dos contextos distintos: la **Landing Page**, orientada a captar y convertir visitantes en usuarios registrados, y la **Web Application**, donde los usuarios operan la plataforma según su rol. Ambos contextos tienen estructuras de navegación y organización de contenido diferenciadas, pero comparten un lenguaje visual y terminológico consistente.

### Landing Page

La Landing Page es el primer punto de contacto entre SupplyWok y sus potenciales usuarios. Su arquitectura de información está pensada para que el visitante comprenda el valor del producto, identifique su segmento (restaurante o proveedor) y tome acción hacia el registro, todo en un recorrido vertical y sin fricciones.

En la sección **Hero**, el visitante encuentra el mensaje principal de la plataforma acompañado de dos llamadas a la acción: una para iniciar el registro y otra para explorar más la propuesta de valor. Esta sección establece el tono visual y comunica la propuesta en una sola mirada.

En la sección **Cómo funciona**, se presenta el proceso de incorporación a la plataforma en tres pasos secuenciales: registro, configuración del inventario y gestión operativa. Esta sección reduce la percepción de complejidad para usuarios no técnicos.

En la sección **Funcionalidades principales**, se detallan las capacidades clave del producto: control de inventario, pedidos a proveedores, monitoreo IoT y proyección de demanda. Cada funcionalidad se presenta con un ícono representativo y una descripción breve.

En la sección **¿Para quién es SupplyWok?**, se presentan dos bloques diferenciados por segmento: uno para restaurantes y otro para proveedores, cada uno con sus beneficios específicos y un botón de registro con rol preseleccionado. Esto permite que el visitante se identifique con su perfil y acceda al flujo de registro correspondiente.

En la sección **Planes y precios**, se muestran los planes disponibles (Wok Premium y Wok Enterprise) con sus características y precios, incluyendo un botón de acción que redirige al formulario de registro con el plan preseleccionado.

En la sección **Preguntas frecuentes (FAQ)**, se resuelven dudas comunes sobre la plataforma, costos, integración de hardware IoT y diferencias respecto a otros sistemas.

En la sección **Footer**, el visitante puede acceder a enlaces legales (política de privacidad, términos de servicio), redes sociales, y datos de contacto del equipo Aurora.

### Web Application

La Web Application de SupplyWok organiza su contenido en dos espacios de trabajo distintos según el rol del usuario autenticado: la **Vista Restaurante** y la **Vista Proveedor**. Cada rol accede únicamente a las funcionalidades relevantes para su operación.

En la sección **Dashboard**, el usuario accede a un resumen del estado operativo del día. Desde esta pantalla puede visualizar las alertas de stock mínimo activas, los pedidos pendientes de confirmación, el nivel de ocupación de mesas y cualquier anomalía de temperatura registrada por los sensores IoT. Es el punto de entrada principal tras iniciar sesión y está pensada para que el administrador tome decisiones rápidas sin necesidad de navegar a otras secciones.

En la sección **Inventario**, el restaurante gestiona el registro completo de sus insumos. Cada producto incluye nombre, categoría, unidad de medida, cantidad actual en stock, stock mínimo configurado y proveedor asociado. Desde aquí se pueden registrar entradas de mercadería, descontar unidades consumidas y actualizar la información de cualquier insumo.

En la sección **Pedidos**, el restaurante crea, gestiona y hace seguimiento de sus órdenes de abastecimiento. Cada pedido tiene un estado visible (Pendiente, En camino, Entregado, Cancelado) que se actualiza en tiempo real. El historial de pedidos permite revisar órdenes anteriores.

En la sección **Kitchen Tickets / Comandas**, el personal gestiona las comandas activas del salón. Cada comanda está vinculada a una mesa y muestra los platos solicitados con su estado de preparación (En cola, En preparación, Listo). La cocina ve esta vista en tiempo real.

En la sección **Proveedores**, el restaurante accede al directorio de proveedores vinculados, con datos de contacto, categorías de insumos y historial de transacciones.

En la sección **Tables and Occupancy / Mesas y Ocupación**, el administrador visualiza el estado en tiempo real de cada mesa del salón (libre, ocupada, en espera), útil para coordinar el flujo del servicio.

En la sección **Alertas**, se concentran todas las notificaciones generadas por el sistema: stock mínimo alcanzado, temperatura fuera de rango configurado y eventos operativos críticos.

En la sección **Reportes**, el restaurante analiza métricas de consumo, evolución del inventario y proyección de demanda a través de gráficos y tablas exportables.

En la sección **Configuración**, se gestionan los datos del perfil del negocio, los umbrales de sensores IoT, los rangos seguros de temperatura y humedad, y las preferencias de notificación.

En la sección **Suscripción**, el usuario revisa su plan activo, consulta las funcionalidades disponibles y puede cambiar de plan según las necesidades del negocio.

El equipo de Aurora confía en que esta arquitectura permitirá a ambos tipos de usuario operar de manera más eficiente, reduciendo el tiempo dedicado a tareas manuales y mejorando la coordinación entre restaurantes y proveedores.

---

### 4.2.1. Organization Systems

El contenido de SupplyWok se organiza aplicando distintos esquemas según la naturaleza de cada sección y el flujo esperado del usuario. Se detalla también qué esquemas no se utilizan y la razón de esa decisión.

#### Esquemas utilizados

| Tipo de organización | Aplicación en SupplyWok | Justificación |
|---|---|---|
| Jerárquica | Landing Page, Dashboard principal de cada rol | Permite destacar la información más crítica (alertas de stock, estado de pedidos) y guiar al usuario hacia las acciones prioritarias sin sobrecargar la pantalla. |
| Secuencial | Registro de usuario, configuración inicial del inventario, creación de un pedido, flujo de comanda | Acompaña al usuario paso a paso en flujos que requieren completar etapas en orden. Reduce errores y abandono en procesos críticos. |
| Matricial | Gestión de inventario, historial de pedidos, panel de Kitchen Tickets | Permite visualizar múltiples variables simultáneamente (producto, cantidad, fecha, proveedor, estado) para facilitar comparaciones y toma de decisiones rápida. |

#### Esquemas no utilizados

| Tipo de organización | Razón de exclusión |
|---|---|
| Alfabético | Los insumos, proveedores y pedidos no tienen un orden natural por nombre. Los usuarios buscan por categoría, estado o fecha, no por orden de letra. Usar orden alfabético aumentaría el tiempo de búsqueda en lugar de reducirlo. |
| Por popularidad | La plataforma no es un marketplace ni tiene contenido editorial. No existe un concepto de "más visto" o "más popular" relevante para la operación de un restaurante. |
| Geográfico | Aunque los proveedores tienen zonas de cobertura, la plataforma no organiza su contenido por ubicación geográfica. La coordinación es por relación cliente-proveedor, no por mapa. |

#### Organización por contexto

**Landing Page**

| Sección | Tipo de organización |
|---|---|
| Hero + CTA | Jerárquica — el mensaje principal domina visualmente, los CTAs secundarios están subordinados |
| Cómo funciona | Secuencial — 3 pasos numerados con progresión clara |
| Funcionalidades | Matricial — grid de features comparables entre sí |
| ¿Para quién? | Por audiencia — dos bloques diferenciados por segmento (restaurante / proveedor) |
| Planes y precios | Matricial — tabla comparativa de planes con características en filas |
| FAQ | Por tópicos — agrupadas por tipo de duda (producto, precio, hardware, soporte) |

**Web Application — Vista Restaurante**

| Sección | Tipo de organización |
|---|---|
| Dashboard | Jerárquica — alertas críticas primero, métricas secundarias después |
| Inventario | Matricial — tabla con columnas de producto, stock actual, stock mínimo, estado |
| Pedidos | Cronológico + Matricial — ordenados por fecha, filtrable por estado |
| Kitchen Tickets | Secuencial — flujo de estado: Cola → En preparación → Listo → Entregado |
| Alertas | Cronológico — ordenadas por hora de generación, más recientes primero |
| Reportes | Matricial — métricas comparables por periodo y por insumo |

**Web Application — Vista Proveedor**

| Sección | Tipo de organización |
|---|---|
| Dashboard | Jerárquica — pedidos urgentes primero, demanda proyectada como contexto |
| Pedidos recibidos | Cronológico + por estado — ordenados por fecha de entrega esperada |
| Mis clientes | Matricial — comparativa de frecuencia, monto y demanda por cliente |
| Catálogo | Matricial — productos con precio, unidad y disponibilidad en columnas |

---

### 4.2.2. Labeling Systems

El sistema de etiquetado de SupplyWok usa términos directos en español (con excepciones técnicas como "Dashboard" o "IoT" que son de uso común en el sector), asegurando que cada etiqueta esté anclada a un elemento concreto de la interfaz.

#### Navbar — Landing Page

| Etiqueta | Elemento | Destino |
|---|---|---|
| SupplyWok (logo) | Enlace en navbar | Ancla a sección Hero (#hero) |
| ¿Cómo funciona? | Enlace de navegación | Ancla a sección #como-funciona |
| Segmentos | Enlace de navegación | Ancla a sección #para-quien |
| Precios | Enlace de navegación | Ancla a sección #precios |
| Iniciar sesión | Botón secundario (outline) | Redirige a /login |
| Registrarse | Botón primario (filled) | Redirige a /register |

#### Hero — Landing Page

| Etiqueta | Elemento | Acción |
|---|---|---|
| Comenzar gratis | Botón CTA primario | Redirige a /register |
| Ver cómo funciona | Botón CTA secundario | Ancla a sección #como-funciona |

#### Sección Segmentos — Landing Page

| Etiqueta | Elemento | Acción |
|---|---|---|
| Empezar como restaurante | Botón en card de restaurante | Redirige a /register?rol=restaurante |
| Empezar como proveedor | Botón en card de proveedor | Redirige a /register?rol=proveedor |

#### Formulario de Registro (/register)

| Etiqueta | Elemento | Tipo |
|---|---|---|
| Tipo de cuenta | Selector de rol | Radio button: Restaurante / Proveedor |
| Nombre del negocio | Input de texto | Campo obligatorio |
| Correo electrónico | Input de email | Campo obligatorio |
| Contraseña | Input de contraseña | Campo obligatorio |
| Crear cuenta | Botón de submit | Primario |
| ¿Ya tienes cuenta? Inicia sesión | Enlace | Redirige a /login |

#### Formulario de Login (/login)

| Etiqueta | Elemento | Tipo |
|---|---|---|
| Correo electrónico | Input de email | Campo obligatorio |
| Contraseña | Input de contraseña | Campo obligatorio |
| Iniciar sesión | Botón de submit | Primario |
| ¿Olvidaste tu contraseña? | Enlace | Redirige a /forgot-password |
| ¿No tienes cuenta? Regístrate | Enlace | Redirige a /register |

#### Sidebar — Web Application

| Etiqueta | Ícono | Ruta |
|---|---|---|
| Dashboard | Cuadrícula | /dashboard |
| Inventory / Inventario | Caja | /inventory |
| Orders / Pedidos | Documento | /orders |
| Kitchen Tickets | Ticket | /kitchen |
| Suppliers / Proveedores | Camión | /suppliers |
| Tables and Occupancy | Mesa | /tables |
| Alerts / Alertas | Campana | /alerts |
| Reports / Reportes | Gráfico | /reports |
| Configuration / Configuración | Engranaje | /settings |
| Subscription / Suscripción | Escudo | /subscription |

#### Header — Web Application

| Etiqueta | Elemento | Acción |
|---|---|---|
| Nombre del restaurante / proveedor | Texto en header | Identificación del negocio activo |
| Plan actual (ej: Premium) | Badge | Redirige a /subscription |
| Ícono de notificaciones | Campana con contador | Abre panel lateral de alertas |
| Avatar del usuario | Foto o iniciales | Abre menú: Perfil / Configuración / Cerrar sesión |

#### Botones de acción contextual — Web Application

| Sección | Etiqueta del botón principal | Acción |
|---|---|---|
| Inventario | + Agregar insumo | Abre formulario de nuevo insumo |
| Pedidos | + Crear pedido | Abre formulario de nueva orden de compra |
| Kitchen Tickets | + Nueva comanda | Abre formulario de nueva comanda |
| Proveedores | + Agregar proveedor | Abre formulario de nuevo proveedor |
| Alertas | Marcar como revisada | Cambia estado de la alerta |
| Reportes | Exportar PDF / CSV | Descarga el reporte en el formato seleccionado |

#### Breadcrumbs — Web Application

| Vista | Breadcrumb mostrado |
|---|---|
| Detalle de pedido | Pedidos › Pedido #PO-8821 |
| Detalle de insumo | Inventario › Arroz jazmín |
| Detalle de comanda | Kitchen Tickets › Mesa 12 |
| Detalle de proveedor | Proveedores › Global Foods Ltd. |

#### Estados y badges

| Etiqueta | Color | Contexto |
|---|---|---|
| Urgent / Urgente | Rojo | Stock crítico en Dashboard |
| Alert | Naranja | Temperatura fuera de rango |
| Low stock | Rojo | Estado de insumo en Inventario |
| Preventive alert | Naranja | Insumo próximo al mínimo |
| Pending / Pendiente | Gris | Estado de pedido |
| In transit / En camino | Azul | Estado de pedido |
| Delayed / Retrasado | Rojo | Estado de pedido |
| In Prep | Naranja | Estado de comanda en cocina |
| Ready / Listo | Verde | Estado de comanda en cocina |
| Queue / En cola | Gris | Estado de comanda en cocina |

---

### 4.2.3. SEO Tags and Meta Tags

Se definen las etiquetas SEO y Meta Tags para las páginas principales de SupplyWok, tanto de la Landing Page como de las vistas clave de la Web Application.

**Home — Landing Page (/)**

- **Title:** SupplyWok | Gestión inteligente de abastecimiento para restaurantes
- **Meta Description:** Controla tu inventario, anticipa la demanda y coordina pedidos con tus proveedores desde una sola plataforma. Diseñada para restaurantes chifa y negocios gastronómicos.
- **Meta Keywords:** gestión de inventario restaurantes, abastecimiento chifa, control de stock, proveedores restaurantes, software gastronómico Perú
- **Meta Author:** Aurora

**Planes y Precios — Landing Page (/#precios)**

- **Title:** Planes y Precios | SupplyWok
- **Meta Description:** Conoce los planes Wok Premium y Wok Enterprise. Elige el que mejor se adapta al tamaño y necesidades de tu restaurante o negocio proveedor.
- **Meta Keywords:** precio software restaurante, plan gestión inventario, suscripción SupplyWok, plan premium chifa
- **Meta Author:** Aurora

**Login — Web Application (/login)**

- **Title:** Iniciar sesión | SupplyWok
- **Meta Description:** Accede a tu cuenta de SupplyWok para gestionar tu inventario, pedidos y operación en tiempo real.
- **Meta Keywords:** login SupplyWok, iniciar sesión restaurante, acceso plataforma
- **Meta Author:** Aurora

**Registro — Web Application (/register)**

- **Title:** Crear cuenta | SupplyWok
- **Meta Description:** Regístrate en SupplyWok como restaurante o proveedor. Empieza a gestionar tu inventario y abastecimiento de forma inteligente.
- **Meta Keywords:** registro SupplyWok, crear cuenta restaurante, registrar proveedor insumos
- **Meta Author:** Aurora

**Dashboard — Web Application (/dashboard)**

- **Title:** Dashboard | SupplyWok
- **Meta Description:** Accede a tu panel de control para monitorear stock, pedidos, alertas IoT y ocupación de mesas en tiempo real.
- **Meta Keywords:** panel restaurante, control operativo, alertas stock, monitoreo IoT
- **Meta Author:** Aurora

**Inventario — Web Application (/inventory)**

- **Title:** Inventario | SupplyWok
- **Meta Description:** Gestiona el inventario de tu restaurante. Registra entradas, controla el stock y recibe alertas de reabastecimiento automáticas.
- **Meta Keywords:** inventario restaurante, control de insumos, stock chifa, alertas stock mínimo
- **Meta Author:** Aurora

**Pedidos — Web Application (/orders)**

- **Title:** Pedidos | SupplyWok
- **Meta Description:** Crea y haz seguimiento de tus órdenes de compra a proveedores. Visualiza el estado de cada pedido en tiempo real.
- **Meta Keywords:** órdenes de compra restaurante, pedidos proveedores, seguimiento abastecimiento
- **Meta Author:** Aurora

---

### 4.2.4. Searching Systems

SupplyWok implementa sistemas de búsqueda y filtrado en las secciones donde el volumen de datos lo requiere. Para cada sistema se describe tanto la entrada de búsqueda como la presentación de los resultados.

| Sección | Filtros y búsquedas disponibles | Cómo se ven los resultados |
|---|---|---|
| Inventario | Búsqueda por nombre de insumo; filtro por categoría (carnes, verduras, condimentos, bebidas) | La tabla se filtra en tiempo real mostrando solo las filas coincidentes. Columnas visibles: Producto, Stock actual, Stock mínimo, Estado, Proveedor. Los insumos críticos aparecen con badge rojo "Low stock" al inicio de la lista. El filtro de categoría activo se muestra como chip sobre la tabla con opción de eliminarlo. |
| Pedidos | Búsqueda por número de orden o nombre de proveedor; filtro por estado (Pendiente, En camino, Entregado, Cancelado); filtro por rango de fechas | La tabla muestra solo las órdenes que coinciden. Cada fila muestra: ID de orden, Proveedor, Estado (badge de color), Fecha de entrega. El contador de resultados se actualiza ("3 pedidos encontrados"). Para el filtro de fechas se muestra un date picker con inicio y fin; los resultados se ordenan cronológicamente dentro del rango. |
| Proveedores | Búsqueda por nombre de proveedor o tipo de insumo que suministra | Lista de tarjetas filtrada en tiempo real. Cada tarjeta muestra nombre del proveedor, categoría de insumos y estado de vínculo (activo / inactivo). |
| Alertas | Filtro por tipo de alerta (stock, temperatura, operativa); filtro por período (rango de fechas) | La lista muestra solo las alertas del tipo o período seleccionado, ordenadas cronológicamente. Cada alerta muestra: tipo, descripción, fecha/hora y estado (Revisada / Pendiente). El total de resultados se actualiza en el encabezado de la sección. |
| Kitchen Tickets | Filtro por estado de comanda (En cola, En preparación, Listo) | Solo se muestran las comandas con el estado seleccionado. Cada comanda muestra mesa, platos solicitados y tiempo transcurrido desde la creación. |
| Catálogo (Proveedor) | Búsqueda por nombre de producto | Lista del catálogo filtrada en tiempo real. Cada resultado muestra: nombre, precio unitario, unidad de medida y disponibilidad (activo / desactivado). |
| Mis clientes (Proveedor) | Búsqueda por nombre de restaurante cliente | Se muestra la tarjeta del restaurante encontrado con su historial de pedidos recientes, frecuencia de compra y demanda proyectada. |
 

---

### 4.2.5. Navigation Systems

SupplyWok tiene dos contextos de navegación diferenciados: la **Landing Page**, cuya navegación guía al visitante hacia el registro, y la **Web Application**, cuya navegación permite al usuario operar la plataforma desde cualquier sección.

#### Navegación — Landing Page

| Elemento | Descripción |
|---|---|
| Navbar fija | Barra superior visible en todo momento durante el scroll. Contiene logo, enlaces a secciones (anclas) y botones de Iniciar sesión / Registrarse. En mobile se colapsa en menú hamburguesa. |
| Anclas de sección | Los enlaces del navbar desplazan suavemente (smooth scroll) a cada sección de la página: #hero, #como-funciona, #funcionalidades, #para-quien, #precios, #faq. |
| CTA primario en Hero | Botón "Comenzar gratis" redirige a /register. Es el punto de conversión principal de la landing. |
| CTA secundario en Hero | Botón "Ver cómo funciona" hace scroll a la sección #como-funciona, manteniendo al usuario en la landing para informarse antes de registrarse. |
| CTAs por segmento | En la sección "¿Para quién es SupplyWok?", cada card (restaurante / proveedor) tiene un botón que redirige a /register con el parámetro de rol preseleccionado (?rol=restaurante o ?rol=proveedor). |
| CTA en sección Precios | Cada plan tiene un botón que redirige a /register con el plan preseleccionado, reduciendo pasos en el onboarding. |
| CTA final (bottom of page) | Sección de cierre con un último llamado a la acción antes del footer, dirigido a usuarios que llegaron al final sin convertir. |
| Footer | Contiene enlaces a páginas legales (política de privacidad, términos), redes sociales y el enlace de inicio de sesión para usuarios ya registrados. |

#### Navegación — Web Application

| Elemento | Descripción |
|---|---|
| Sidebar  | Menú principal fijo a la izquierda, visible en todo momento. Contiene accesos directos a todas las secciones del rol activo con ícono y etiqueta. En mobile se colapsa en hamburguesa. |
| Header | Barra superior con nombre del negocio, badge del plan activo, ícono de notificaciones con contador y avatar del usuario con menú desplegable (Perfil / Configuración / Cerrar sesión). |
| Dashboard como home | Tras iniciar sesión, el usuario es redirigido automáticamente al Dashboard de su rol. El Dashboard funciona como hub de acceso rápido: las tarjetas de métricas (low stock, pending orders, alerts) son clicables y llevan a la sección correspondiente. |
| Breadcrumbs | Visibles en vistas de detalle para indicar la ruta actual y permitir la navegación hacia atrás. Ejemplo: Pedidos › #PO-8821. |
| Botones de acción contextual | Cada sección tiene un botón primario ("+ Agregar insumo", "+ Crear pedido") ubicado en la esquina superior derecha del contenido, accesible sin scroll. |
| Panel de notificaciones | Al hacer clic en el ícono de campana del header, se despliega un panel lateral con las alertas recientes ordenadas cronológicamente. Cada alerta tiene un acceso directo a la sección donde ocurrió el evento. |
| Modo restringido | El dueño puede activar un modo de acceso limitado desde Configuración. En este modo solo son visibles Kitchen Tickets y Tables and Occupancy, ocultando las secciones administrativas. Útil para personal de cocina y servicio. |
| Cambio de rol | Si un usuario tiene ambos roles (restaurante y proveedor), puede cambiar de vista desde un selector en el header sin cerrar sesión. |
---
## 4.3. Landing Page UI Design.
Durnate la elaboración de la landing page se utilizaropn los principios de diseño, utlizando diferentes secciones que muestran la información.
### 4.3.1. Landing Page Wireframe.
#### Desktop
![](../assets/images/figma/landingpage-desktop-wireframe.png)

#### Mobile
![](../assets/images/figma/landingpage-mobile-wireframe.png)

### 4.3.2. Landing Page Mock-up.
#### Desktop
![](../assets/images/figma/landingpage-desktop-mockup.png)

#### Mobile
![](../assets/images/figma/landingpage-mobile-mockup.png)


## 4.4. Web Applications UX/UI Design.

La propuesta UX/UI de las Web Applications de SupplyWok está diseñada para responder a dos necesidades principales: permitir que los restaurantes gestionen su operación diaria con rapidez y dar a los proveedores visibilidad clara sobre pedidos, clientes y demanda proyectada. A partir de ello, la interfaz prioriza acceso directo a módulos críticos, visualización rápida del estado operativo y reducción de pasos en las tareas más frecuentes.

### 4.4.1. Web Applications Wireframes.

Los wireframes de las Web Applications definen la estructura base de las vistas más relevantes del sistema antes de aplicar el diseño visual final. En ellos se observa la distribución de dashboards, formularios, tablas, tarjetas, paneles laterales y zonas de acción principal. Esta etapa permitió validar la relación entre jerarquía visual, arquitectura de información y flujos operativos por rol.

En escritorio, los wireframes muestran una estructura con sidebar, header superior y área central de trabajo, adecuada para dashboards, tablas y reportes. En mobile, la información se reorganiza en tarjetas y listas táctiles, reduciendo la complejidad visual sin perder funcionalidad.
![wireframes web](../assets/images/figma/wireframes-web.jpg)
![wireframe mobile1](../assets/images/figma/web-app-mobile-wireframe1.png)
![wireframe mobile2](../assets/images/figma/web-app-mobile-wireframe2.png)
[wireframe mobile3](../assets/images/figma/web-app-mobile-wireframe3.png)

### 4.4.2. Web Applications Wireflow Diagrams.

Los wireflows de SupplyWok muestran cómo cambian las pantallas wireframe a medida que el usuario avanza en un flujo concreto. Cada wireflow se construye a partir de un user goal y representa la secuencia de pasos necesarios para alcanzarlo, incluyendo decisiones intermedias y estados relevantes de la interfaz.

**User Goal 1: Registrar y controlar insumos del restaurante.**  
Este wireflow representa el recorrido del usuario restaurante desde el acceso al Dashboard hasta el módulo de Inventario, donde puede registrar un nuevo insumo, definir unidad de medida, stock mínimo y proveedor asociado. El flujo permite validar que la pantalla principal, la tabla de inventario y el formulario de creación estén conectados de manera lógica y con mínima fricción.

![wireflow1](../assets/images/figma/web-app-mobile-wireflow1.jpeg) 


**User Goal 2: Crear y dar seguimiento a un pedido de abastecimiento.**  
Este wireflow muestra cómo el restaurante inicia un pedido desde la sección de Pedidos, selecciona proveedor, agrega productos y revisa el estado del pedido una vez registrado. La secuencia evidencia una organización paso a paso que reduce errores y favorece la trazabilidad de la orden.

![wireflow](../assets/images/figma/web-app-mobile-wireflow2.jpeg)

**User Goal 3: Gestionar comandas y operación interna del restaurante.**  
Este wireflow representa el flujo mediante el cual el personal del restaurante registra una comanda, la asocia a una mesa y hace seguimiento a su avance dentro de la operación interna. La estructura permite visualizar con claridad los cambios de estado entre cola, preparación y listo.

![wireflow3](../assets/images/figma/web-app-mobile-wireflow3.jpeg)
**User Goal 4: Gestionar pedidos recibidos y catálogo del proveedor.**  
Este wireflow muestra el recorrido del proveedor desde su dashboard hacia pedidos recibidos, clientes o catálogo de productos, permitiéndole revisar demanda, actualizar disponibilidad y dar seguimiento a entregas. Esto valida la coherencia de la experiencia del segundo rol principal del sistema.

![wireflow4](../assets/images/figma/web-app-mobile-wireflow4.jpeg)

### 4.4.2. Web Applications Mock-ups.

![mockupweb1](../assets/images/figma/mockup-web1.png)
![mockupweb2](../assets/images/figma/mockup-web2.png)
![mockupweb3](../assets/images/figma/mockup-web3.png)
![mockupweb4](../assets/images/figma/mockup-web4.png)
![mockupweb5](../assets/images/figma/mockup-web5.png)
![mockupweb7](../assets/images/figma/mockup-web7.png)
![mockupweb8](../assets/images/figma/mockup-web8.png)
![mockupweb9](../assets/images/figma/mockup-web9.png)
![mockupweb10](../assets/images/figma/mockup-web10.png)
![mockupweb11](../assets/images/figma/mockup-web11.png)
![mockupweb12](../assets/images/figma/mockup-web12.png)

##### Login and Register Web

![mockupweblogin](../assets/images/figma/guides/login-guide.png)

**1)** La seleccion de idioma del sistema, pudiendo escojer entre ingles, español y chino. <br>
**2)** Es la seccion donde el usuario podra rellenar su información, en el caso del login pedira su correo y contraseña, mientras que para registarse pedira correo, contraseña, rol y plan de suscripción. <br>
**3)** Son los campos para rellenar la información solicitada, en el caso del login son solo dos campos, mientras que para registarse son cuatro. Ambos campos en login con un ejemplo de correo y contraseña. <br>
**4)** Son los textos interacctivos, estos redirigen al usuario a otras secciones del sistema segun indique el texto. <br>
**5)** El botón principal, en el caso del login permite iniciar sesión, mientras que en el registro redirigire al pago para crear la cuenta.

##### Dashboard Main Page

![dashboardmain](../assets/images/figma/guides/main-dashboard-guide.png)

**1)** La barra de navegación lateral de la plataforma, interactuando con ella te permite navegar a las diferentes secciones del sistema, como lo son el inventario, ordenes, comandas, proveedores, etc.

**2)** En seccion superior dentro de la pagina esta la vista general con la información pertinente del rol, en este caso el inventario con bajos niveles de stock como ejemplo.

**3)** En el Header se muestran las notificaciones, preguntas o dudas y el perfil del usuario.

**4)** El aparatado visual que muestra nuestra plataforma con el rol y el nombre asociado.

**5)** Una seccion que muestra con más detalle la información de los sensores disponibles.

**6)** Una seccion que muestra con más detalle las comandas y sus estados.

**7)** Este apartado muestra informacion del inventario, priorizando los productos que estan bajos de stock.

**8)** Un apartado que muestra las ordenes que se hacen a los proveedores.

##### Inventory Page

![inventorypage](../assets/images/figma/guides/inventory-dashboard-guide.png)

**1)** La barra de navegación lateral de la plataforma, interactuando con ella te permite navegar a las diferentes secciones del sistema.

**2)** La sección más detallada del inventario, mostrando todos los productos registrados en forma de lista, contando con buscadores por escritura del usuario y otro seleccionable por categorías.

**3)** El item de la lista del inventario muestra el nombre del producto, el nivel de stock, categoria, proveedor y acciones como editar o eliminar el producto.

**4)** El botón prncipal de esta sección, el cual permite agregar un nuevo producto al inventario.

##### Orders Page

![orderspage](../assets/images/figma/guides/orders-dashboard-guide.png)

**1)** La barra de navegación lateral de la plataforma, interactuando con ella te permite navegar a las diferentes secciones del sistema.

**2)** Sección para crear ordenes a los proveedores, permite seleccionar el proovedor, fecha  y prioridad; tambien añade los productos que se quieren pedir añadiendo lineas en forma de listas e indicando el precio. Contiene tambien el boton que enviaria la orden al proveedor.

**3)** Apartado para ver el seguimiento de las ordenes realizadas a proveedores, se muestran en forma de listas.

##### Kitchen Tickets Page

![kitchentickets](../assets/images/figma/guides/kitchen-tickets-guide.png)

**1)** La barra de navegación lateral de la plataforma, interactuando con ella te permite navegar a las diferentes secciones del sistema.

**2)** Una vista rapida de las comandas mostrando cuantas estan abiertas, en preparacion y listas.

**3)** Vista detallada de las comandas, mostrando a que mesa pertenece, el estado de la comanda y su fecha de creación, con acciones que se pueden hacer a cada comanda como eliminarlo.

**4)** El botón principal, el cual permite crear una nueva comanda.

##### Suppliers Page

![supplierspage](../assets/images/figma/guides/supliers-guide.png)

**1)** La barra de navegación lateral de la plataforma, interactuando con ella te permite navegar a las diferentes secciones del sistema.

**2)** Lista detallada de los proveedores disponibles en la plataforma, la información que muestra en en formato de listas con el nombre del proveedor, datos de contacto, categorías de suministros, etc. Tambien cuenta con un botón para pasar a la siguiente vista con más proveedores en caso hallan.

##### Tables Page

![tablespage](../assets/images/figma/guides/tables-guide.png)

**1)** La barra de navegación lateral de la plataforma, interactuando con ella te permite navegar a las diferentes secciones del sistema.

**2)** Vista simple de las mesas, mostrando las mesas ocupadas, libres y un porcentaje de ocupación.

**3)** Sección de búsqueda, uno por input del usuario y un seleccionable por zonas.

**4)** Apartado que muestra una vista detallada de las mesas con su número de comensales, estado, etc. Para ver todos es necesario hacer scroll hacia abajo.

##### Alerts Page

![alertspage](../assets/images/figma/guides/alerts-guide.png)

**1)** La barra de navegación lateral de la plataforma, interactuando con ella te permite navegar a las diferentes secciones del sistema.

**2)** Sección de búsqueda, uno por input del usuario y un seleccionable por prioridad.

**3)** Una lista detallada de las alertas notificadas, mostrando su prioridad, detalle, fuente, fecha, estado y como accion marcarlo como leída.

##### Reports Page

![reportspage](../assets/images/figma/guides/reports-guide.png)

**1)** La barra de navegación lateral de la plataforma, interactuando con ella te permite navegar a las diferentes secciones del sistema.

**2)** Botones para exportar los datos del reporte a formato PDF o CSV.

**3)** Sección de gráficos que permite ver los datos del reporte de forma visual. incluye la evolución del inventario, el comsumo por periodos, ordenes por proveedor e incidentes.

##### Settings Page

![settingspage](../assets/images/figma/guides/settings-guide.png)

**1)** La barra de navegación lateral de la plataforma, interactuando con ella te permite navegar a las diferentes secciones del sistema.

**2)** Sección del perfil del usuario. Permite cambiar datos y horarios, ademas de habilitar notificaciones por SMS o Email.

**3)** Lista de Usuarios que tiene acceso a las comandas, tanto para crearlas como asignarlas.

**4)** Bloqueador del sistema, permite bloquear las funciones del sistema para que el personal solo pueda ver las secciones autorizadas.

##### Subscription Plans Page

![subscriptionplanspage](../assets/images/figma/guides/subscripcions-guide.png)

**1)** La barra de navegación lateral de la plataforma, interactuando con ella te permite navegar a las diferentes secciones del sistema.

**2)** Sección de vista rapuda que muestra el plan actual, usuarios, locaciones y sensores que tiene el usuario.
**3)** Primer plan de suscripción, muestra sus beneficios, precio y un botón para adquirirlo, en caso ya lo tenga se desactiva y cambia el texto a "Plan Actual".

**4)** Segundo plan de suscripción, muestra sus beneficios, precio y un botón para adquirirlo, en caso ya lo tenga se desactiva y cambia el texto a "Plan Actual".


### 4.4.3. Web Applications User Flow Diagrams.

Los User Flow Diagrams de SupplyWok representan los recorridos funcionales principales de los usuarios dentro del sistema, considerando tanto la ruta esperada como posibles variantes o interrupciones. A diferencia del wireflow, aquí el foco está en la lógica de navegación, las decisiones del usuario y las condiciones que afectan la continuidad del flujo.

**User Goal 1: Mantener actualizado el inventario del restaurante.**  
Happy path: el usuario ingresa al Dashboard, accede a Inventario, selecciona la opción para agregar o editar un insumo, guarda la información y visualiza la actualización reflejada en la tabla principal.  
Unhappy path: el usuario omite campos obligatorios o ingresa valores inválidos; el sistema bloquea el guardado y muestra mensajes de validación.

![userflow1](../assets/images/figma/web-app-mobile-userflow1.jpeg)

#### mobile
![mockupmobile1](../assets/images/figma/web-app-mobile-mockup1.png)

![mockupmobile2](../assets/images/figma/web-app-mobile-mockup2.png)
![mockupmobil3](../assets/images/figma/web-app-mobile-mockup3.png)

**User Goal 2: Generar un pedido de abastecimiento correctamente.**  
Happy path: el restaurante accede al módulo de Pedidos, selecciona proveedor, agrega productos, confirma cantidades y registra la orden, quedando visible con estado pendiente.  
Unhappy path: no existe stock de referencia, no se selecciona proveedor o faltan productos; el sistema notifica el error y evita el registro incompleto.

![userflow2](../assets/images/figma/web-app-mobile-userflow2.jpeg)

**User Goal 3: Gestionar una comanda hasta su finalización.**  
Happy path: el personal registra una comanda, la asocia a una mesa, la cocina la procesa y el sistema actualiza su estado hasta marcarla como lista o entregada.  
Unhappy path: la mesa no está disponible, la comanda queda incompleta o el estado no puede avanzar por una inconsistencia operativa; el sistema informa la condición al usuario.

![userflow3](../assets/images/figma/web-app-mobile-userflow3.jpeg)

**User Goal 4: Dar seguimiento a pedidos desde la vista proveedor.**  
Happy path: el proveedor accede a pedidos recibidos, revisa el detalle, actualiza el estado del despacho y confirma la entrega.  
Unhappy path: el pedido está retrasado, faltan productos o el proveedor no puede confirmar entrega; el sistema permite registrar la incidencia y mantener trazabilidad del estado.

![userflow4](../assets/images/figma/web-app-mobile-userflow4.jpeg)

## 4.5. Web Applications Prototyping.

La fase de prototipado de SupplyWok permite simular la navegación y la interacción principal de las aplicaciones antes de su implementación final. Los prototipos fueron diseñados para validar la continuidad entre arquitectura de información, componentes de interfaz y flujos funcionales, tanto en escritorio como en mobile. Además del prototipo navegable en Figma, esta sección debe incorporar evidencia audiovisual del recorrido de uso, tal como solicita la rúbrica.

#### Escritorio
![desktop-prototype](../assets/images/figma/desktop-prototype.png)

[Prototipo Desktop](https://www.figma.com/proto/JUBnvZfJvlrpxIpW8ICRvS/SupplyWok?node-id=428-4042&p=f&t=kGhZbpCdqH2BntGS-0&scaling=scale-down&content-scaling=fixed&page-id=428%3A2335)

#### Mobile
![mobile-protoype](../assets/images/figma/mobile-prototype.png)

[prototipo mobile](https://www.figma.com/proto/JUBnvZfJvlrpxIpW8ICRvS/SupplyWok?node-id=428-2336&p=f&t=kGhZbpCdqH2BntGS-0&scaling=scale-down&content-scaling=fixed&page-id=428%3A2336)

#### Video prototype
[video de prototype desktop y mobile](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202318609_upc_edu_pe/IQDkq2Qv2M5aR40vWnyGaTpSAfxzErIKTIrpk9ecgyM3YHI?e=dJMWyy&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)


## 4.6. Domain-Driven Software Architecture.


### 4.6.1. Design-Level EventStorming.

En esta sección se detalla el proceso de Design-Level EventStorming realizado por el equipo para perfeccionar el modelo del dominio de Aurora. Partiendo del Big Picture, profundizamos en el comportamiento interno del sistema para alcanzar el mayor nivel de detalle arquitectónico posible.

Primero, refinamos la línea de tiempo original, eliminando eventos redundantes o procesos manuales que quedaban fuera del alcance tecnológico de la plataforma. Sobre este flujo depurado, incorporamos los elementos tácticos del Domain-Driven Design: Actores y Comandos para representar las intenciones, Políticas para las reglas automáticas, y Agregados (Aggregates) como responsables de procesar las operaciones y emitir los eventos de dominio. Este nivel de granularidad nos permitió consolidar y justificar las fronteras definitivas de nuestros Bounded Contexts.

Este contexto delimitado constituye el núcleo operativo para los restaurantes tipo chifa dentro de la plataforma Aurora. Su propósito principal es centralizar y automatizar el control de los insumos, transformando la gestión manual tradicional en un proceso preciso y basado en datos.

![](../assets/images/event-storming-e01.png)

Este contexto delimitado actúa como el puente transaccional entre los restaurantes tipo chifa y sus proveedores dentro del ecosistema Aurora. Su objetivo fundamental es digitalizar y estructurar la coordinación de pedidos de insumos, reemplazando las vías de comunicación informales por un flujo de trabajo centralizado y rastreable en la plataforma.

![](../assets/images/event-storming-e02.png)

Este contexto delimitado tiene como propósito supervisar las condiciones físicas críticas en las instalaciones del restaurante, específicamente en áreas vulnerables como la cocina y el almacén. Mediante la integración simulada de sensores IoT, el sistema monitorea variables ambientales clave de forma continua, tales como la temperatura y la humedad.

![](../assets/images/event-storming-e03.png)

Este contexto delimitado está diseñado para centralizar la gestión de los proveedores, brindándoles las herramientas necesarias para optimizar su logística y planificación comercial. A través de este módulo, los proveedores obtienen visibilidad sobre la demanda futura de sus clientes, lo que les permite gestionar sus catálogos de insumos y realizar un seguimiento detallado del estado de los pedidos recibidos.

![](../assets/images/event-storming-e04.png)

Este contexto delimitado representa la capa transversal de seguridad y administración comercial de la plataforma Aurora. Su propósito principal es proporcionar un entorno centralizado y seguro donde todos los usuarios puedan autenticarse, gestionar sus cuentas y recibir soporte técnico de manera eficiente.

![](../assets/images/event-storming-e05.png)

Este contexto delimitado representa el núcleo operativo del restaurante chifa dentro de la plataforma Aurora. Su propósito principal es orquestar la comunicación crítica entre el salón y la cocina, asegurando que los pedidos se procesen con precisión, se monitoreen en tiempo real y se mantenga la integridad operativa.

![](../assets/images/event-storming-e06.png)

### 4.6.2. Software Architecture Context Diagram.

![](../assets/images/suppluwok-system-context.png)

### 4.6.3. Software Architecture Container Diagrams.

![](../assets/images/supplywok-containers.png)

### 4.6.4. Software Architecture Components Diagrams.

![](../assets/images/supplywok-components.png)

## 4.7. Software Object-Oriented Design.
### 4.7.1. Class Diagrams.

En esta seccion se presentara y se explicara el diagrama de clases por cada Boundes Context

![](../assets/images/IMBC.png)

El **Inventory Management Bounded Context** es el encargado de gestionar los recursos de inventario de cada restaurante, incluyendo el control de stock, niveles mínimos y movimientos de entrada y salida.

El **InventoryService** actúa como capa de aplicación, coordinando las operaciones del sistema. Este servicio utiliza el **InventoryRepository** para la persistencia de datos y el **InventoryItem** como entidad principal del dominio, encargada de representar cada insumo almacenado en el Inventario del restaurante.El **StockMovement** representa las modificaciones realizadas al stock de cada ítem, permitiendo llevar un registro detallado de entradas, salidas y ajustes.

![](../assets/images/S&PBC.png)

El **Supply and Purchasing Bounded Context** es el encargado de gestionar las órdenes de compra realizadas por cada restaurante, incluyendo el registro, cancelación y seguimiento de los pedidos.

El **PurchaseOrderService** actúa como capa de aplicación, coordinando las operaciones del sistema. Este servicio utiliza el **PurchaseOrderRepository** para la persistencia de datos y el **PurchaseOrder** como entidad principal del dominio, encargada de representar toda la información de una orden de compra de insumos del restaurante. Además, el **OrderItem** encapsula las especificaciones de cada producto dentro de la orden, como la cantidad solicitada y el precio unitario, permitiendo un control detallado de cada pedido.

![](../assets/images/O&IBC.png)

El **Operational Monitoring and IoT Alerts Bounded Context** es el encargado de gestionar la información recopilada por los sensores del restaurante, así como la configuración y generación de alertas ante condiciones fuera de los rangos establecidos.

El **SensorService** actúa como capa de aplicación, coordinando las operaciones del sistema. Este servicio utiliza los repositorios **IAlertRepository** y **ISensorRepository** para la persistencia de datos.

Además, emplea la entidad **Sensor**, junto con **SensorReading**, para representar la información capturada por los sensores. Por otro lado, la entidad **Alert** modela las alertas generadas cuando una medición supera los límites configurados.

![](../assets/images/RMBC.png)

El **Restaurant Management Bounded Context** es el encargado de gestionar todo lo relacionado con la operación del establecimiento, incluyendo la administración de mesas y la gestión de comandas en cada restaurante.

Los servicios **ComandaService**, **RestaurantService** y **TableService** actúan como capa de aplicación, coordinando las distintas operaciones del sistema. Estos servicios utilizan los repositorios **ComandaRepository**, **IRestaurantRepository** y **TableRepository** respectivamente para la persistencia de datos.

Además, se emplean las entidades **Table**, que representa una mesa dentro del restaurante; **Comanda** y **ComandaItem**, que modelan las órdenes de consumo; y **Restaurant**, que encapsula la información principal de cada restaurante.

![](../assets/images/S&OBC.png)

El **Supplier Management & Operations Bounded Context** es el encargado de gestionar la información de los proveedores, sus catálogos de productos y las operaciones relacionadas con el cumplimiento de pedidos.

Los servicios **SupplierService**, **SupplierCatalogService**, **DemandForecastService** y **OrderFulfillmentService** actúan como capa de aplicación, coordinando las distintas operaciones del sistema dentro de este contexto.

El **SupplierService** gestiona la información de los proveedores utilizando el repositorio **SupplierRepository**. Por su parte, el **SupplierCatalogService** administra los productos ofrecidos por cada proveedor mediante **SupplierCatalog** y **CatalogItem**, utilizando **SupplierCatalogRepository** para la persistencia.

Además, el **DemandForecastService** se encarga de generar proyecciones de demanda a través de la entidad **DemandForecast**, la cual contiene múltiples **ProductDemand** que representan estimaciones de consumo.

Finalmente, el **OrderFulfillmentService** gestiona el proceso de entrega de pedidos mediante la entidad **OrderFulfillment**, permitiendo hacer seguimiento al estado de los envíos desde su despacho hasta su entrega final.

![](../assets/images/I&ABC.png)

El **Identity & Access Bounded Context** es el encargado de gestionar todo lo relacionado con la autenticación y administración de cuentas de usuario en el sistema.

Los servicios **AuthService** y **TokenService** actúan como capa de aplicación, coordinando las operaciones de autenticación. El **AuthService** utiliza el repositorio UserRepository para la persistencia de datos, mientras que **TokenService** se encarga de la generación y validación de tokens de acceso.

La entidad **User** encapsula toda la información relevante de un usuario en la plataforma, como su correo electrónico, contraseña (almacenada de forma segura) y su **Role**, el cual define sus permisos dentro del sistema.

![](../assets/images/SBC.png)

El **Shared Bounded Context** contiene Value Objects comunes que son reutilizados por múltiples bounded contexts del sistema, evitando duplicación y promoviendo consistencia en el modelo.

El **ContactInfo** encapsula la información de contacto relevante, como teléfono, correo electrónico y sitio web. Este value object es utilizado por entidades como **Supplier** y **Restaurant**. Por otro lado, **Address** encapsula la información de dirección necesaria, siendo utilizado también por entidades como **Supplier** y **Restaurant** para representar ubicaciones físicas de manera estructurada.

## 4.8. Database Design.

El siguiente Diagrama Entidad-Relación detalla la estructura de datos fundamental que soporta la lógica de la plataforma. A este modelo, compuesto por 25 entidades, se le aplicaron las tres fases de normalización para garantizar un diseño robusto y eficiente. Esto asegura la escalabilidad, la separación de responsabilidades y el mantenimiento de la aplicación, organizada en los siguientes seis módulos:

- #### Gestión de Inventario

Controla las entradas, salidas y niveles de stock para evitar desabastecimientos o excesos.

- #### Abastecimiento y Órdenes de Compra

Gestiona los pedidos de insumos entre el restaurante y el proveedor, reduciendo los tiempos de respuesta entre ambos.

- #### Panel del Proveedor

Centraliza la funcionalidad del proveedor, permitiendo una mejor gestión de catálogos y pedidos.

- #### Plataforma y Acceso

Administra el acceso seguro de los usuarios, sus cuentas y planes de suscripción.

- #### Monitoreo Operativo y Alertas IoT

Representa el núcleo operativo del sistema; controla sensores y notificaciones para garantizar la seguridad en el entorno de trabajo.

- #### Comandas y Órdenes para Cocina

Facilita la comunicación eficiente entre la cocina y las mesas para garantizar un servicio rápido y sin errores.


### 4.8.1. Database Diagrams.

![](../assets/images/database-diagram.png)

[^1]: Clec. (s.f.). El color rojo en China: orígenes y tradiciones. Recuperado el 23 de abril de 2026, de https://fundacionclec.org/el-color-rojo-en-china-origenes-y-tradiciones/