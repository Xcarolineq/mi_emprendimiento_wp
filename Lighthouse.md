# Análisis de rendimiento con Lighthouse

*Sitio analizado:* http://caroline207.ct.ws (página de inicio en producción)  
*Herramienta:* (https://pagespeed.web.dev/analysis/https-caroline207-ct-ws/knxkeoxvgkadv9pttsh8yi?form_factor=desktop)
*Fecha del análisis:* 24 de noviembre de 2026

## 1. Resultados (1 pt)

| Categoría | Puntaje (0 a 100) |
| :--- | :--- |
| Rendimiento | *96* / 100 |
| Accesibilidad | *100* / 100 |
| Buenas prácticas | *100* / 100 |
| SEO | *92* / 100 |

*Evidencia:* Informe generado en PageSpeed Insights https://pagespeed.web.dev/analysis/https-caroline207-ct-ws/knxkeoxvgkadv9pttsh8yi?form_factor=desktop 

## 2. Análisis (1 pt)

* *Qué significan los puntajes:* Los resultados reflejan un sitio altamente optimizado incluso operando sobre un servidor gratuito (InfinityFree). El rendimiento en móvil alcanzó 96/100 con métricas rápidas (First Contentful Paint de 2.0 s, Largest Contentful Paint de 2.3 s, 0 ms de bloqueo de interacción y 0 desplazamiento visual inesperado).
* *Mi mejor categoría y por qué:* *Accesibilidad (100/100)* y *Buenas prácticas (100/100)* obtuvieron el puntaje máximo. Esto se debe al uso del tema oficial *Twenty Twenty-Five*, que garantiza una estructura semántica limpia, buen contraste de lectura y estándares modernos de código sin errores en consola.
* *Mi categoría más débil y por qué:* *SEO (92/100)* fue la categoría más baja (aunque sigue estando en rango verde sobresaliente) debido a una única advertencia específica detectada por la herramienta: la página de inicio no cuenta aún con una etiqueta de meta descripción definida.
* *Problemas que encontró el informe:* 
  1. Falta de meta descripción en el documento principal (SEO).
  2. Posibilidad de optimizar la entrega de fotografías del portafolio felino (ahorro estimado de 376 KiB).
  3. Solicitudes que bloquean parcialmente el renderizado inicial (1.450 ms) y carga de fuentes tipográficas (190 ms).

## 3. Mejoras (1 pt)

| Mejora | Qué problema resuelve | ¿Aplicada o propuesta? | Resultado (si la aplicaste) |
| :--- | :--- | :--- | :--- |
| *Compresión automática de fotografías con el plugin Smush* | Reduce el peso de las fotografías de gatos en alta resolución y activa la carga diferida (Lazy Load) para acelerar la carga en celulares. | *Aplicada* | Se logró mantener el tiempo de carga del elemento principal (LCP) en 2.3 s en móvil y alcanzar 96 puntos en Rendimiento. |
| *Redacción de meta descripciones con Yoast SEO* | Resuelve la advertencia "El documento no tiene una meta descripción" detectada en la auditoría SEO para mejorar la visibilidad en buscadores. | *Propuesta* | Permitirá elevar el puntaje de SEO de 92 a 100 / 100 al definir descripciones únicas para Inicio, Blog, Nosotros y Contactame. |
| *Conversión de imágenes nuevas a formato WebP* | Aprovecha el ahorro adicional de 376 KiB sugerido por Lighthouse en la entrega de imágenes sin perder calidad visual en los retratos. | *Propuesta* | Reducirá aún más el consumo de datos móviles y mantendrá el rendimiento por encima de 95 cuando se agreguen nuevas fotos al portafolio. |
