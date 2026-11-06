# 📄 Páginas y contenidos

Propuesta de contenido para las **14 páginas previstas** del sitio. La portada `html/index.html` ya está implementada parcialmente. Las otras 13 páginas todavía no existen.

## Estado de la portada implementada

La página existente incluye:

- Cabecera con escudo, nombre del club y menú de navegación.
- Portada con escudo, lema «Play - code..» y enlaces a Partidos y Equipo.
- Próximo partido de Liga Digital entre Byte City FC y Code United FC, con hora y escudos.
- Sección «Quiénes somos» con historia y estadio; la ubicación se presenta en un `<aside>`.
- Pie de página con aviso legal y contacto.

El calendario, la fecha y el estadio del próximo encuentro no aparecen todavía en la página. Los enlaces a páginas interiores apuntan a destinos aún no implementados.

| # | Página | Archivo |
|:-:|---|---|
| 1 | Inicio | `index.html` |
| 2 | Club | `club.html` |
| 3 | Equipo | `equipo.html` |
| 4 | Ficha de jugador | `jugador.html` |
| 5 | Partidos | `partidos.html` |
| 6 | Detalle de partido | `partido.html` |
| 7 | Clasificación | `clasificacion.html` |
| 8 | Nuestra piel | `nuestra-piel.html` |
| 9 | Actualidad | `actualidad.html` |
| 10 | Noticia | `noticia.html` |
| 11 | Hazte socio | `hazte-socio.html` |
| 12 | Gracias | `gracias.html` |
| 13 | Contacto | `contacto.html` |
| 14 | Aviso legal | `legal.html` |

---

