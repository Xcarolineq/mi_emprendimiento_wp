# Plan de continuidad - Etapa 2 de mi sitio

**Emprendimiento:** Nora Fotografía Felina
**Sitio de la etapa 1:** http://caroline207.ct.ws
**Fecha:** 22 de noviembre de 2026

## 1. Qué quedó fuera de la etapa 1 y por qué (3 pts)

Lista las funcionalidades que quisiste hacer y no pudiste. Para cada una, la razón.

| Funcionalidad | Por qué quedó fuera (tiempo, recursos, costo, conocimientos) | Qué aporta a mi emprendimiento |
| :--- | :--- | :--- |
| **Tienda online de cuadros y marcos físicos con WP EasyCart** | **Tiempo y recursos:** Configurar un carrito de compras con variaciones de tamaños y marcos requería mayor tiempo de desarrollo y un servidor con más memoria y almacenamiento que el hosting gratuito InfinityFree. | Permite monetizar el emprendimiento vendiendo cuadros impresos y enmarcados directamente desde la web sin depender solo de cotizaciones manuales. |
| **Panel de usuario / Mi Cuenta para clientes registrados** | **Tiempo y conocimientos:** Implementar un área privada segura donde cada cliente inicie sesión para revisar y seleccionar las pruebas fotográficas de su gato requería configurar permisos de roles y protección de rutas. | Mejora la experiencia de los tutores de gatos al permitirles ver, elegir sus fotos favoritas y descargar sus galerías desde un espacio personalizado. |
| **Página de Servicios detallada con reserva y pago directo** | **Costo y requisitos técnicos:** Automatizar la contratación de los planes fotográficos (*"Esencia Felina"* y *"Clan Felino"*) con cobro en línea exige contratar un hosting pago con certificado SSL activo (HTTPS) y trámites previos de pasarela de pagos. | Agiliza la contratación de sesiones a domicilio, permitiendo cobrar un abono inicial para asegurar la reserva de fecha y reducir cancelaciones. |
| **Tema propio a medida (`nora-fotografia-felina`)** | **Tiempo:** Para asegurar estabilidad y cumplir con los plazos de la entrega sin errores de código, se decidió pivotear al tema oficial **Twenty Twenty-Five** en la etapa 1. | Permitiría a futuro contar con una identidad visual 100% personalizada y libre de estilos genéricos si se retoma el desarrollo del tema propio. |

## 2. Recursos que necesito (2 pts)

| Funcionalidad | Plugin o herramienta | Gratis o de pago | Costo aproximado | Qué tendría que aprender |
| :--- | :--- | :--- | :--- | :--- |
| **Tienda online de cuadros y marcos** | WP EasyCart (o WooCommerce) | Freemium (versión gratuita base o Pro de pago) | $0 USD (versión Free) / ~$69 USD al año (Pro) | Creación de catálogo de productos físicos, opciones de enmarcado, cálculo de envíos y gestión de pedidos. |
| **Panel de usuario / Mi Cuenta** | Ultimate Member o WP EasyCart (cuentas de cliente) | Freemium | $0 USD (versión básica gratuita) | Configuración de formularios de registro/inicio de sesión, perfiles de usuario y restricción de páginas privadas. |
| **Pasarela de pagos para planes y cuadros** | MercadoPago o Transbank Webpay | Gratis (el plugin) | ~2.9% a 3.5% de comisión por transacción | Configuración de claves API (modo prueba y producción) y gestión de abonos para los planes *"Esencia Felina"* y *"Clan Felino"*. |
| **Agendamiento de sesiones sin estrés** | Simply Schedule Appointments | Freemium | $0 USD (versión gratuita) / ~$99 USD al año (Plus) | Configuración de disponibilidad horaria, tiempos de traslado a domicilio y sincronización con Google Calendar. |

