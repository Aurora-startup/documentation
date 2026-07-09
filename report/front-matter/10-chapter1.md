<div style="page-break-before: always;"></div>

# Capítulo I: Introducción
## 1.1. Startup Profile 
### 1.1.1. Descripción de la Startup 
Somos Aurora, un grupo de estudiantes apasionados por la innovación tecnológica de la Universidad Peruana de Ciencias Aplicadas. Nuestra startup está enfocada en optimizar la gestión operativa y de abastecimiento en restaurantes tipo chifa mediante soluciones tecnológicas inteligentes. Nuestra plataforma conecta a restaurantes y proveedores a través de un sistema centralizado que permite gestionar inventarios, preveenir accidentes, anticipar la demanda y mejorar la coordinación en la cadena de suministro.

- **Misión:** Nuestra misión es mejorar la eficiencia operativa de los restaurantes mediante herramientas tecnológicas que permitan gestionar inventarios, anticipar necesidades de abastecimiento y optimizar la coordinación con proveedores, contribuyendo a una gestión más inteligente y sostenible del negocio gastronómico.

- **Visión:** Convertirnos en una plataforma líder en la digitalización de operaciones para restaurantes en Latinoamérica, facilitando la toma de decisiones basada en datos y fortaleciendo la integración entre restaurantes y proveedores.

- **Valores:**
    - **Eficiencia**: Buscamos optimizar procesos clave para reducir pérdidas y mejorar la operación diaria.
    - **Innovación**: Aplicamos tecnología y análisis de datos para resolver problemas reales del sector gastronómico.
    - **Confiabilidad**: Proporcionamos información precisa y útil para la toma de decisiones.
    - **Escalabilidad**: Diseñamos soluciones adaptables a distintos tamaños de negocio.
    - **Colaboración**: Facilitamos la interacción entre restaurantes y proveedores para mejorar resultados conjuntos.

### 1.1.2. Perfiles de integrantes del equipo 


| Integrante | Descripción | Foto |
|------------|------------|------|
| **Nombre:** Marcelo Fabio Cuadros Villanueva<br>**Carrera:** Ingeniería de Software<br>**Código:** U202422890 | **Descripción breve de sus habilidades:** <br> Soy Marcelo Cuadros, estudiante de Ingeniería de Software en la UPC actualmente cursando mi cuarto ciclo academico. Me considero una persona proactiva, sociable y con gran capacidad de trabajo en equipo; con conocimientos en c++, python, java, html, css y javascript.| <img src="../assets/images/members/marcelo.png" width="500" /> |
|**Nombre:** Zayd Jaffar Ayasta Martel<br>**Carrera:** Ingeniería de Software<br>**Código:** U202410837          | **Descripción breve de sus habilidades:** <br>Soy Zayd Ayasta, estudiante de Ingeniería de Software con conocimientos en C++, SQL, Java y Kotlin. Me caracterizo por ser creativo y adaptable, con interés en la innovación tecnológica y el desarrollo de soluciones que aporten valor real a los usuarios.               | <img src="../assets/images/members/zayd.jpg" alt="Zayd-logo" width="500" />|
| **Nombre:** Alexandra Yamile Meza Soza<br>**Carrera:** Ingeniería de Software<br>**Código:** U20241b451 | **Descripción breve de sus habilidades:** <br> Soy Alexandra Meza, estudiante de Ingenieria de Software en la UPC, me gustaría aportar a este proyecto con mis conocimientos en programación en los lenguajes C++, Python, HTML y CSS. Asimismo, puedo contribuir al equipo con habilidades en trabajo colaborativo, organización y resolución de problemas. | <img src="../assets/images/members/alexandra.png" width="500" /> |
| **Nombre:** Juan Sung Jau Wang Chen<br>**Carrera:** Ingeniería de Software<br>**Código:** U202318609 | **Descripción breve de sus habilidades:**<br> Soy Juan Wang, estudiante de Ingeniería de Software en la UPC. Me considero alguien amigable y sociable, puedo adaptarme sin problemas a cualquier entorno, tengo experiencia en organizacion de equipos y conocimientos de c++, python, html, css y javascript. | <img src="../assets/images/members/juan.png" width="500px"> |
| **Nombre:** Joan Fabricio Payano Puchuri<br>**Carrera:** Ingeniería de Software<br>**Código:** U202318620 | **Descripción breve de sus habilidades:** <br> Soy Joan Payano, estudiante de Ingeniería de Software en la UPC. En mis tiempos libres me gusta salir con amigos o familiares, aunque también me gusta escuchar musica y cocinar, actualmente cuento con conocimientos breves de los lenguajes de programación C++, Python, Javascript, HTML y CSS.| <img src="../assets/images/members/joan.png" width="500" /> |

