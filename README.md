<div align="center">

# ⚽ BYTE CITY FC

### *Fútbol con código en las venas.*

Proyecto educativo de un club de fútbol ficticio. El sitio ya cuenta con una portada HTML semántica y recursos gráficos; el resto de páginas y los estilos siguen en desarrollo.

</div>

---

## Estado actual

La implementación está en desarrollo:

- La única página implementada es [`html/index.html`](html/index.html). Incluye encabezado y navegación, portada con lema y enlaces, próximo partido, historia, información del estadio y pie de página.
- La navegación ya apunta a las páginas previstas, pero esas páginas todavía no existen; por tanto, esos enlaces aún no conducen a contenido implementado.
- Los recursos gráficos disponibles están en [`img/`](img/): escudo de Byte City FC, escudo de Code United FC, tres equipaciones y artículos de ropa.
- La planificación y las propuestas de diseño están en [`docs/`](docs/).
- Todavía no existen hojas CSS, formularios funcionales ni comportamiento JavaScript. La portada no enlaza ninguna hoja de estilos.

Las páginas y funcionalidades detalladas en la documentación que no aparecen en la portada son objetivos de diseño, no características implementadas.

## Estructura del proyecto

```text
.
├── README.md
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
├── html/
│   └── index.html
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
| [Guía de estilo](docs/03-guia-de-estilo.md) | Identidad visual y recursos gráficos |
| [Páginas y contenidos](docs/04-paginas.md) | Propuesta de páginas, todavía no implementadas |
| [Formularios](docs/05-formularios.md) | Especificación de formularios, todavía no implementados |
| [Accesibilidad y validación](docs/06-accesibilidad-y-validacion.md) | Criterios pendientes de aplicar y comprobar |
| [Requisitos](docs/07-requisitos.md) | Seguimiento del alcance frente a lo que existe |
| [Referencias de diseño](docs/08-referencias-de-diseno.md) | Referencia visual y adaptaciones propuestas |

## Identidad visual propuesta

La guía propone verde lima (`#B6FF00`), negro (`#080F0E`), gris oscuro (`#252B2A`) y blanco roto (`#F5F7F5`), con Barlow Condensed e Inter. Estos estilos aún no están aplicados en una hoja CSS.

## Próximos pasos

1. Implementar las páginas previstas y comprobar los enlaces del menú.
2. Crear los estilos y adaptar el sitio a móvil y escritorio.
3. Revisar accesibilidad, enlaces y validación HTML/CSS; guardar evidencias en `docs/validacion/`.
4. Completar los mockups en `docs/mockups/`.

---

<div align="center">

*Club ficticio creado con fines educativos.*

</div>
