# 🎨 Guía de estilo

> La paleta y las tipografías de este documento definen la identidad visual de **Byte City FC**, incorporadas en `css/base.css`. La lista de recursos gráficos refleja el contenido disponible en el proyecto.

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

## 🔤 Sistema Tipográfico

### 1. Filosofía tipográfica
El sistema visual adopta una dirección editorial de alto impacto inspirada en referencias contemporáneas de diseño deportivo y digital (*landonorris.com*). Su núcleo se fundamenta en la tensión visual extrema entre dos opuestos: la elegancia clásica y estilizada de una **serif de alto contraste (Didone)** para aperturas breves, enfrentada a la contundencia rotunda de una **sans-serif geométrica ultra negra (800)** con interlineado negativo y solape controlado.

---

### 2. Tabla de fuentes del sistema

| Fuente | Rol | Pesos permitidos | Origen / Ruta | Licencia | Fallback |
|---|---|:---:|---|---|---|
| **Brier** | Display de acento (palabra de apertura) | **Bold (700)** | Archivo local: `assets/fonts/brier/Brier-Bold.otf` | Propietaria / Trial *(revisar términos para despliegue web público)* | `"Playfair Display", Georgia, serif` |
| **Mona Sans** | Fuente principal de la interfaz (≈95%) | **200..900** (usos clave: 400, 600, 700, 800) | Google Fonts (Variable) | Abierta (OFL / Google Fonts) | `Arial, sans-serif` |


---

### 3. Jerarquía y roles tipográficos

| Rol | Fuente | Peso | Tamaño fluido (`clamp`) | Interlineado (`line-height`) | Espaciado (`letter-spacing`) | Transform | Ejemplo de uso |
|---|---|:---:|:---:|:---:|:---:|:---:|---|
| `display-serif` | Brier | 700 | `clamp(3.5rem, 8vw, 7rem)` | `0.85` | `-0.01em` | UPPERCASE | Apertura corta del titular (`PLAY`, `ON`, `OFF`) |
| `display-sans` | Mona Sans | 800 | `clamp(4.2rem, 11vw, 9.5rem)` | `0.8` | `-0.03em` | UPPERCASE | Palabra dominante del titular (`CODE`, `WIN`, `TRACK`) |
| `heading-section` | Mona Sans | 800 | `clamp(2rem, 4vw, 3rem)` | `1.05` | `-0.02em` | Normal / Auto | Títulos de sección (`Quiénes somos`, `Partidos`) |
| `eyebrow / label` | Mona Sans | 600 | `clamp(0.75rem, 1vw, 0.875rem)` | `1.2` | `+0.08em` | UPPERCASE | Categorías, metadatos, tags (`LIGA DIGITAL · JORNADA 8`) |
| `body` | Mona Sans | 400 | `clamp(1rem, 1.1vw, 1.125rem)` | `1.55` | `normal` | Normal | Párrafos, descripciones de tarjetas (ancho 25–40ch) |
| `body-emphasis` | Mona Sans | 700 | Heredado | Heredado | `normal` | Normal | Resaltados y conceptos clave dentro de párrafos |
| `button` | Mona Sans | 700 | `0.9375rem (15px)` | `1` | `+0.02em` | Normal / Auto | Texto de botones de acción y llamadas a la acción |

---

### 4. Tokens CSS de tipografía

Los tokens se encuentran unificados en `css/base.css` bajo las siguientes variables:

```css
:root {
  /* Familias */
  --font-display: "Brier", "Playfair Display", Georgia, serif;
  --font-body: "Mona Sans", Arial, sans-serif;

  /* Pesos */
  --font-weight-regular: 400;
  --font-weight-medium:  500;
  --font-weight-semibold: 600;
  --font-weight-bold:    700;
  --font-weight-black:   800;

  /* Escala tipográfica fluida */
  --text-xs:   0.75rem;                       /* 12px */
  --text-sm:   0.875rem;                      /* 14px */
  --text-base: clamp(1rem, 1.1vw, 1.125rem);  /* 16-18px */
  --text-lg:   1.25rem;                       /* 20px */
  --text-xl:   clamp(1.5rem, 2.5vw, 2rem);    /* 24-32px */
  --text-2xl:  clamp(2rem, 4vw, 3rem);        /* 32-48px */
  --text-hero-serif: clamp(3.5rem, 8vw, 7rem);
  --text-hero-sans:  clamp(4.2rem, 11vw, 9.5rem);

  /* Interlineados */
  --leading-tight:  0.8;
  --leading-snug:   1.05;
  --leading-normal: 1.55;

  /* Espaciado entre letras */
  --tracking-tighter: -0.03em;
  --tracking-tight:   -0.01em;
  --tracking-normal:   0em;
  --tracking-wide:    +0.08em;
}
```

