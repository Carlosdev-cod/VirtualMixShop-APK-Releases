# VirtualMixShop APK — Releases

Repositorio **público** de binarios de la app Android de VirtualMixShop.

Aquí solo van los APK y sus notas de versión. El **código fuente vive en un repositorio privado**.

---

## ⚠️ Estado: BETA

Todavía **no hay ninguna release publicada**. La app está en fase de pruebas internas.

Cuando salga la primera versión estable, aparecerá aquí y en la sección
[**Releases**](https://github.com/Carlosdev-cod/VirtualMixShop-APK-Releases/releases).

---

## Cómo se actualizará la app

La APK consulta `GET /api/app/version` al arrancar:

- Si hay una versión más nueva → muestra un aviso con el changelog y un botón **Descargar**.
- Si la versión instalada es más vieja que el mínimo exigido → el aviso es obligatorio.

Ese botón abre la página de Releases en el navegador del teléfono. Desde ahí se
descarga el APK y se instala encima del anterior (los datos se conservan).

---

## Requisitos

| | |
|---|---|
| Android | 8.0 (Oreo, API 26) o superior |
| Permisos | Internet, red, cámara, biometría |
| Huella / Face ID | Opcional, para login sin contraseña |

---

## Seguridad

- Los APK van firmados con el mismo certificado en cada versión: las
  actualizaciones se instalan **encima**, sin perder datos.
- La huella dactilar **nunca sale del teléfono**: solo viaja una firma
  criptográfica, validada contra el dominio.
- No se publican binarios sin firmar.

---

*VirtualMixShop — Cuba*