<sub>*Tabla 1. Perfiles de integrantes de equipo*</sub>

## 1.2. Solution Profile 
### 1.2.1.  Antecedentes y problemática
Los restaurantes tipo chifa enfrentan dificultades en la gestión eficiente de sus inventarios y en la planificación de abastecimiento debido a la falta de herramientas tecnológicas que integren información operativa en tiempo real. Esta situación genera pérdidas económicas por sobrestock o desabastecimiento, decisiones basadas en estimaciones imprecisas y una coordinación ineficiente con proveedores. Asimismo, los proveedores carecen de visibilidad sobre la demanda real de sus clientes, lo que dificulta la planificación de producción y distribución. Existe la necesidad de una solución que permita centralizar la gestión de inventarios, analizar datos operativos y facilitar la coordinación entre restaurantes y proveedores, mejorando así la eficiencia y reduciendo la incertidumbre en la toma de decisiones.

<h4>5W + 2H</h4>

- **¿Qué ocurre? (WHAT)**
    Los restaurantes tipo chifa y sus proveedores enfrentan limitaciones en la gestión integrada de sus procesos operativos y de abastecimiento. Esto se refleja en problemas como control deficiente de inventarios, poca visibilidad del estado de mesas y comandas, riesgos en cocina, pérdidas por almacenamiento inadecuado y dificultad para anticipar la demanda. Según INACAL (2023)[^1], los restaurantes deben asegurar controles de recepción, inocuidad, seguridad e infraestructura, pero muchos procesos siguen ejecutándose de forma manual o fragmentada. Además, la digitalización de la cadena de suministro alimentaria todavía presenta brechas de coordinación e intercambio de información entre actores, lo que limita la eficiencia y la reducción de desperdicios (Annosi et al., 2021)[^2].

- **¿Quiénes se ven afectados? (WHO)**
    El problema afecta principalmente a los dueños y administradores de restaurantes chifa, quienes deben controlar cocina, salón, almacén y compras con recursos limitados. También impacta a los proveedores de insumos, ya que la falta de información oportuna sobre consumo, rotación y demanda reduce la precisión del abastecimiento y dificulta la planificación conjunta (Annosi et al., 2021)[^2]. De manera complementaria, los trabajadores de cocina resultan afectados por la exposición a accidentes y enfermedades laborales en entornos de trabajo intensivos, donde la prevención muchas veces no está soportada por sistemas de monitoreo continuo (Wassif et al., 2024)[^3].

- **¿Dónde ocurre? (WHERE)**
    Este problema se presenta en restaurantes y servicios de alimentación, especialmente en negocios con alta rotación de insumos perecibles y múltiples procesos simultáneos, como los chifas. En el contexto peruano, la problemática resulta relevante por el crecimiento sostenido del rubro restaurantes, donde el INEI (2024)[^4] reporta expansión del sector e incluye explícitamente a los chifas dentro de los negocios con desempeño positivo. Además, las exigencias de calidad e inocuidad planteadas por INACAL (2023)[^1] muestran que el reto no solo está en vender más, sino en operar mejor y con mayor seguridad.

- **¿Cuándo ocurre? (WHEN)**
    El problema es permanente, pero se intensifica en horas pico, campañas comerciales, fines de semana, feriados y temporadas de alta demanda, cuando aumentan simultáneamente los pedidos, la presión sobre cocina, el consumo de insumos y la necesidad de reposición rápida. Tanizaki et al. (2020)[^5] señalan que la gestión del restaurante mejora cuando el pronóstico de demanda incorpora datos internos y externos, precisamente porque la variabilidad del consumo afecta decisiones críticas como compras, personal e inventario.