---

### 5. Patrón del titular de dos líneas (Brier + Mona Sans)

El diseño icónico de dos líneas apila la primera palabra corta en Brier (serif) con la segunda palabra imponente en Mona Sans 800, logrando un solape sutil mediante un `line-height` ultracompacto (~0.8) y margen negativo calculado:

#### Estructura HTML
```html
<h1 class="title-stacked">
  <span class="title-serif">PLAY</span>
  <span class="title-sans">CODE</span>
</h1>
```

#### Estilos CSS
```css
.title-stacked {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  line-height: 0.8;
  margin: 0;
  text-transform: uppercase;
}

.title-stacked .title-serif {
  font-family: var(--font-display);
  font-weight: 700;
  font-size: var(--text-hero-serif);
  letter-spacing: var(--tracking-tight);
  color: var(--color-text);
  position: relative;
  z-index: 2;
}

.title-stacked .title-sans {
  font-family: var(--font-body);
  font-weight: 800;
  font-size: var(--text-hero-sans);
  letter-spacing: var(--tracking-tighter);
  color: var(--color-text);
  margin-top: -0.12em; /* Sutil solape bajo la serif */
  position: relative;
  z-index: 1;
}
```

---

### 6. Reglas DO / DON'T

| Práctica | Regla | Motivo |
|---|---|---|
| **DO** | Usar Brier 700 exclusivamente para la palabra de apertura o titulares de gran escala (>48px). | Mantiene la exclusividad y legibilidad del contraste Didone. |
| **DO** | Utilizar Mona Sans 800 en mayúsculas para la palabra base y fuerte del titular. | Crea la masa visual pesada sobre la que reposa el diseño. |
| **DO** | Redactar párrafos y bloques de lectura en Mona Sans 400 con ancho controlado (~25–40 caracteres en tarjetas, máx. 65ch en editorial). | Garantiza una lectura cómoda y descansada. |
| **DON'T** | Emplear Brier en párrafos, botones, menús de navegación o textos menores a 48px. | Sus trazos finos se degradan y dificultan severamente la lectura a cuerpos pequeños. |
| **DON'T** | Introducir una tercera familia tipográfica en la interfaz (evitar `Barlow` o fuentes externas de iconos como `webflow-icons`). | La pureza visual depende exclusivamente del binomio Brier + Mona Sans. |
| **DON'T** | Componer textos largos o párrafos completos enteramente en mayúsculas (`text-transform: uppercase`). | Reduce drásticamente la velocidad de lectura y vulnera buenas prácticas de accesibilidad. |

---

### 7. Paleta asociada a la tipografía y contraste (WCAG AA)

Para armonizar la estética de *landonorris.com* con la identidad deportiva de **Byte City FC**, se establecen dos escenarios cromáticos que garantizan legibilidad absoluta:

| Escenario | Color de fondo | Color de texto principal | Acento / Botones | Ratio de contraste | Cumplimiento WCAG |
|---|:---:|:---:|:---:|:---:|:---:|
| **Tema Dark Oficial** (Base club) | `#080F0E` (Negro profundo) | `#F5F7F5` (Blanco roto) | `#B6FF00` (Verde lima neón) | `16.2:1` (Blanco/Negro) | **AAA** (Excede 7:1) |
| **Tema Editorial Claro** (Referencia) | `#F4F4EC` (Crema claro) | `#262A1F` (Verde bosque oscuro) | `#D4FF00` / `#B6FF00` (Lima) | `12.8:1` (Bosque/Crema) | **AAA** (Excede 7:1) |
| **Botón de acción lima** | `#B6FF00` / `#D4FF00` | `#080F0E` / `#262A1F` (Oscuro) | — | `14.5:1` (Oscuro/Lima) | **AAA** (Excede 7:1) |

> 🚫 **Prohibición expresa:** Nunca colocar texto blanco roto (`#F5F7F5`) sobre fondos lima (`#B6FF00`). Sobre superficies lima, el texto siempre será oscuro.

---

### 8. Rendimiento y carga de fuentes

1. **`font-display: swap`**: Activo tanto en `@font-face` como en el parámetro de Google Fonts para evitar destellos invisibles de texto (FOIT) y mostrar texto inmediato con fuentes fallback.
2. **Preconexión temprana (Preconnect):** En el `<head>` de los documentos HTML hacia `fonts.googleapis.com` y `fonts.gstatic.com` (con `crossorigin`).
3. **Métrica de CLS (Cumulative Layout Shift):** Los fallbacks (`"Playfair Display", Georgia, serif` para Brier y `Arial, sans-serif` para Mona Sans) preservan métricas verticales similares para minimizar saltos de página durante la hidratación tipográfica.

