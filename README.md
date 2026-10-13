# ciberseguridad-vulnerabilidadesWEB-demo
# Laboratorio de Vulnerabilidades Web

Este repositorio contiene demostraciones prácticas de vulnerabilidades web basadas en OWASP Top 10.

El objetivo es mostrar:

- Código vulnerable.
- Explotación de la vulnerabilidad.
- Código corregido.
- Explicación de la mitigación.

## Vulnerabilidades incluidas

### Broken Access Control (A01:2021)

Demostración en la que un usuario puede acceder a la información de otro modificando un identificador en la URL.

#### Escenario vulnerable

- Inicio de sesión como usuario legítimo.
- Modificación manual del parámetro `id`.
- Acceso a recursos no autorizados.

#### Mitigación

- Validación explícita de autorización.
- Verificación de que el recurso solicitado pertenece al usuario autenticado.

---

### Cross-Site Scripting - XSS (A03:2021 Injection)

Demostración de una vulnerabilidad XSS basada en la inserción de contenido controlado por el usuario utilizando `innerHTML`.

#### Escenario vulnerable

- Introducción de una carga XSS.
- Ejecución de JavaScript en el navegador de la víctima.

#### Mitigación

- Uso de `textContent`.
- Aplicación de políticas CSP (Content Security Policy).

---