- **¿Por qué es importante resolverlo? (WHY)**
    Resolver este problema es clave porque impacta directamente en la eficiencia operativa, la seguridad del personal, la calidad del servicio y la relación con los proveedores. La adopción de soluciones digitales e IoT puede fortalecer la trazabilidad, la supervisión de variables críticas como temperatura y almacenamiento, y la respuesta oportuna ante fallas o riesgos operativos (Bouzembrak et al., 2019)[^6]. Además, una mejor coordinación digital en la cadena de suministro permite reducir desperdicios, mejorar el flujo de información y sostener relaciones más eficientes entre restaurantes y proveedores (Annosi et al., 2021)[^2].

- **¿Cómo se manifiesta? (HOW)**
    El problema se evidencia en quiebres o excesos de stock, demora en comandas, poca trazabilidad de insumos, limitada visibilidad de la ocupación de mesas,v fallas en el control del almacén y exposición constante a riesgos en cocina. También se manifiesta en pedidos mal planificados a proveedores y en decisiones reactivas basadas en experiencia más que en datos. Wassif et al. (2024)[^3] muestran que el entorno de cocina puede concentrar altas tasas de lesiones y enfermedades ocupacionales, mientras que Bouzembrak et al. (2019)[^6] destacan que sensores IoT permiten monitorear temperatura, humedad y trazabilidad en procesos alimentarios, justamente para atender estas brechas operativas.

- **¿Cuánto impacta? (HOW MUCH)**
    El impacto es operativo, económico y humano. En términos sectoriales, el INEI (2024)[^4] reportó que la actividad de restaurantes en Perú creció 2,57% en febrero de 2024, reflejando un entorno competitivo donde la eficiencia del servicio y del abastecimiento se vuelve más importante. En el plano ocupacional, Wassif et al. (2024)[^3] encontraron prevalencias de 77,3% en lesiones laborales y 81,3% en enfermedades relacionadas con el trabajo entre personal de cocina estudiado, lo que confirma la relevancia de la prevención. En el plano logístico, Tanizaki et al. (2020)[^5] sostienen que el pronóstico de demanda mejora decisiones de pedidos e inventarios, mientras que Annosi et al. (2021)[^2] destacan que la digitalización favorece la colaboración y la reducción de desperdicios a lo largo de la cadena alimentaria. En conjunto, esto demuestra que la ausencia de una plataforma integrada genera pérdidas por ineficiencia, riesgos para el personal y menor capacidad de coordinación entre restaurante y proveedor.


### 1.2.2 Lean UX Process   

#### 1.2.2.1 Lean UX Problem Statement
El estado actual de la gestión operativa y de abastecimiento en restaurantes tipo chifa se ha centrado principalmente en controles manuales, registros dispersos, decisiones reactivas sobre inventario y coordinación informal con proveedores. 

Lo que los productos y servicios existentes no logran atender es la necesidad de una solución integrada que combine control de inventario, alertas operativas, proyección de demanda, coordinación digital de pedidos y monitoreo operativo en un solo entorno. 

Nuestro producto abordará esta brecha mediante una plataforma web que conecte restaurantes y proveedores para centralizar inventario, alertas, pedidos, proyecciones de demanda y monitoreo operativo. 

Nuestro enfoque inicial estará dirigido a dueños y administradores de restaurantes chifa, incorporando progresivamente a proveedores clave para validar la coordinación de abastecimiento. 

Sabremos que vamos en la dirección correcta cuando los usuarios objetivo gestionen su inventario con mayor consistencia, anticipen antes sus necesidades de compra y coordinen pedidos de abastecimiento con menor incertidumbre y menos decisiones reactivas.


#### 1.2.2.2 Lean UX Assumptions

