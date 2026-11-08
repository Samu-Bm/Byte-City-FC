# 🔎 Referencias de diseño e identidad visual

Este documento recoge el análisis del estándar visual y la estructura estética que guiarán el desarrollo de **Byte City FC**.

> El objetivo es lograr una identidad visual moderna, digital y deportiva: una estética oscura (*dark mode*), limpia y minimalista inspirada en los clubes de fútbol de nueva generación que unen deporte, tecnología y cultura urbana.

## Principios y elementos de diseño

| Elemento de referencia | Cómo se adapta a Byte City FC | Ubicación / Archivo |
|---|---|---|
| **Hero de gran impacto** con escudo centrado, lema y dos llamadas a la acción (CTAs) | Portada con el escudo oficial, el lema «Play Code Win» y accesos directos a Partidos y Plantilla | `index.html` |
| **Tarjeta de próximo partido** con escudos enfrentados, hora, competición y estadio | Bloque visual moderno con escudos de Byte City FC vs. Code United FC, detalles del encuentro y cuenta atrás estética | `index.html` / `pages/partidos.html` |
| **Tarjetas métricas clave** (temporada, competición, estadio) | Bloques destacados en formato KPI / métricas resumen del club | `index.html` |
| **Sección institucional («El Club»)** con historia, estadio y afición | Diseño editorial en rejilla con tipografía condensada y bloques limpios | `index.html` / `pages/club.html` |
| **Escaparate de equipaciones («Nuestra Piel»)** | Muestra de primera, segunda y tercera equipación con fotografía y estética *streetwear* | `pages/nuestra-piel.html` |
| **Menú de navegación minimalista** con submenú desplegable en «Club» | Menú superior con navegación rápida y botón destacado en verde lima para «Hazte socio» | Todas las páginas |
| **Pie de página corporativo** con navegación, aviso legal y enlaces | Footer estructurado con enlaces semánticos y derechos de autor | Todas las páginas |
| **Estética oscura y acento de contraste** | Fondo negro `#080F0E` y acento verde lima neón `#B6FF00` para botones, badges y detalles clave | `css/base.css` |

## Criterios técnicos de adaptación

| Criterio | Decisión técnica en Byte City FC |
|---|---|
| **Pureza de lenguajes** | Todo el diseño se implementará con **HTML5 semántico y CSS3 puro** (Flexbox y Grid), sin frameworks pesados ni dependencias externas. |
| **Interactividad sin dependencias** | Los desplegables y efectos hover se resolverán mediante transiciones y pseudoclases CSS (`:hover`, `:focus-within`), aptos para el módulo de Lenguajes de Marcas. |
| **Accesibilidad (a11y)** | Ratios de contraste adecuados según WCAG (texto negro sobre verde lima, texto blanco roto sobre negro/gris). |


---

<div align="center">

[⬅️ Requisitos](07-requisitos.md) · [📚 Índice](../README.md#-documentación)

</div>
