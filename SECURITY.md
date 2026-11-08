# Política de Seguridad y Reporte Responsable (`SECURITY.md`)

En **REMEMBER**, la seguridad y la privacidad de la información académica de nuestros usuarios son prioritarias.

## Versiones Soportadas

| Versión | Estado de Soporte de Seguridad |
| :--- | :--- |
| `0.1.4-beta` (Actual) | ✅ Soportada activamente |
| `< 0.1.4` | ❌ Obsoleta (actualizar a la última versión Beta) |

---

## Cómo Reportar una Vulnerabilidad de Seguridad

> ⚠️ **IMPORTANTE:** Si descubres un fallo de seguridad, **NO abras un Issue público en GitHub**.

Por favor envíanos un reporte privado por correo electrónico a:
- 📧 **[rememberhm.landing123@gmail.com ](mailtorememberhm.landing123@gmail.com)** con el asunto `[SECURITY] Descripción breve del hallazgo`.

### Qué incluir en tu reporte:
1. Versión de REMEMBER y sistema operativo (Windows, Linux o Web).
2. Pasos detallados para reproducir la vulnerabilidad (Prueba de Concepto).
3. Impacto potencial (p. ej. exposición de datos locales, manejo de sesiones OAuth, sincronización).

### Tiempos de Respuesta Comprometidos:
- **Acuse de recibo:** dentro de las primeras **48 horas**.
- **Evaluación y clasificación de severidad:** dentro de **5 días hábiles**.
- **Publicación del parche:** coordinada contigo antes de cualquier divulgación pública.

---

## Modelo de Privacidad y Manejo de Datos

1. **Modo Invitado (100% Local):**
   - Ningún dato abandona tu equipo. Tus tareas, notas, materias y tarjetas se almacenan exclusivamente en la base de datos SQLite local de tu sistema operativo.
2. **Sincronización en la Nube (Opcional):**
   - Solo se activa cuando el usuario inicia sesión explícitamente y autoriza el modo de sincronización en la nube.
   - La comunicación con Supabase se realiza exclusivamente sobre HTTPS/TLS con políticas de seguridad a nivel de fila (*Row Level Security - RLS*) por `user_id`.
3. **Integración con Google Classroom:**
   - Utiliza **OAuth 2.0 con PKCE** y solicita únicamente permisos de **solo lectura** (`classroom.courses.readonly`, `classroom.coursework.me.readonly`, `classroom.announcements.readonly`).
   - REMEMBER nunca modifica, elimina ni entrega tareas en nombre del usuario en Google Classroom.

### Recomendación al reportar Bugs generales:
Cuando abras un Issue público en este repositorio, **nunca adjuntes tu archivo `.db` / `.sqlite` real ni capturas que muestren tokens o información personal sensible**.