**Usuarios objetivo**
- Asumimos que los dueños y administradores de restaurantes chifa necesitan una forma más simple y centralizada de controlar inventario, evitar pérdidas y reaccionar a tiempo ante problemas operativos.
- Asumimos que los proveedores de insumos necesitan mayor visibilidad sobre la demanda de sus clientes para planificar pedidos, rutas y entregas con menor incertidumbre.
- Asumimos que ambos segmentos estarán dispuestos a adoptar una plataforma compartida si esta reduce trabajo manual, mejora la coordinación y ofrece beneficios claros en su operación diaria.

**Objetivos de los usuarios**
- Asumimos que los restaurantes valorarán poder registrar inventario, configurar alertas y visualizar su operación en tiempo real desde una sola plataforma.
- Asumimos que los proveedores valorarán contar con información de demanda estimada, estado de pedidos y herramientas para organizar sus entregas.
- Asumimos que ambos segmentos preferirán información clara, actualizada y fácil de interpretar antes que procesos manuales o dispersos.

**Business Outcomes**
- Asumimos que una plataforma que unifique inventario, pedidos, alertas y monitoreo operativo puede mejorar la eficiencia de los restaurantes.
- Asumimos que una mejor coordinación digital entre restaurantes y proveedores puede reducir retrasos, desabastecimientos y compras de emergencia.
- Asumimos que la reducción de desperdicio y de fallas operativas generará valor económico suficiente para que los usuarios perciban utilidad real en el producto.
- Asumimos que un modelo de suscripción con planes diferenciados puede sostener el producto en el tiempo si los usuarios perciben beneficios concretos.

**Solution Assumptions**
- Asumimos que el registro de inventario y las alertas de stock mínimo serán funcionalidades prioritarias para la adopción inicial del producto.
- Asumimos que una proyección básica de demanda será suficiente para ayudar a los restaurantes a anticipar compras en una primera etapa.
- Asumimos que el monitoreo de variables operativas como la temperatura aportará valor al permitir detectar riesgos antes de que afecten la calidad de los insumos.
- Asumimos que la integración de restaurantes y proveedores en una misma plataforma generará una mejor coordinación que el uso de canales informales.


#### 1.2.2.3 Lean UX Hypothesis Statements
- Creemos que la reducción de desabastecimientos y la mejora del control operativo se logrará si los dueños y administradores de restaurantes chifa obtienen visibilidad centralizada de sus insumos con la funcionalidad de registro de inventario.
- Creemos que la disminución de compras de emergencia y quiebres de stock se logrará si los dueños y administradores de restaurantes chifa obtienen alertas oportunas sobre niveles críticos de insumos con la funcionalidad de alertas de stock mínimo.
- Creemos que una toma de decisiones más rápida y mejor informada se logrará si los dueños y administradores de restaurantes chifa obtienen una vista clara del estado de sus insumos con la funcionalidad de dashboard de inventario.
- Creemos que una mejor planificación de compras y abastecimiento se logrará si los dueños y administradores de restaurantes chifa obtienen una estimación anticipada de consumo con la funcionalidad de proyección básica de demanda.
- Creemos que una coordinación más eficiente con proveedores se logrará si los dueños y administradores de restaurantes chifa obtienen un proceso más simple para solicitar abastecimiento con la funcionalidad de generación de órdenes de compra.
- Creemos que una mejor coordinación operativa entre restaurantes y proveedores se logrará si los dueños y administradores de restaurantes chifa obtienen visibilidad del estado de sus pedidos con la funcionalidad de seguimiento de órdenes de compra.
- Creemos que una relación de abastecimiento más ordenada y eficiente se logrará si los dueños y administradores de restaurantes chifa obtienen un directorio centralizado de sus proveedores con la funcionalidad de gestión de proveedores vinculados.
- Creemos que una mejor planificación de entregas y distribución se logrará si los proveedores de insumos obtienen mayor visibilidad de las necesidades futuras de sus clientes con la funcionalidad de visualización de demanda estimada.
- Creemos que una mejor coordinación comercial y menor fricción al generar pedidos se logrará si los proveedores de insumos obtienen una forma clara de mostrar precios, unidades y disponibilidad con la funcionalidad de gestión de catálogo de productos.
- Creemos que la reducción del riesgo operativo y de pérdidas de insumos se logrará si los dueños y administradores de restaurantes chifa obtienen alertas sobre condiciones críticas del entorno con la funcionalidad de monitoreo de temperatura.
- Creemos que una respuesta más rápida ante eventos críticos se logrará si los dueños y administradores de restaurantes chifa obtienen notificaciones visibles y accionables con la funcionalidad de alertas operativas.