> **Estructura común a todas las páginas**
> - `<header>` con el logo y `<nav>` con el menú principal (con **Club** como submenú desplegable y **Hazte socio** como botón destacado).
> - `<main>` con el contenido único de la página.
> - `<footer>` con: contacto, enlaces de interés, redes sociales ficticias, datos del club, enlace al [aviso legal](#️-aviso-legal--legalhtml) y **formulario de boletín** (email + casilla de consentimiento + botón).
> - Un solo `<h1>` por página; después `<h2>` y `<h3>` sin saltarse niveles.

---

## 🏠 Inicio — `html/index.html`

La tabla siguiente recoge el alcance previsto para la portada; los bloques que aún no se mencionan en el apartado «Estado de la portada implementada» siguen pendientes.

| Bloque | Etiqueta | Contenido |
|---|---|---|
| Banner | `<section>` | Implementado con escudo, lema *«Play - code..»* y enlaces **Ver Partidos** y **Conoce al Equipo** |
| Quiénes somos | `<section>` | Implementado con artículos de historia y estadio; la ubicación se agrupa en un `<aside>` |
| Datos rápidos | `<section>` con 3 `<article>` | Tarjetas: entrenador, competición y temporada |
| Próximo partido | `<section>` y `<article>` | Implementado con competición, jornada, equipos, escudos y hora; fecha, estadio y enlace al detalle pendientes |
| Último resultado | `<aside>` | Marcador, rival y enlace a la crónica |
| Últimas noticias | `<section>` con 3 `<article>` | Imagen, título, fecha y enlace |
| Jugadores destacados | `<section>` con 3 `<article>` | Foto, nombre, dorsal, posición |
| Equipaciones | `<section>` | Imagen de la primera equipación + enlace a Nuestra piel |
| Mini clasificación | `<section>` | Tabla con los 5 primeros puestos |
| Llamada a socios | `<section>` | Texto breve + botón a `hazte-socio.html` |

**Encabezados implementados:** `h1` BYTE CITY FC → `h2` Próximo partido / Quiénes somos → `h3` Nuestra historia / Nuestro estadio → `h4` Ubicación. Los demás encabezados indicados en la propuesta siguen pendientes.

---

## 🛡️ Club — `club.html`

| Bloque | Contenido |
|---|---|
| **Historia** | Año de fundación, origen del nombre (ciudad tecnológica), evolución por etapas (lista ordenada `<ol>` tipo línea del tiempo) |
| **Identidad** | Imagen del escudo, explicación de sus elementos, colores corporativos con muestras |
| **Filosofía y valores** | Misión, visión y 4 valores (por ejemplo: innovación, trabajo en equipo, esfuerzo, comunidad), uno por `<article>` |
| **Estadio** | Nombre, capacidad, ubicación, año de inauguración, 3 imágenes (`<figure>` + `<figcaption>`) y ficha técnica en `<dl>` |
| **Afición** | Presentación de la afición y su historia, fotografías de seguidores (`<figure>`), actividades y eventos, y enlace a **Hazte socio** |
| **Palmarés** | Tabla de títulos: competición, temporadas, nº de títulos |

**Menú interno** (enlaces ancla): Historia · Identidad · Valores · Estadio · Afición · Palmarés.

**Submenú «Club» del menú principal:** apunta a las anclas `club.html#historia`, `club.html#estadio` y `club.html#aficion`, por lo que cada bloque lleva su `id`.

**Elemento obligatorio que cubre:** tabla de datos (palmarés).

---

## 👥 Equipo — `equipo.html`

Plantilla organizada por posiciones, cada una en su `<section>`:

| Sección | Nº orientativo |
|---|:---:|
| Porteros | 3 |
| Defensas | 6 |
| Centrocampistas | 6 |
| Delanteros | 4 |
| Cuerpo técnico | 3 |

**Tarjeta de jugador** (`<article>`): foto, nombre, dorsal, posición, nacionalidad, edad, altura y enlace a su ficha.

**Tabla de estadísticas individuales:** jugador, partidos, goles, asistencias, minutos.

> Los filtros por posición se resuelven con un **menú de enlaces ancla** a cada sección, sin JavaScript.

---

## 🧑‍🎤 Ficha de jugador — `jugador.html`

Una ficha completa de ejemplo.

| Bloque | Contenido |
|---|---|
| Cabecera | Foto grande, nombre, dorsal, posición |
| Datos personales | `<dl>`: fecha de nacimiento, edad, nacionalidad, altura, peso, pie hábil |
| Biografía | 2 párrafos |
| Trayectoria | Tabla: temporada, equipo, partidos, goles |
| Estadísticas de la temporada | Tabla: goles, asistencias, minutos, tarjetas |
| Navegación | Enlace de vuelta a la plantilla |

---

## 📅 Partidos — `partidos.html`

| Bloque | Contenido |
|---|---|
| **Próximos partidos** | Tabla de calendario: jornada, fecha, hora, rival, competición, estadio |
| **Resultados** | Tabla: jornada, fecha, local, marcador, visitante, enlace al detalle |
| **Competiciones** | Separación por Liga y Copa mediante `<section>` distintas |

**Rivales ficticios de ejemplo:** Real Compilers, Atlético Debug, Sporting Syntax, CF Cache, Deportivo Firewall, Racing Router.

**Elemento obligatorio que cubre:** tablas con `<thead>`, `<tbody>` y `<th scope>`.

---

## 📋 Detalle de partido — `partido.html`

Ficha de ejemplo de un encuentro ya disputado.

| Bloque | Contenido |
|---|---|
| Marcador | Equipos, escudos, resultado, fecha, estadio, competición |
| Goleadores | Lista con minuto |
| Alineaciones | Dos listas (titulares y suplentes) |
| Estadísticas | Tabla comparativa: posesión, tiros, tiros a puerta, faltas, córners |
| Crónica | Enlace a la noticia correspondiente |

---

## 🏆 Clasificación — `clasificacion.html`

| Bloque | Contenido |
|---|---|
| **Tabla general** | Posición, equipo, PJ, PG, PE, PP, GF, GC, DG, Pts (8 equipos, Byte City resaltado) |
| **Leyenda** | Significado de cada abreviatura (`<abbr title="...">`) |
| **Estadísticas del equipo** | Tabla de máximos goleadores y de asistentes |
| **Datos de la temporada** | Racha, victorias en casa/fuera, goles totales |

---

## 👕 Nuestra piel — `nuestra-piel.html`

| Bloque | Contenido |
|---|---|
| **Primera equipación** | Imágenes (frontal y trasera), colores, materiales, inspiración |
| **Segunda equipación** | Ídem |
| **Tercera equipación** | Ídem |
| **Equipación de portero** | Ídem |
| **Tienda** | Tabla o tarjetas de productos con nombre, descripción y precio |
| **Formulario de pedido (simulado)** | Producto (`select`), talla (`radio`), cantidad (`number`), dorsal y nombre personalizados (`text`), email (`email`), envío exprés (`checkbox`), botón **Comprar** |

Cada equipación en su propio `<article>` con `<figure>` y `<figcaption>`.

---

## 📰 Actualidad — `actualidad.html`

| Bloque | Contenido |
|---|---|
| **Noticia destacada** | `<article>` grande con imagen, título, fecha y categoría |
| **Listado de noticias** | 6 `<article>` con imagen, título, fecha, categoría y enlace |
| **Categorías** | Menú de enlaces: Primer equipo · Crónicas · Previas · Fichajes · Entrevistas · Comunicados · Equipaciones |
| **Multimedia** | Galería de fotos (`<figure>`) y 1–2 vídeos con `<video controls>` o incrustados |
| **Aside** | Últimos resultados y enlace a Hazte socio |

---

## 📄 Noticia — `noticia.html`

Noticia completa de ejemplo.

- `<article>` con `<h1>` título, `<time datetime>`, categoría, autor.
- Imagen principal con `<figcaption>`.
- Cuerpo en varios párrafos con un `<h2>` intermedio y una cita (`<blockquote>`).
- `<aside>` con noticias relacionadas.

---

## 🎟️ Hazte socio — `hazte-socio.html`

Página para hacerse socio de Byte City y suscribirse a las novedades.

**Bloques**

| Bloque | Contenido |
|---|---|
| Presentación | Por qué hacerse socio y qué aporta formar parte de la comunidad |
| **Tabla de modalidades** | Modalidad, cuota anual, ventajas |
| Ventajas | Lista de beneficios (descuentos en tienda, entradas prioritarias, carné, boletín exclusivo) |
| **Formulario de inscripción** | Ver [Formularios](05-formularios.md) |
| Comunidad | Texto breve con enlace a la sección **Afición** de `club.html` |

**Tabla de modalidades (propuesta)**

| Modalidad | Cuota anual | Ventajas |
|---|:---:|---|
| Junior (hasta 14 años) | 30 € | Carné, boletín |
| Joven (15–25) | 60 € | Carné, boletín, descuento en tienda |
| Adulto | 100 € | Carné, boletín, descuento en tienda, entrada prioritaria |
| Premium | 180 € | Todo lo anterior + asiento fijo y camiseta oficial |

**Formulario de inscripción:** ver los campos completos en [Formularios](05-formularios.md#-formulario-de-inscripción-de-socio).

---

## ✅ Gracias — `gracias.html`

Página de confirmación tras enviar la inscripción: mensaje de bienvenida, resumen de los siguientes pasos y enlaces de vuelta al inicio y a la tienda.

---

## ✉️ Contacto — `contacto.html`

| Bloque | Contenido |
|---|---|
| Datos del club | Dirección, teléfono, email, horario (`<address>`) |
| Ubicación | Imagen del mapa del estadio |
| **Formulario de contacto** (ver [Formularios](05-formularios.md)) | Nombre (`text`), email (`email`), teléfono (`tel`), asunto (`select`: Socios, Tienda, Prensa, Otros), mensaje (`textarea`), aceptación de privacidad (`checkbox`), botón de envío |
| Redes sociales | Enlaces a los perfiles ficticios |

## ⚖️ Aviso legal — `legal.html`

Página sencilla, enlazada desde el pie de todas las páginas.

| Bloque | Etiqueta | Contenido |
|---|---|---|
| Naturaleza del sitio | `<section>` | Aclarar que Byte City es un club ficticio y que la web es un proyecto educativo |
| Propiedad de contenidos | `<section>` | Origen de las imágenes y textos, y créditos de las fuentes utilizadas |
| Privacidad | `<section>` | Qué se hace con los datos de los formularios (en este proyecto no se almacenan) |
| Créditos | `<section>` | Autor del proyecto, módulo y ciclo formativo |

**Encabezados:** `h1` Aviso legal → `h2` por cada bloque.

---

---

<div align="center">

[⬅️ Guía de estilo](03-guia-de-estilo.md) · [📚 Índice](../README.md#-documentación) · [Formularios ➡️](05-formularios.md)

</div>
