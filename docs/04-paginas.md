# 📄 Páginas y contenidos

Especificación detallada del contenido y la estructura de las páginas de **Byte City FC**, adaptadas a los requisitos del proyecto.

## Estado actual del sitio

- **Página implementada:** `index.html` (ubicada en la raíz del proyecto), con cabecera, navegación, hero con lema, tarjeta de próximo partido, extracto de historia/estadio y pie de página.
- **Hojas de estilo:** `css/base.css` (variables de color, tipografía y reset inicial).
- **Páginas interiores:** planificadas dentro de la carpeta `pages/` para su desarrollo.

| # | Página | Archivo | Descripción resumida |
|:-:|---|---|---|
| 1 | Inicio | `index.html` | Portada institucional, hero, próximo partido y accesos rápidos |
| 2 | Club | `pages/club.html` | Historia, estadio y afición (peñas y contador de socios) |
| 3 | Equipo | `pages/equipo.html` | Plantilla por demarcación (porteros, defensas, medios, delanteros) + cuerpo técnico |
| 4 | Partidos | `pages/partidos.html` | Calendario con 4–5 partidos recientes (matchdays / tablas) |
| 5 | Nuestra piel (Tienda) | `pages/nuestra-piel.html` | Tienda online: 3 equipaciones + merchandising con detalle de producto |
| 6 | Actualidad | `pages/actualidad.html` | Portal de noticias con acceso a fotos y texto completo de cada noticia |
| 7 | Hazte socio | `pages/hazte-socio.html` | Página estática informativa con 3 cuotas diferenciadas y sus beneficios |
| 8 | Contacto | `pages/contacto.html` | Correo electrónico, teléfono, redes sociales y disclaimer de contacto |
| 9 | Aviso legal | `pages/legal.html` | Aviso legal informativo y carácter académico del sitio |

---

> **Estructura semántica común en todas las páginas:**
> - `<header>`: Logo/escudo del club y `<nav>` con el menú de navegación principal.
> - `<main>`: Contenedor único del contenido de cada página.
> - `<footer>`: Correo de contacto, redes sociales ficticias, enlaces legales y aviso de copyright.
> - Jerarquía estricta de encabezados: un único `<h1>` por página, seguido de `<h2>` y `<h3>` estructurados.

---

## 🏠 1. Inicio — `index.html`

Página principal del club situada en la raíz del repositorio.

| Bloque | Elemento HTML | Contenido |
|---|---|---|
| **Cabecera** | `<header>` | Escudo, nombre del club y barra de navegación `<nav>` |
| **Hero / Banner** | `<section>` | Escudo destacado, lema *«PLAY - CODE - WIN»* y botones de acceso directo a Partidos y Equipo |
| **Próximo partido** | `<section>` / `<article>` | Encuentro de Liga Digital: escudos de Byte City FC vs. Code United FC, fecha y hora |
| **Quiénes somos** | `<section>` | Resumen introductorio del club y de su sede/estadio con enlace a `pages/club.html` |
| **Pie de página** | `<footer>` | Enlaces a contacto, redes sociales y aviso legal |

---

## 🛡️ 2. Club — `pages/club.html`

Sección institucional dividida en tres apartados clave con anclas de navegación directa:

### A) Historia (`#historia`)
- Narrativa sobre el origen y la fundación del club en el entorno tecnológico de Byte City.
- Fotografías históricas representativas (`<figure>` con `<figcaption>`).
- Evolución y momentos cumbre explicados de forma clara y amena.

### B) Estadio (`#estadio`)
- Fotografías del estadio oficial del club.
- Información esencial y ficha técnica concisa:
  - Año de creación/inauguración.
  - Ubicación dentro de Byte City.
  - Capacidad de espectadores y tipo de superficie.

### C) Afición (`#aficion`)
- Homenaje a la hinchada y comunidad del club con fotos de la grada y la afición en día de partido.
- **Peñas oficiales actuales:** listado y mención a las peñas activas del club.
- **Contador de socios:** dato destacado en texto plano indicando la masa social actual de Byte City FC (ejemplo: *«Más de 12.500 socios activos»*).

---

## 👥 3. Equipo — `pages/equipo.html`

Presentación completa de la plantilla y el cuerpo técnico organizada de forma clara por demarcaciones:

### Demarcaciones de jugadores
1. **Porteros:** tarjetas individuales de los guardametas con foto, nombre y dorsal.
2. **Defensas:** defensas centrales y laterales con foto, nombre y dorsal.
3. **Centrocampistas:** mediocentros defensivos y creativos con foto, nombre y dorsal.
4. **Delanteros:** extremos y delanteros centro con foto, nombre y dorsal.