#### 1.2.2.4 Lean UX Canvas

# Lean UX Canvas

| 1. Business Problem | 5. Solution Ideas | 2. Business Outcomes |
|--------------------|------------------|---------------------|
| - Estado actual del dominio: El estado actual de la gestión operativa y de abastecimiento en restaurantes tipo chifa se ha enfocado principalmente en controles manuales y procesos fragmentados realizados por dueños y encargados, con escasa digitalización. Esto provoca dificultades para mantener inventarios actualizados, falta de visibilidad sobre la demanda y una coordinación ineficiente con proveedores.<br><br>Lo que los productos/servicios existentes no resuelven: Los productos y servicios disponibles no abordan de forma integrada la combinación de inventario en tiempo real, proyección de demanda sencilla, generación automática de pedidos y monitoreo operativo (por ejemplo, temperatura), necesarios para que restaurantes y proveedores se sincronicen y tomen decisiones preventivas basadas en datos.<br><br>Cómo nuestra solución cerrará la brecha: Nuestra plataforma, SupplyWok, abordará esta brecha mediante una aplicación web con roles diferenciados para restaurantes y proveedores que centraliza inventario y alertas, ofrece proyecciones de demanda basadas en historial y ocupación, sugiere y genera pedidos automatizados, y reporta eventos operativos críticos (p. ej. temperatura fuera de rango) para facilitar decisiones oportunas y coordinación eficiente.<br><br>En qué nos enfocaremos inicialmente: Nuestro enfoque inicial será en dueños y administradores de restaurantes chifa, validando con ellos las funcionalidades esenciales de inventario, alertas y generación de pedidos; en paralelo incorporaremos proveedores clave para validar la vista de demanda y la coordinación de entregas.<br><br>Cómo sabremos que tuvimos éxito (comportamientos medibles):<br>≥ 60% de restaurantes activos configuran su inventario inicial y al menos una alerta durante el primer mes.<br>≥ 50% de los pedidos se originan a partir de sugerencias o alertas del sistema.<br>≥ 70% de los usuarios encuestados manifiestan que la plataforma mejora la coordinación operativa.<br>≥ 50% de proveedores activos consultan su panel de demanda al menos una vez por semana.<br>≥ 80% de los eventos de temperatura fuera de rango generan alertas visibles y accionables en el dashboard.| Los usuarios podrán ver en una sola pantalla lo más importante del día (pendientes, alertas, estado general) y entrar rápido a acciones frecuentes.<br>Los usuarios podrán identificar productos en riesgo (bajo mínimo) y tomar acción para reponer antes de quedarse sin stock.<br>El personal podrá crear órdenes con productos, cantidades y notas, y actualizarlas a medida que avanza el servicio.<br>Los usuarios podrán ver qué órdenes están pendientes, en progreso o finalizadas, para coordinar mejor entre áreas.<br>Los usuarios podrán armar pedidos de compra de forma guiada (qué comprar y en qué cantidad) para reabastecer con menos fricción. | Menos pérdidas por quiebre de stock y mejor rotación de inventario (comprar lo necesario a tiempo).<br>Mayor velocidad de operación (comandas y pedidos se registran/actualizan más rápido) y menos errores por registro manual.<br>Mejor coordinación entre roles (cocina, inventario, administración) con estados y pendientes visibles.<br>Visibilidad operacional para managers: KPIs básicos y backlog de pendientes/alertas para priorizar.<br>Escalabilidad: procesos repetibles para múltiples locales/equipos, con configuración (proveedores, zonas de servicio, notificaciones) mantenible. |
| **3. Users** | **7. Most Important Learning** | **4. User Outcomes & Benefits** |
| - Los usuarios son personal operativo de restaurante y back-office (p. ej. Chef, Inventory, Manager) que trabajan con tareas urgentes y contextos de alta rotación.<br>Necesitan ejecutar acciones con pocos clics y con baja carga cognitiva, porque alternan entre trabajo físico y pantalla.<br>Usan el sistema en distintos momentos del día y valoran acceso rápido a: comandas, stock, alertas, pedidos de compra y tablas/mesas.<br>Tienen necesidades distintas por rol (lo que “importa” en el dashboard y en los accesos varía según permisos/responsabilidades).<br>En algunos entornos habrá conectividad irregular, por lo que esperan que la app sea robusta ante errores (mensajes claros, reintentos, no perder datos del formulario).<br>Algunos usuarios requieren la interfaz en más de un idioma (hay selector de idioma), y esperan consistencia en textos y etiquetas. | - ¿Los usuarios realmente usarán el sistema como su herramienta principal para operar y decidir (“reaccionar”), o seguirán usando métodos alternativos fuera de la app?<br><br>Si esta suposición es falsa (si los usuarios no adoptan la app como su base de operación diaria), todo el valor prometido por nuestras features se pierde, sin importar cuán bien estén diseñadas o implementadas. | - Identificar rápidamente qué requiere atención (alertas/pendientes) desde un dashboard principal sin navegar por múltiples pantallas.<br>Reducir quiebres de stock detectando productos “por debajo del mínimo” y actuando (reposición/compra) antes de impactar la operación.<br>Crear/editar comandas u órdenes de cocina con seguridad (evitar errores de mesa/tipo de servicio/items/observaciones) y poder volver atrás sin fricción.<br>Generar pedidos de compra más rápido, con datos prellenados y validaciones (fechas, proveedor, prioridad, líneas de pedido).<br>Sentir control y trazabilidad: saber “qué pasó y qué sigue”, incluso cuando cambian estados (pendiente/en proceso/etc.).<br>Evitar duplicidad y errores manuales: que el sistema centralice inventario, órdenes y compras con información consistente. |
| **6. Hypotheses** |  | **8. Least Effort to Learn** |
| Creemos que una vista principal que priorice lo urgente ayudará a que el equipo actúe más rápido y con menos estrés, porque reduce la navegación y facilita decidir qué hacer primero.<br>Sabremos que funciona cuando baje el tiempo desde que ingresan hasta que completan la primera acción y aumente la atención de pendientes críticos.<br>Creemos que hacer visibles los faltantes y riesgos de inventario ayudará a prevenir quiebres de stock, porque convierte el control en una tarea simple y frecuente.<br>Sabremos que funciona cuando disminuyan los quiebres de stock y aumente la reposición anticipada.<br>Creemos que un flujo rápido y claro para registrar y actualizar órdenes ayudará a reducir errores y acelerar la operación, porque estandariza la información y evita omisiones.<br>Sabremos que funciona cuando bajen las correcciones por errores y disminuya el tiempo promedio para registrar una orden completa.<br>Creemos que dar visibilidad del estado de las órdenes ayudará a mejorar la coordinación y reducir retrabajo, porque todos saben qué está pasando sin tener que preguntar.<br>Sabremos que funciona cuando disminuyan interrupciones/consultas internas y se reduzca el tiempo de ciclo de las órdenes.<br>Creemos que guiar el armado de pedidos de compra ayudará a reponer inventario más rápido y con menos errores, porque reduce el trabajo manual y estandariza el proceso.<br>Sabremos que funciona cuando disminuya el tiempo para generar un pedido y bajen los pedidos incompletos o corregidos. |  | - El menor trabajo para validar la suposición más crítica es crear un prototipo navegable (o MVP básico) que simule la centralización de la operación. Hacer que usuarios reales lo usen para casos frecuentes y observar si lo adoptan o todavía prefieren métodos alternativos. Así podremos aprender rápidamente si nuestra solución cubre las necesidades y si realmente será usada como centro operativo.|

