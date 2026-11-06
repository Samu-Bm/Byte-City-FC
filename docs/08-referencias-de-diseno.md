# 🔎 Referencias de diseño

Referencia visual propuesta: **Rōnin FC** — [roninfc.digital](https://roninfc.digital/). La tabla indica qué elementos de la portada ya se han implementado y cuáles siguen pendientes.

> Solo se toma como referencia el **diseño y la estructura**. No se copian logos, textos, imágenes ni el diseño al pie de la letra: Byte City es un club ficticio y tiene su propia identidad.

## Qué se toma de referencia

| Elemento de Rōnin FC | Cómo se adapta a Byte City | Página / archivo |
|---|---|---|
| Hero con escudo grande, lema y dos botones | Portada implementada con escudo, lema «Play - code..» y enlaces a Partidos y Equipo | `html/index.html` |
| Tarjeta de próximo partido con escudos, «VS», hora y estadio | Implementada parcialmente con competición, jornada, escudos, equipos y hora; fecha, estadio y detalle pendientes | `html/index.html` |
| «Quiénes somos» con Historia, Estadio y Equipo | Implementado parcialmente con artículos de Historia y Estadio; bloque Equipo y página `club.html` pendientes | `html/index.html` |
| Tres tarjetas de datos (entrenador, competición, temporada) | Pendientes de implementar | `html/index.html` |
| Menú corto con «Club» desplegable | Enlaces de navegación y submenú definidos en HTML; el comportamiento visual desplegable requiere CSS | `html/index.html` |
| Pie con navegación, redes, texto legal y créditos | Pie implementado con enlaces a Aviso legal y Contacto; redes y boletín pendientes | `html/index.html` |
| Aviso legal como página aparte | Enlace presente; la página aún no está creada | `legal.html` (pendiente) |
| Fondo negro, estética minimalista y detalle en japonés | Paleta negro y verde lima propuesta; aún no hay CSS que la aplique | `css/base.css` (pendiente) |

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
