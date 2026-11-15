Decisiones.md
markdown
Decisiones del Proyecto: Nora Fotografía Felina

# Decisiones del Proyecto: Nora Fotografía Felina

## 1. Plugins

| Plugin | Funcionalidad que resuelve | Tipo y versión gratis | Compatible ("Probado hasta") | ¿Funciona con tema propio? | Enlace en WordPress.org |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Yoast SEO** | Optimización para motores de búsqueda y visibilidad web. | Gratis (Versión 28.8, incluye análisis de contenido y mapas de sitio) | WordPress 6.x | Sí | [Ver en WordPress.org](https://wordpress.org/plugins/wordpress-seo/) |
| **Forminator** | Gestión de formularios de contacto interactivos y reservas. | Gratis (Versión 1.58.4, creación de formularios y lógica condicional) | WordPress 6.x | Sí | [Ver en WordPress.org](https://wordpress.org/plugins/forminator/) |
| **Smush** | Optimización y compresión automática de imágenes de los felinos. | Gratis (Versión 4.3.6, compresión masiva sin pérdida de calidad) | WordPress 6.x | Sí | [Ver en WordPress.org](https://wordpress.org/plugins/wp-smushit/) |
| **WP Mail SMTP** | Envío confiable de correos electrónicos y notificaciones del sitio. | Gratis (Versión 4.10.3, conexión con servicios de correo) | WordPress 6.x | Sí | [Ver en WordPress.org](https://wordpress.org/plugins/wp-mail-smtp/) |
| **Anti-Spam by CleanTalk** | Protección y filtrado automático contra spam en comentarios y registros. | Gratis (Versión 6.91, protección integral sin captcha molesto) | WordPress 6.x | Sí | [Ver en WordPress.org](https://wordpress.org/plugins/anti-spam-by-cleantalk/) |

---

## 2. Páginas de la fase 1

### Páginas seleccionadas para la Fase 1:
1. **Inicio:** Es la carta de presentación del emprendimiento, muestra la propuesta de valor y los accesos principales. 
2. **Contacto:** Permite a los tutores de los gatos enviar solicitudes de reserva o consultas directas mediante Forminator. 
3. **Nosotros:** Cuenta la historia de cómo nació el proyecto inspirándose en Nora y el vínculo con los felinos.
4. **Servicios:** Detalla los planes fotográficos disponibles (como "Esencia Felina" y "Clan Felino") y su metodología sin estrés.
5. **Blog:** Espacio para compartir las vivencias, historias de rescate y el inicio del proyecto con nuestra musa Nora.

### Páginas que quedan para fases posteriores:
- Tienda online de cuadros y enmarques físicos (carrito de compras y pasarela de pagos con WP EasyCart).
- Panel de usuario / Mi Cuenta para clientes registrados.

---

## 3. Plan del Tema

- **Nombre del tema:** `nora-fotografia-felina`
- **Tipo de tema:** Custom (propio), desarrollado a medida para reflejar la identidad visual y la calidez del emprendimiento centrado en mascotas.

### Carta Gantt (Etapas del Proyecto)

| Etapa / Actividad | Fecha de Inicio | Fecha de Término | Estado / Checkpoint |
| :--- | :--- | :--- | :--- |
| Identidad visual y estilos base | 05 Nov 2026 | 09 Nov 2026 | Por iniciar |
| Desarrollo de página Inicio y Blog | 10 Nov 2026 | 14 Nov 2026 | Por iniciar |
| Creación de páginas (Nosotros, Servicios, Contacto) | 15 Nov 2026 | 17 Nov 2026 | Por iniciar |
| **Checkpoint y revisión de avances** | **18 Nov 2026** | **18 Nov 2026** | 🔍 **Hito clave** |
| Configuración de plugins y ajustes finales | 19 Nov 2026 | 24 Nov 2026 | Por iniciar |
| **Entrega final del proyecto** | **25 Nov 2026** | **25 Nov 2026** | 🚀 **Entrega oficial** |

---

## 4. Plan B (Riesgos y Mitigaciones)

| Riesgo detectado | Acción de resolución (Mitigación) | Cuándo se activa (Señal o Fecha) |
| :--- | :--- | :--- |
| **El tema propio presenta errores de código o no carga bien.** | Se revierte al último commit funcional en Git o se cambia temporalmente a un tema descargado (ej. Astra) para cumplir con la estructura. | Si el diseño no levanta correctamente al 11 de noviembre. |
| **Un plugin de optimización o formularios genera conflictos internos.** | Se desactiva inmediatamente el plugin afectado y se reemplaza por la alternativa secundaria evaluada (ej. WPForms). | Al momento de realizar las pruebas de integración de plugins. |
| **Problemas de rendimiento o caída del servidor gratuito (InfinityFree).** | Se espera unos minutos de margen; si persiste, se traslada el flujo temporalmente de trabajo local a Local WP para continuar el desarrollo. | Si el error del servidor se extiende por más de 1 hora continua. |

## Estado del sitio en producción (Formativa 08: Checkpoint)

* **URL en producción:** http://caroline207.ct.ws
* **Tema activo:** Twenty Twenty-Five (tema oficial de WordPress basado en bloques)
* **Páginas publicadas en el menú:** Inicio, Blog, Nosotros y Contactame (con texto propio y datos directos de contacto)
* **Entradas de blog publicadas:** 3 entradas con texto propio y fotografías reales de Nora (*«El comienzo»*, *«La Nora»* y *«Fotografías Felinas musa Nora»*)

---

## Cambios respecto de la Sumativa 2

### Qué se mantuvo
* **Identidad visual y concepto:** Se conservó el enfoque del emprendimiento *Nora Fotografía Felina*, la paleta de colores cálidos y verde salvia, las tipografías legibles y el contenido visual protagonizado por Nora.
* **Estructura de contenido base:** Se mantuvieron las páginas esenciales de la Fase 1 (incluyendo Inicio, Nosotros, Blog y Contactame) y las 3 entradas de blog con relatos reales.
* **Alcance por etapas:** Se mantuvo la decisión de dejar la tienda y los pagos en línea fuera de esta fase de lanzamiento inicial.

### Qué se cambió y por qué
* **Cambio de tema (de tema propio / Cat Walking a Twenty Twenty-Five):** Inicialmente se planificó desarrollar un tema propio y luego se probó el tema descargado *Cat Walking*. Sin embargo, *Cat Walking* arrastraba contenido de demostración ajeno al rubro (fotos de perros, textos de relleno en latín y shortcodes rotos de tienda), por lo que se decidió migrar al tema oficial **Twenty Twenty-Five**. Este cambio permitió construir un diseño limpio mediante bloques, sin errores de carga en InfinityFree y fiel a la identidad de la marca.
* **Página de Contacto directa (sin formulario incrustado aún):** Aunque se instaló el plugin Forminator, para este checkpoint se optó por publicar la página *Contactame* con texto propio, horarios y canales directos (correo electrónico e Instagram) para asegurar estabilidad y claridad antes de integrar formularios avanzados.

---

## Decisión: Pivotear y continuar con Twenty Twenty-Five

* **Decisión tomada:** Se activa el **Plan B (pivotear a un tema oficial/descargado)** utilizando **Twenty Twenty-Five** como tema definitivo en producción.
* **Justificación y evidencia:** 
  * Durante las pruebas previas con *Cat Walking* se detectaron conflictos visuales y restos de plantilla difíciles de depurar en el plazo del checkpoint (como shortcodes `[ec_store]` y contenido de demostración).
  * Con **Twenty Twenty-Five**, el sitio carga sin errores en producción, cumple con todas las páginas y entradas exigidas para el checkpoint y ofrece una base sólida para avanzar hacia la entrega final.
  * 
