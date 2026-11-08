# 📝 Formularios e interactividad de datos

Especificación de formularios y captura de datos del sitio web de **Byte City FC**.

> **Nota sobre el alcance:**  
> - La página `pages/hazte-socio.html` es primordialmente una **página estática informativa** donde se presentan las 3 modalidades de cuota, sus costes y ventajas asociadas.
> - La página `pages/contacto.html` centraliza los datos directos (correo electrónico, redes sociales, teléfono, ubicación) acompañados de un disclaimer oficial y un formulario básico de contacto.
> - La tienda `pages/nuestra-piel.html` presenta las 3 equipaciones oficiales y merchandising, permitiendo ver en detalle imágenes, título y descripción de cada producto.

---

## Directrices técnicas de accesibilidad en formularios

Cuando se implementen formularios en el proyecto, deberán cumplir las siguientes pautas estándar de HTML5:

1. Cada campo llevará su `<label for="...">` estrictamente emparejado con el `id` del control.
2. Los campos imprescindibles se marcarán con el atributo booleano `required`.
3. Cada input contendrá atributos `name` y `id` únicos y descriptivos.
4. Las agrupaciones lógicas de campos se estructurarán con `<fieldset>` y `<legend>`.
5. El botón de acción empleará `<button type="submit">`.
6. En un entorno web estático, la validación se realiza mediante los tipos y atributos nativos de HTML5 (`type="email"`, `type="tel"`, `minlength`, `pattern`, etc.).

---

## ✉️ Formulario de contacto — `pages/contacto.html`

Acompañando a los canales directos (correo, teléfono y RRSS) y al disclaimer de la entidad:

| Campo | Etiqueta / Input | Tipo | Obligatorio | Descripción |
|---|---|:---:|:---:|---|
| Nombre completo | `<input>` | `text` | ✅ | Identificación del aficionado o solicitante |
| Correo electrónico | `<input>` | `email` | ✅ | Canal para responder a la consulta |
| Teléfono de contacto | `<input>` | `tel` | ❌ | Opcional para llamadas de atención |
| Motivo / Asunto | `<select>` | Lista | ✅ | Opciones: *Atención al Socio, Tienda, Prensa, General* |
| Mensaje | `<textarea>` | Texto largo | ✅ | Contenido detallado de la consulta |
| Aceptación de política | `<input>` | `checkbox` | ✅ | Conformidad con el aviso legal del club |
| Envío | `<button>` | `submit` | — | Envío del mensaje |

---

## 📬 Formulario de boletín informativo (Newsletter) — `<footer>`

Ubicado en el pie de página de todas las vistas del sitio para captación de seguidores:

| Campo | Etiqueta / Input | Tipo | Obligatorio |
|---|---|:---:|:---:|
| Correo electrónico | `<input>` | `email` | ✅ |
| Consentimiento de novedades | `<input>` | `checkbox` | ✅ |
| Suscribirse | `<button>` | `submit` | — |

---

## 🎟️ Modalidades de Socio (Página estática) — `pages/hazte-socio.html`

A diferencia de un proceso transaccional complejo, esta sección se concibe como una **guía estática** para consultar las 3 opciones disponibles:

| Modalidad | Rango orientativo | Cuota anual | Beneficios incluidos |
|---|---|:---:|---|
| **Cuota Joven / Junior** | Hasta 20 años | 35 € | Carné oficial, bienvenida digital y 10% en tienda |
| **Cuota Adulto** | Aficionado general | 85 € | Carné oficial, prioridad en compra de entradas y 15% en tienda |
| **Cuota Premium / VIP** | Aficionado especial | 160 € | Asiento preferente, carné exclusivo, bufanda y acceso a eventos |

---

<div align="center">

[⬅️ Páginas y contenidos](04-paginas.md) · [📚 Índice](../README.md#-documentación) · [Accesibilidad y validación ➡️](06-accesibilidad-y-validacion.md)

</div>
