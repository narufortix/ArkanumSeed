# Security Policy

## Modelo de seguridad

ArkánumSeed es un archivo HTML autocontenido que opera **completamente offline**. No hay servidor, no hay API, no hay red.

**Lo que protege:**
- Tus seed phrases y claves xpub mientras están almacenadas en el archivo
- Acceso protegido por clave maestra con PBKDF2-SHA256 (600.000 iteraciones)
- Cifrado AES-256-GCM por campo individual + cifrado del blob completo

**Lo que NO protege:**
- Un dispositivo ya comprometido (keylogger, malware)
- Una clave maestra débil o reutilizada
- Pérdida física del archivo sin copia de seguridad
- Ingeniería social

## Uso seguro recomendado

- Úsalo en un dispositivo **sin conexión a internet**
- Usa una **clave maestra única y fuerte** (nunca la misma que usas en otros servicios)
- Guarda **copias de seguridad** del `.svault` en lugares físicos separados
- Verifica el hash SHA-256 del archivo si lo has descargado de una fuente no oficial

## Reporte de vulnerabilidades

Si encuentras una vulnerabilidad de seguridad, **no abras un issue público**.

Contacta directamente por email antes de divulgarlo: juanpr31@gmail.com

Por favor incluye:
- Descripción de la vulnerabilidad
- Pasos para reproducirla
- Impacto potencial estimado

Responderé en un plazo de 72 horas.
