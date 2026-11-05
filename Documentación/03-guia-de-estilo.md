# 🎨 Guía de estilo

## Paleta oficial

| Muestra | Color | HEX | Uso |
|:---:|---|:---:|---|
| ![](https://placehold.co/60x24/B6FF00/B6FF00.png) | Verde lima | `#B6FF00` | Acento, botones, enlaces, números destacados |
| ![](https://placehold.co/60x24/080F0E/080F0E.png) | Negro | `#080F0E` | Fondo principal |
| ![](https://placehold.co/60x24/252B2A/252B2A.png) | Gris oscuro | `#252B2A` | Tarjetas, superficies, cabecera, pie |
| ![](https://placehold.co/60x24/F5F7F5/F5F7F5.png) | Blanco roto | `#F5F7F5` | Textos y elementos claros |

```css
:root {
  --lima:   #B6FF00;
  --negro:  #080F0E;
  --gris:   #252B2A;
  --blanco: #F5F7F5;
}
```

**Contraste:** el texto en blanco roto sobre negro y gris cumple de sobra. El verde lima sobre negro también. **No** se usará texto blanco sobre fondo verde lima: sobre lima va texto negro.

## Tipografías (Google Fonts)

| Uso | Fuente | Pesos |
|---|---|---|
| Títulos (`h1`–`h3`), menú, botones | **Barlow Condensed** | 600, 700 |
| Texto corrido, tablas, formularios | **Inter** | 400, 500, 600 |

## Banco de imágenes

| Carpeta | Contenido | Formato recomendado |
|---|---|---|
| `logo/` | Escudo (versión color y monocroma) | SVG / PNG |
| `jugadores/` | Una foto por jugador, mismo encuadre | JPG / WebP |
| `equipaciones/` | Cada equipación: frontal, trasera y detalle | JPG / WebP |
| `estadio/` | Exterior, interior, vista aérea | JPG / WebP |
| `noticias/` | Una imagen principal por noticia | JPG / WebP |
| `aficion/` | Gradas, peñas, eventos | JPG / WebP |

Se pueden usar imágenes de bancos libres (Unsplash, Pexels) o generadas con IA, **siempre con atributo `alt` descriptivo**.

---

<div align="center">

[⬅️ Estructura del sitio](02-estructura-del-sitio.md) · [📚 Índice](../README.md#-documentación) · [Páginas y contenidos ➡️](04-paginas.md)

</div>
