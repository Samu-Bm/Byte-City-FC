# 🎨 Guía de estilo

> La paleta y las tipografías de este documento son la identidad visual **propuesta**. Aún no se han aplicado en CSS. La lista de recursos gráficos refleja el contenido disponible actualmente.

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

| Carpeta | Contenido disponible | Estado |
|---|---|---|
| `img/escudo/` | `Escudo.svg` y `Escudo-Sin-Fondo.png` | Disponible |
| `img/codeunitedfc/` | Escudo de Code United FC, rival mostrado en el próximo partido | Disponible |
| `img/equipaciones/Primera equipacion/` | Tres imágenes de la primera equipación | Disponible |
| `img/equipaciones/Segunda equipacion/` | Tres imágenes de la segunda equipación | Disponible |
| `img/equipaciones/Tercera equipacion/` | Tres imágenes de la tercera equipación | Disponible |
| `img/ropa/` | Balón, bufanda, gorra, sudadera, chándal y ropa de entrenamiento | Disponible |
| `img/logo/`, `img/jugadores/`, `img/estadio/`, `img/noticias/`, `img/aficion/` | Sin imágenes todavía; se conservan con `.gitkeep` | Pendiente |

La portada usa los dos escudos para identificar a los equipos del próximo partido. Las futuras imágenes deberán tener procedencia adecuada y texto `alt` descriptivo cuando aporten información. Los nombres de archivo y las subcarpetas de equipaciones contienen espacios y deben referenciarse respetando exactamente su ruta.

---

<div align="center">

[⬅️ Estructura del sitio](02-estructura-del-sitio.md) · [📚 Índice](../README.md#-documentación) · [Páginas y contenidos ➡️](04-paginas.md)

</div>
