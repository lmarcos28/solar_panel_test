# Imágenes pendientes

Este proyecto usa placeholders visuales (`.ph`) en lugar de imágenes reales para poder maquetar
el diseño sin depender de material fotográfico. Cuando tengáis las fotos definitivas, sustituid
cada placeholder por una etiqueta `<img>` (o `background-image`) manteniendo la misma relación de
aspecto para no romper la composición.

## Placeholders a sustituir

| Ubicación | Archivo/sección en `index.html` | Ratio recomendado | Contenido sugerido |
|---|---|---|---|
| Hero (visual principal) | `.ph--hero` dentro de `#inicio` | 4:5 (vertical) | Vivienda unifamiliar con paneles solares instalados, luz cálida de atardecer |
| Contacto (mapa) | `.ph--map` dentro de `#contacto` | 16:10 | Mapa de zona de cobertura o foto de oficina |

## Testimonios

Los avatares de `#testimonios` usan iniciales sobre un círculo de color (sin imagen) para no
depender de fotos de clientes ficticias. Cuando incorporéis testimonios reales, podéis:

- Mantener las iniciales (recomendado si no tenéis foto de todos los clientes), o
- Sustituir el `<div class="avatar">` por una `<img>` circular de 44x44px.

## Notas

- Los iconos de ventajas, proceso y contacto son SVG inline hechos a medida (no dependen de
  ninguna librería externa), así que no requieren archivos adicionales.
- El formulario de contacto (`#contactForm`) es solo de front-end: al enviarlo se muestra un
  mensaje de éxito simulado. Falta conectarlo a un backend o servicio de email real (por ejemplo
  Formspree, un endpoint propio, etc.) antes de producción.