### Cuerpo técnico
- **Primer Entrenador:** fotografía, nombre, trayectoria y rol en el banquillo.
- **Segundo Entrenador:** fotografía, nombre y funciones tácticas en el cuerpo técnico.

*Cada miembro contará con su tarjeta en `<article>` con imagen, nombre, rol/posición y dorsal correspondiente.*

---

## 📅 4. Partidos — `pages/partidos.html`

Seguimiento de la competición con foco en los partidos recientes:

- **4 a 5 partidos recientes:** resumen de los últimos encuentros disputados por el club.
- **Formato visual:** presentación mediante tarjetas tipo *Matchday* con imágenes de los encuentros o mediante tablas semánticas (`<table>`, `<thead>`, `<tbody>`, `<th>`).
- **Datos de cada partido:**
  - Equipos enfrentados y escudos (local y visitante).
  - Marcador y resultado final.
  - Competición, jornada y fecha del encuentro.
  - Fotografía ilustrativa del día del partido.

---

## 👕 5. Nuestra piel (Tienda) — `pages/nuestra-piel.html`

Página estructurada como una **tienda online** oficial del club, dividida en dos grandes bloques:

### A) Equipaciones oficiales (Sección superior)
- **Primera equipación (Home):** imagen frontal/trasera, título, descripción y precio.
- **Segunda equipación (Away):** imagen frontal/trasera, título, descripción y precio.
- **Tercera equipación (Alternative):** imagen frontal/trasera, título, descripción y precio.

### B) Merchandising y accesorios (Sección inferior)
- Catálogo de productos oficiales: balones, gorras, bufandas, sudaderas y ropa de entrenamiento.
- Presentación en rejilla de tarjetas de producto.

### C) Ficha / Detalle de cada producto
- Cada artículo permite abrirse (o cuenta con su ficha detallada) mostrando:
  - Galería con distintas imágenes del mismo producto (diferentes ángulos o detalles).
  - Título oficial del producto.
  - Descripción de características, materiales y precio.

---

## 📰 6. Actualidad — `pages/actualidad.html`

Portal de noticias y actualidad de Byte City FC:

- **Listado de noticias:** tarjetas con titular, fecha, fotografía de cabecera y entradilla.
- **Acceso a la noticia completa:** cada noticia permite acceder a su página o sección de detalle para:
  - Ver la galería o fotos del evento / suceso.
  - Leer el cuerpo de la noticia en texto completo (`<article>`, párrafos, declaraciones y subtítulos).

---

## 🎟️ 7. Hazte socio — `pages/hazte-socio.html`

Página estática informativa diseñada para dar a conocer las modalidades de abono y ventajas de ser socio:

- **3 cuotas diferenciadas:**
  1. **Cuota Joven / Junior:** cuota reducida para los aficionados más jóvenes.
  2. **Cuota Adulto / Estándar:** modalidad completa para el seguidor general.
  3. **Cuota Premium / VIP:** pase con acceso a zonas exclusivas y ventajas adicionales.
- **Información detallada por cuota:**
  - Precio / coste periódico (anual o mensual).
  - Lista de beneficios incluidos (descuentos en tienda, acceso prioritario a entradas, carné físico/digital, asiento garantizado, etc.).
- **Diseño estático:** comparativa limpia mediante tabla semántica o tarjetas de precios destacadas, sin necesidad de pasarela de pago real.

---

## ✉️ 8. Contacto — `pages/contacto.html`

Página institucional de atención al aficionado y medios:

- **Datos oficiales de contacto:**
  - Correo electrónico oficial del club.
  - Teléfono de atención al aficionado y oficinas.
  - Enlaces a las redes sociales oficiales (RRSS ficticias: X, Instagram, YouTube).
- **Disclaimer y horarios:** texto informativo sobre horarios de atención y advertencia de uso adecuado del canal.
- **Ubicación:** mapa esquemático o dirección física en Byte City.

---

## ⚖️ 9. Aviso legal — `pages/legal.html`

Página informativa de cumplimiento y transparencia enlazada desde el pie:

- **Aviso legal estándar:** condiciones generales de uso del sitio web.
- **Naturaleza del proyecto:** aclaración expresa de que Byte City FC es un club ficticio creado con fines exclusivamente académicos y formativos.
- **Propiedad intelectual y créditos:** atribución de fuentes, recursos gráficos y autoría del proyecto.

---

<div align="center">

[⬅️ Guía de estilo](03-guia-de-estilo.md) · [📚 Índice](../README.md#-documentación) · [Formularios ➡️](05-formularios.md)

</div>