<sub>*Tabla 2. Lean UX Canvas*</sub>


## 1.3 Segmentos Objetivo

Con la investigación y el enfoque del producto, se identificaron 2 segmentos objetivos principales:

**- Segmento 1: Dueños de restaurantes chifa y administradores**

**Descripción:** Usuarios responsables de la operación diaria del restaurante, la compra de insumos, el control de stock y la supervisión de procesos internos. Su motivación principal es reducir pérdidas, mejorar la planificación y tener mayor control sobre la operación.

**Características generales:**
- **Ubicación:** Restaurantes urbanos y zonas con alta concentración de oferta gastronómica.
- **Rol:** Dueños, administradores o encargados de operación.
- **Necesidad principal:** Control de inventario, alertas, proyección de demanda y coordinación de pedidos.
- **Nivel tecnológico:** Uso frecuente de sistemas web o móviles para gestión básica del negocio.

**Información de sustento:**
- La mala proyección de demanda en foodservice se asocia con sobreproducción y desperdicio, mientras que mejorar el forecasting ayuda a reducir desperdicio y demanda insatisfecha.
- Los enfoques de IoT permiten monitorear temperatura, humedad y trazabilidad en entornos alimentarios, aportando control operativo y visibilidad.

**- Segmento 2: Proveedores de insumos para restaurantes**

