Decisiones.md
markdown
Decisiones del Proyecto: Nora Fotografía Felina

1. Plugins

| Plugin | Funcionalidad que resuelve | Tipo y versión gratis | Compatible ("Probado hasta") | ¿Funciona con tema propio? | Enlace en WordPress.org |

| **Yoast SEO** | Optimización para motores de búsqueda y visibilidad del sitio en Google. | Gratis (Incluye análisis de contenido y meta descripciones) | WordPress 6.x | Sí | [Ver en WordPress.org](https://wordpress.org/plugins/wordpress-seo/) |
| **Forminator** | Gestión de formularios avanzados de contacto y reservas de sesiones. | Gratis (Creación de formularios personalizados y campos básicos) | WordPress 6.x | Sí | [Ver en WordPress.org](https://wordpress.org/plugins/forminator/) |
| **Anti-Spam by CleanTalk** | Protección y filtrado automático de spam en formularios y registros. | Gratis / Freemium (Protección básica antispam) | WordPress 6.x | Sí | [Ver en WordPress.org](https://wordpress.org/plugins/anti-spam-by-cleantalk/) |
| **All-in-One WP Migration** | Copias de seguridad, exportación y restauración segura del sitio web. | Gratis (Exportación e importación de archivos y base de datos) | WordPress 6.x | Sí | [Ver en WordPress.org](https://wordpress.org/plugins/all-in-one-wp-migration/) |
| **Smush** | Optimización y compresión automática de las imágenes de los felinos. | Gratis (Compresión masiva sin pérdida notable de calidad visual) | WordPress 6.x | Sí | [Ver en WordPress.org](https://wordpress.org/plugins/wp-smushit/) |

2. Páginas de la fase 1

 Páginas seleccionadas para la Fase 1:
1. Inicio: Es la carta de presentación del emprendimiento, muestra la propuesta de valor y los accesos principales. (Obligatoria)
2. Contacto: Permite a los tutores de los gatos enviar solicitudes de reserva o consultas directas. (Obligatoria)
3. Nosotros: Cuenta la historia de cómo nació el proyecto inspirándose en Nora y el vínculo con los felinos.
4. Servicios: Detalla los planes fotográficos disponibles (como "Esencia Felina" y "Clan Felino") y su metodología sin estrés.
5. Blog: Espacio para compartir las vivencias, historias de rescate y el inicio del proyecto con nuestra musa Nora.

Páginas que quedan para fases posteriores:
- Tienda online de cuadros y enmarques físicos (carrito de compras con WP EasyCart y pasarela de pagos).
- Panel de usuario / Mi Cuenta para clientes registrados.

3. Plan del Tema

- Nombre del tema: `nora-fotografia-felina`
- Tipo de tema: Custom (propio), desarrollado a medida para reflejar la identidad visual y la calidez del emprendimiento centrado en mascotas.

Carta Gantt (Etapas del Proyecto)

| Etapa / Actividad | Fecha de Inicio | Fecha de Término | Estado / Checkpoint |

| Identidad visual y estilos base | 05 Nov 2026 | 09 Nov 2026 | Por iniciar |
| Desarrollo de página Inicio y Blog | 10 Nov 2026 | 14 Nov 2026 | Por iniciar |
| Creación de páginas (Nosotros, Servicios, Contacto) | 15 Nov 2026 | 17 Nov 2026 | Por iniciar |
| **Checkpoint y revisión de avances** | **18 Nov 2026** | **18 Nov 2026** | **Hito clave** |
| Configuración de plugins y ajustes finales | 19 Nov 2026 | 24 Nov 2026 | Por iniciar |
| **Entrega final del proyecto** | **25 Nov 2026** | **25 Nov 2026** | **Entrega oficial** |

4. Plan B (Riesgos y Mitigaciones)

| Riesgo detectado | Acción de resolución (Mitigación) | Cuándo se activa (Señal o Fecha) |

| El tema propio presenta errores de código o no carga bien. | Se revierte al último commit funcional en Git o se cambia temporalmente a un tema descargado (ej. Astra) para cumplir con la estructura. | Si el diseño no levanta correctamente al 11 de noviembre. |
| Un plugin de optimización o formulario genera conflictos internos. | Se desactiva inmediatamente el plugin afectado y se reemplaza por la alternativa secundaria evaluada (ej. usar Rank Math en vez de Yoast, o W3 Total Cache). | Al momento de realizar las pruebas de integración de plugins. |
| Problemas de rendimiento o caída del servidor gratuito (InfinityFree).| Se espera unos minutos de margen; si persiste, se traslada el flujo temporalmente de trabajo local a Local WP para continuar el desarrollo. | Si el error del servidor se extiende por más de 1 hora continua
