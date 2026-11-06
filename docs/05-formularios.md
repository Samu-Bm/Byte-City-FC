# 📝 Formularios

Se proponen **cuatro formularios** para futuras páginas. Ninguno está implementado: la portada actual no contiene formularios y las páginas previstas para alojarlos aún no existen. Las siguientes tablas son especificaciones, no una descripción de formularios funcionales.

Cuando se implementen, todos deberán cumplir estas reglas:

- Cada campo tiene su `<label for="...">` vinculado al `id` del input.
- Los campos obligatorios llevan el atributo `required`.
- Cada input lleva `name` y `id` únicos.
- Los campos relacionados se agrupan con `<fieldset>` y `<legend>`.
- El envío se hace con `<button type="submit">`.
- El destino y el tratamiento del envío deberán definirse al implementar cada formulario; una página estática por sí sola no procesa ni almacena solicitudes.

| Formulario | Página | Objetivo |
|---|---|---|
| Inscripción de socio | `hazte-socio.html` | Hacerse socio |
| Contacto | `contacto.html` | Consultas al club |
| Pedido simulado | `nuestra-piel.html` | Comprar equipaciones (ficticio) |
| Boletín | Pie de todas las páginas | Recibir novedades |

---

## 🎟️ Formulario de inscripción de socio

| Grupo (`fieldset`) | Campo | Tipo de input | Obligatorio |
|---|---|---|:---:|
| Datos personales | Nombre | `text` | ✅ |
| Datos personales | Apellidos | `text` | ✅ |
| Datos personales | Correo electrónico | `email` | ✅ |
| Datos personales | Teléfono | `tel` | ❌ |
| Datos personales | Fecha de nacimiento | `date` | ✅ |
| Datos personales | Provincia | `select` | ✅ |
| Cuenta | Usuario | `text` | ✅ |
| Cuenta | Contraseña | `password` | ✅ |
| Cuenta | Foto para el carné | `file` | ❌ |
| Modalidad | Modalidad de socio (Junior / Joven / Adulto / Premium) | `radio` | ✅ |
| Modalidad | Nº de acompañantes | `number` | ❌ |
| Preferencias | ¿Cómo nos conociste? | `textarea` | ❌ |
| Preferencias | Quiero recibir novedades por email | `checkbox` | ❌ |
| Preferencias | Acepto las condiciones y la política de privacidad | `checkbox` | ✅ |
| — | Enviar solicitud | `<button type="submit">` | — |

> Si en clase se han visto otros tipos de input (`range`, `url`, `color`...), se pueden sustituir o añadir.

---

## ✉️ Formulario de contacto

| Campo | Tipo de input | Obligatorio |
|---|---|:---:|
| Nombre | `text` | ✅ |
| Correo electrónico | `email` | ✅ |
| Teléfono | `tel` | ❌ |
| Asunto (Socios / Tienda / Prensa / Otros) | `select` | ✅ |
| Mensaje | `textarea` | ✅ |
| Acepto la política de privacidad | `checkbox` | ✅ |
| Enviar mensaje | `<button type="submit">` | — |

---

## 👕 Formulario de pedido (simulado)

| Campo | Tipo de input | Obligatorio |
|---|---|:---:|
| Producto | `select` | ✅ |
| Talla (S / M / L / XL) | `radio` | ✅ |
| Cantidad | `number` (`min`, `max`) | ✅ |
| Nombre para la camiseta | `text` | ❌ |
| Dorsal | `number` | ❌ |
| Correo electrónico | `email` | ✅ |
| Envío exprés | `checkbox` | ❌ |
| Comprar | `<button type="submit">` | — |

---

## 📬 Formulario de boletín

Incluido en el `<footer>` de **todas** las páginas.

| Campo | Tipo de input | Obligatorio |
|---|---|:---:|
| Correo electrónico | `email` | ✅ |
| Acepto recibir novedades | `checkbox` | ✅ |
| Suscribirme | `<button type="submit">` | — |

---

<div align="center">

[⬅️ Páginas y contenidos](04-paginas.md) · [📚 Índice](../README.md#-documentación) · [Accesibilidad y validación ➡️](06-accesibilidad-y-validacion.md)

</div>
