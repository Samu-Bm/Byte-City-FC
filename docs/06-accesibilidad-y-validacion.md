# ♿ Accesibilidad y validación

## Estado actual

La página existente es [`../html/index.html`](../html/index.html). Declara `lang="es"` y las imágenes de los escudos tienen texto alternativo descriptivo. La portada tiene encabezados hasta `h4`, enlaces de navegación y estructura semántica básica. No se han aportado resultados de validadores ni capturas, por lo que la validación formal sigue pendiente.

**Accesibilidad**
- [ ] Declarar el idioma correcto (`<html lang="es">`) en las páginas en español.
- [ ] Proporcionar texto `alt` adecuado según la función de cada imagen (descriptivo si aporta información; vacío si es decorativa).
- [ ] Cada campo de formulario con su `<label>` asociado (cuando se implementen formularios).
- [ ] Contraste suficiente entre texto y fondo.
- [ ] Enlaces con texto claro (evitar «pincha aquí»).
- [ ] Navegación completa con teclado y `<title>` único por página.
- [ ] Un enlace *«Saltar al contenido»* al principio de cada página.

**Validación**
- [ ] HTML validado en [validator.w3.org](https://validator.w3.org) sin errores.
- [ ] CSS validado en [jigsaw.w3.org/css-validator](https://jigsaw.w3.org/css-validator/) sin errores.
- [ ] Todos los enlaces internos comprobados.
- [ ] Capturas guardadas en `docs/validacion/`.

---

<div align="center">

[⬅️ Formularios](05-formularios.md) · [📚 Índice](../README.md#-documentación) · [Requisitos ➡️](07-requisitos.md)

</div>