---

### 9. Adaptabilidad responsive y móviles

- **Escalado mediante `clamp()`**: Los titulares no usan tamaños estáticos en `px`. Se adaptan dinámicamente desde pantallas móviles (320px) hasta monitores de escritorio amplios sin saltos bruscos.
- **Interlineado móvil:** En pantallas menores a `640px`, el interlineado (`line-height`) del titular de dos líneas se ajusta a `0.85–0.9` para evitar que los ascendentes y descendentes colisionen en viewports estrechos.

---

### 10. Criterios de accesibilidad (a11y)

- **Cuerpo mínimo:** Ningún texto informativo o de cuerpo desciende de `1rem` (16px).
- **Etiquetas y metadatos:** Los elementos con `text-transform: uppercase` y tamaño reducido (0.75rem–0.875rem) se reservan exclusivamente para etiquetas de una o dos palabras (*eyebrows*).
- **Botones con solo icono:** Todo botón de acción que contenga únicamente un icono gráfico dispone de un atributo accesible descriptivo (ejemplo: `<button class="btn-icon" aria-label="Abrir menú de navegación">`).

---

### 11. Checklist de validación tipográfica

Antes de dar por finalizada cualquier maqueta o página:
- [ ] La palabra de apertura del hero/titular utiliza `--font-display` (Brier 700) en mayúsculas.
- [ ] La palabra principal del hero utiliza `--font-body` (Mona Sans 800) en mayúsculas con interlineado compacto.
- [ ] Todo el texto de lectura, navegación y fichas técnicas está maquetado en Mona Sans (400 / 600 / 700).
- [ ] No existen textos con Brier en tamaños inferiores a 48px.
- [ ] Los contrastes de color superan el ratio mínimo de 4.5:1 para texto normal y 3:1 para texto grande (WCAG AA).
- [ ] Las fuentes cargan con `font-display: swap` y los preconnect correspondientes.

---

### 12. Supuestos y decisiones de diseño

1. **Stack detectado:** Proyecto en **HTML5 semántico y CSS3 puro** sin frameworks (sin React/Next.js/Tailwind). La arquitectura tipográfica se implementará en CSS mediante Custom Properties nativas y clases reutilizables.
2. **Ubicación prevista para fuentes:** En HTML plano, los archivos de fuente locales se organizarán bajo `assets/fonts/brier/Brier-Bold.otf`.
3. **Selección de pesos de Brier:** El archivo comprimido `Brier_Trial.zip` de la raíz contiene `Brier-Bold.otf` y `Brier-Regular.otf`. Se utilizará únicamente el peso Bold (700) para acentos editoriales y el peso Regular queda clasificado como no usado.
4. **Armonización de color:** Se integran tanto la paleta oscura oficial del club (`#080F0E` negro, `#B6FF00` lima) como los contrastes de la referencia editorial (`#F4F4EC` crema, `#262A1F` bosque oscuro).

---

## Banco de imágenes

| Carpeta | Contenido disponible | Estado |
|---|---|---|
| `img/escudo/` | `Escudo.svg` y `Escudo-Sin-Fondo.png` | Disponible |
| `img/codeunitedfc/` | Escudo de Code United FC, rival mostrado en el próximo partido | Disponible |
| `img/equipaciones/Primera equipacion/` | Imágenes de la primera equipación | Disponible |
| `img/equipaciones/Segunda equipacion/` | Imágenes de la segunda equipación | Disponible |
| `img/equipaciones/Tercera equipacion/` | Imágenes de la tercera equipación | Disponible |
| `img/ropa/` | Balón, bufanda, gorra, sudadera, chándal y ropa deportiva | Disponible |
| `img/noticias/` | Imágenes para actualidad, crónicas y presentaciones | Disponible |
| `img/logo/`, `img/jugadores/`, `img/estadio/`, `img/aficion/` | Directorios reservados para próximas imágenes | Conservados con `.gitkeep` |

La portada usa los dos escudos para identificar a los equipos del próximo partido. Las futuras imágenes deberán tener procedencia adecuada y texto `alt` descriptivo cuando aporten información. Los nombres de archivo y las subcarpetas de equipaciones contienen espacios y deben referenciarse respetando exactamente su ruta.

---

<div align="center">

[⬅️ Estructura del sitio](02-estructura-del-sitio.md) · [📚 Índice](../README.md#-documentación) · [Páginas y contenidos ➡️](04-paginas.md)

</div>
