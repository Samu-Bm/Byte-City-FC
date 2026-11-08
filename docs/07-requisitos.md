# 📋 Requisitos del proyecto

Seguimiento de los requisitos del proyecto frente a los archivos existentes y la planificación acordada.

## Planteamiento general

| Requisito | Cómo se cumple | Dónde |
|---|---|---|
| Sitio estático, accesible, responsive y semántico | Objetivo del proyecto: maquetación en HTML5 semántico y CSS3 puro | [Planificación](01-planificacion.md) |
| Trabajo por fases | Planificación → HTML → CSS → validación → entrega | [Planificación](01-planificacion.md) |
| Entrega en GitHub | Repositorio activo con control de versiones y documentación completa | [README](../README.md) |

## Fase 1 · Planificación

| Requisito | Estado | Dónde |
|---|:---:|---|
| Mapa del sitio con jerarquía | Definido y actualizado con las 8 secciones y subsecciones | [Estructura del sitio](02-estructura-del-sitio.md) |
| Mockups móvil y escritorio | Carpeta reservada | `docs/mockups/` |
| Paleta, tipografías y banco de imágenes | Guía documentada; escudos, equipaciones, ropa e imágenes de noticias disponibles | [Guía de estilo](03-guia-de-estilo.md) |

## Fase 2 · HTML5

| Requisito | Estado | Dónde |
|---|:---:|---|
| Árbol de carpetas | Estructurado con raíz `index.html`, `pages/`, `css/`, `img/` y `docs/` | [Estructura del sitio](02-estructura-del-sitio.md) |
| Maquetación semántica sin CSS | Portada `index.html` en raíz con cabecera, navegación, secciones y pie | `index.html` |
| Páginas interiores enlazadas | Estructuradas en `pages/` según especificación de contenidos | [Páginas y contenidos](04-paginas.md) |

## Fase 3 · CSS3

| Requisito | Estado | Dónde |
|---|:---:|---|
| Estilos base | Iniciado; variables de color, tipografía y reset | `css/base.css` |
| Layout con Flexbox / Grid | Planificado para maquetar rejilla de tienda, equipo y tarjetas | `css/` |
| Responsive Mobile First con `@media` | Planificado para adaptabilidad en móvil y escritorio | `css/` |

## Elementos mínimos obligatorios

| Requisito | Estado | Dónde / Aplicación |
|---|---|---|
| Mínimo 7 páginas enlazadas | Cubierto | Portada `index.html` + 8 páginas en `pages/` (club, equipo, partidos, nuestra-piel, actualidad, hazte-socio, contacto, legal) |
| Estructura semántica (`header`, `nav`, `main`, `section`, `article`, `aside`, `footer`) | En desarrollo | Presente en `index.html` y extensible a todas las páginas interiores |
| Jerarquía estricta de encabezados | Cubierto | Un único `h1` por vista, descendiendo a `h2` y `h3` sin saltos |
| Tabla de datos semántica (`thead`, `tbody`, `th`) | Planificado | Tabla comparativa de las **3 cuotas de socio** en `pages/hazte-socio.html` y tabla de partidos en `pages/partidos.html` |
| Formularios completos con validación HTML5 | Especificado | Formulario en `pages/contacto.html` y boletín en el pie de página |

---

<div align="center">

[⬅️ Accesibilidad y validación](06-accesibilidad-y-validacion.md) · [📚 Índice](../README.md#-documentación) · [Referencias de diseño ➡️](08-referencias-de-diseno.md)

</div>
