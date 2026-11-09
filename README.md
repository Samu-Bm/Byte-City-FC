<div align="center">

# ⚽ BYTE CITY FC

### *PLAY - CODE - WIN*

Proyecto educativo de un club de fútbol ficticio. El sitio ya cuenta con una portada HTML semántica y recursos gráficos; el resto de páginas y los estilos siguen en desarrollo.

</div>

---

## Estado actual

La implementación se encuentra en desarrollo activo:

- **Portada principal:** [`index.html`](index.html), ubicada en la raíz del proyecto. Incluye encabezado con escudo, navegación principal, sección hero con lema oficial, tarjeta del próximo partido, resumen de historia y estadio, y pie de página institucional.
- **Páginas interiores:** planificadas y organizadas dentro de [`pages/`](pages/) para las distintas secciones del club (Club, Equipo, Partidos, Nuestra piel / Tienda, Actualidad, Hazte socio, Contacto y Legal).
- **Estilos:** se ha creado [`css/base.css`](css/base.css) estableciendo las variables de color corporativo, tipografías y reset de base.
- **Recursos gráficos:** organizados en [`img/`](img/): escudos del club y rivales, fotografías de las tres equipaciones oficiales, artículos de merchandising/ropa y banco de imágenes para noticias.
- **Documentación técnica:** especificaciones completas en [`docs/`](docs/).

## Estructura del proyecto

```text
.
├── README.md
├── index.html
├── css/
│   └── base.css
├── pages/
├── docs/
│   ├── 01-planificacion.md
│   ├── 02-estructura-del-sitio.md
│   ├── 03-guia-de-estilo.md
│   ├── 04-paginas.md
│   ├── 05-formularios.md
│   ├── 06-accesibilidad-y-validacion.md
│   ├── 07-requisitos.md
│   ├── 08-referencias-de-diseno.md
│   ├── mockups/
│   └── validacion/
└── img/
    ├── aficion/
    ├── codeunitedfc/
    ├── equipaciones/
    ├── estadio/
    ├── jugadores/
    ├── logo/
    ├── noticias/
    ├── ropa/
    └── escudo/
```

Los directorios vacíos se conservan con `.gitkeep`.

## Documentación

| Documento | Contenido |
|---|---|
| [Planificación](docs/01-planificacion.md) | Fases de trabajo y estado |
| [Estructura del sitio](docs/02-estructura-del-sitio.md) | Sitemap previsto y estructura actual de carpetas |
| [Guía de estilo](docs/03-guia-de-estilo.md) | Sistema de diseño, identidad visual, tipografía y recursos gráficos |
| [Páginas y contenidos](docs/04-paginas.md) | Propuesta de páginas, todavía no implementadas |
| [Formularios](docs/05-formularios.md) | Especificación de formularios, todavía no implementados |
| [Accesibilidad y validación](docs/06-accesibilidad-y-validacion.md) | Criterios pendientes de aplicar y comprobar |
| [Requisitos](docs/07-requisitos.md) | Seguimiento del alcance frente a lo que existe |
| [Referencias de diseño](docs/08-referencias-de-diseno.md) | Referencia visual y adaptaciones propuestas |

## Identidad visual y tipografía

La identidad visual implementa un contraste editorial entre **Brier Bold 700** (Didone serif de acento local) y **Mona Sans** (fuente principal desde Google Fonts), junto a la paleta oficial (`#080F0E` negro, `#B6FF00` verde lima neón, `#F5F7F5` blanco roto) y referencias editoriales crema/bosque. Todo el sistema está documentado al detalle en la [Guía de estilo](docs/03-guia-de-estilo.md).

## Próximos pasos

1. Implementar las páginas previstas y comprobar los enlaces del menú.
2. Crear los estilos y adaptar el sitio a móvil y escritorio.
3. Revisar accesibilidad, enlaces y validación HTML/CSS; guardar evidencias en `docs/validacion/`.
4. Completar los mockups en `docs/mockups/`.

---

<div align="center">

*Club ficticio creado con fines educativos.*

</div>
