# 🔎 Referencias de diseño

Referencia visual propuesta: **Rōnin FC** — [roninfc.digital](https://roninfc.digital/). Las adaptaciones descritas abajo son objetivos de diseño; todavía no están implementadas en las páginas.

> Solo se toma como referencia el **diseño y la estructura**. No se copian logos, textos, imágenes ni el diseño al pie de la letra: Byte City es un club ficticio y tiene su propia identidad.

## Qué se toma de referencia

| Elemento de Rōnin FC | Cómo se adapta a Byte City | Página / archivo |
|---|---|---|
| Hero con escudo grande, lema de dos líneas y dos botones | Escudo, «Fútbol con código en las venas» y botones a Partidos y Equipo | `index.html` |
| Tarjeta de próximo partido con escudos, «VS», hora y estadio | `<aside>` con la misma estructura, sin cuenta atrás | `index.html` |
| «Quiénes somos» con Historia, Estadio y Equipo | Bloque resumen en Inicio que enlaza a `club.html` | `index.html` · `club.html` |
| Tres tarjetas de datos (entrenador, competición, temporada) | Tarjetas pequeñas con datos rápidos del club | `index.html` |
| Menú corto con «Club» desplegable | «Club» desplegable (Historia, Estadio, Afición) hecho con CSS | Todas las páginas |
| Pie con navegación, redes, texto legal y créditos | Igual, más el formulario de boletín | Todas las páginas |
| Aviso legal como página aparte | `legal.html` sencilla | `legal.html` |
| Fondo negro, estética minimalista y detalle en japonés | Paleta propia negro y verde lima, con un detalle propio (binario o la palabra «byte») | `css/base.css` |

## Qué no se copia

| Elemento | Motivo |
|---|---|
| Logo, textos, imágenes y diseño al pie de la letra | Es un club real; Byte City debe tener identidad propia |
| Cuenta atrás del próximo partido | Necesita JavaScript (el proyecto es un sitio estático) |
| Mapa interactivo del estadio | Necesita JavaScript; se sustituye por una imagen |
| Sección «Directo» | Necesita JavaScript y contenido en tiempo real |

---

<div align="center">

[⬅️ Requisitos](07-requisitos.md) · [📚 Índice](../README.md#-documentación)

</div>