**Servidor:** Para la etapa 2 necesitaré migrar desde el hosting gratuito actual (`InfinityFree / ct.ws`) hacia un **hosting WordPress pago** (como Hosting.cl, EcoHosting o SiteGround) con dominio propio (ej. `norafotografiafelina.cl`). Requerirá **mínimo 10 GB de almacenamiento SSD/NVMe** (indispensable para alojar fotografías felinas en alta resolución y galerías de clientes), **PHP 8.0 o superior**, base de datos **MySQL / MariaDB**, **certificado SSL gratuito (HTTPS)** obligatorio para habilitar pagos en línea, y puertos **SMTP abiertos** para asegurar el envío de notificaciones.

## 3. Priorización y cronograma (2 pts)

Ordena lo que harías primero y en cuánto tiempo. Puedes usar una tabla o un diagrama Gantt.

| Prioridad | Qué hago | Cuándo (mes o semana) | Resultado esperado |
| :--- | :--- | :--- | :--- |
| **1 (Crítica)** | Migración desde InfinityFree a hosting pago, adquisición de dominio propio y activación de certificado SSL (HTTPS). | Semana 1 (Mes 1) | Sitio web estable sin caídas ni límites de recursos, con candado de seguridad SSL activo y envío de correos funcionando correctamente. |
| **2 (Alta)** | Creación y publicación de la página **Servicios** detallando los planes *"Esencia Felina"* y *"Clan Felino"* con formulario de reserva. | Semana 2 (Mes 1) | Los tutores de gatos pueden conocer en detalle las tarifas, duración y metodología sin estrés de cada plan fotográfico. |
| **3 (Media)** | Instalación y configuración de **WP EasyCart** para habilitar la tienda online de cuadros y marcos físicos + pasarela de pagos. | Semanas 3 y 4 (Mes 1) | Tienda operativa donde los clientes seleccionan el tamaño y marco de su cuadro y pagan en línea de forma segura. |
| **4 (Evolutiva)** | Implementación del **Panel de usuario / Mi Cuenta** para clientes registrados y prueba completa del flujo de selección de fotos. | Semanas 1 y 2 (Mes 2) | Los clientes registrados acceden con su cuenta para revisar el estado de sus pedidos y visualizar las pruebas de su sesión. |

## 4. Riesgos y mitigación (1 pt)

| Riesgo | Qué haría | Cuándo se activa |
| :--- | :--- | :--- |
| **Caídas del servidor o lentitud por fotografías de alta resolución** | Mantener activo el plugin **Smush** para comprimir imágenes sin pérdida de calidad, convertir las fotos a formato **WebP** antes de subirlas y completar la migración fuera de InfinityFree. | Cuando el tiempo de carga supere los 3 segundos o el servidor gratuito presente intermitencias de conexión. |
| **Conflictos visuales o errores al activar WP EasyCart con Twenty Twenty-Five** | Realizar un respaldo completo `.wpress` con **All-in-One WP Migration** y probar la tienda primero en un entorno local (**LocalWP**) antes de activarla en producción. | Si al instalar el plugin de tienda se desconfiguran los bloques, shortcodes o el diseño general del tema **Twenty Twenty-Five**. |
| **El costo de licencias Pro (WP EasyCart / reservas) supera el presupuesto inicial** | Utilizar únicamente las versiones gratuitas funcionales en una primera fase (pagos mediante transferencia bancaria directa y reservas vía **Forminator**) hasta reunir ingresos suficientes. | Si los costos fijos mensuales o anuales en dólares no alcanzan a cubrirse con las primeras ventas de sesiones y cuadros. |
| **Bloqueo en el envío de correos de confirmación de pedidos o registro de usuarios** | Configurar **WP Mail SMTP** conectado mediante API a un servicio transaccional dedicado (**Brevo** gratuito) en lugar de usar el correo nativo del servidor. | Cuando los usuarios no reciban los correos de recuperación de contraseña de su cuenta o los comprobantes de compra. |