**Descripción:** Usuarios que abastecen a uno o varios restaurantes y necesitan anticipar pedidos, organizar entregas y mantener una relación más eficiente con sus clientes. Su motivación principal es planificar mejor su distribución y contar con información útil para sus rutas y abastecimiento.

**Características generales:**
- **Ubicación:** Empresas o negocios de distribución de insumos alimentarios.
- **Rol:** Proveedores, distribuidores o encargados comerciales.
- **Necesidad principal:** Visibilidad de demanda, seguimiento de pedidos y planificación de entregas.
- **Nivel tecnológico:** Uso de plataformas digitales para pedidos, coordinación y seguimiento.

**Información de sustento:**
- La digitalización mejora la visibilidad y trazabilidad en cadenas alimentarias, lo que facilita la coordinación entre actores.
- Las soluciones basadas en datos permiten mejorar la planificación de la oferta y reducir errores de abastecimiento.


[^1]: Instituto Nacional de Calidad (INACAL). (2023). *Turismo: Inacal promueve la calidad en servicios de restaurantes*. https://www.gob.pe/institucion/inacal/noticias/809133-turismo-inacal-promueve-la-calidad-en-servicios-de-restaurantes

[^2]: Annosi, M. C., Brunetta, F., Bimbo, F., & Kostoula, M. (2021). Digitalization within food supply chains to prevent food waste: Drivers, barriers and collaboration practices. *Industrial Marketing Management, 93*, 208–220. https://doi.org/10.1016/j.indmarman.2021.01.005

[^3]: Wassif, G. O., Abdelsalam, A., Eldin, W. S., Abdel-Hamid, M. A., & Damaty, S. I. (2024). Work-related injuries and illnesses among kitchen workers at two major students’ hostels. *Journal of the Egyptian Public Health Association, 99*, Article 16. https://doi.org/10.1186/s42506-024-00163-x

[^4]: Instituto Nacional de Estadística e Informática (INEI). (2024). *Actividad de restaurantes aumentó en 2,57% en febrero de 2024*. https://m.inei.gob.pe/prensa/noticias/actividad-de-restaurantes-aumento-en-257-en-febrero-de-2024-15121/

[^5]: Tanizaki, T., Hoshino, T., Shimmura, T., & Takenaka, T. (2020). Restaurant store management based on demand forecasting. *Procedia CIRP, 88*, 580–583. https://doi.org/10.1016/j.procir.2020.05.101

[^6]: Bouzembrak, Y., Klüche, M., Gavai, A., & Marvin, H. J. P. (2019). Internet of things in food safety: Literature review and a bibliometric analysis. *Trends in Food Science & Technology, 94*, 54–64. https://doi.org/10.1016/j.tifs.2019.11.002
