# Inventario de estibas

Artefacto independiente del Entorno THEMENDO (aparte de Seguimiento de Recibo y Paletizado 3D).

- **Página:** https://luismendoza122.github.io/inventario-estibas/
- **Operadores:** abren el enlace que les llega por WhatsApp (`contar.html?t=…`).
- **APK:** "Inventario de estibas" en Mis APK de la Central (se compila desde este repositorio).
- **Entorno THEMENDO:** https://luismendoza122.github.io/app-paletizado-3d/themendo/

## Partes
| Carpeta | Para qué |
|---|---|
| `www/` | Pantallas: panel del administrador (`index.html`), app del operador (`contar.html`), conexión con la nube (`nube.js`) |
| `nube/funcion.js` | La función "inventario" de Supabase en un solo archivo (se genera; no se edita a mano) |
| `scripts/` | Pruebas contra la nube real y en Chrome |

## Cómo entra cada quien
- **Luis:** escribe su correo de la Central y su contraseña. Solo él ve la pestaña **Administradores**.
- **Administradores:** código personal `XXXX-XXXX-XXXX` que crea Luis. Sirve en un solo celular y vence.
- **Operadores:** su enlace, amarrado al primer celular que lo abre.

Los datos viven en la nube (esquema `inventario` de Supabase), no en este repositorio.
