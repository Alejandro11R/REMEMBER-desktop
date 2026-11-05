<div align="center">

  <img src="assets/logo.png" alt="REMEMBER Logo" width="96" height="96" />

  # REMEMBER

  **Estación de trabajo y estudio personal Local-First ultrarrápida**  
  *Construida con Tauri v2, Rust, SQLite y React.*

  [![Sitio Web](https://img.shields.io/badge/Web-isremember.com-00DC82?style=for-the-badge&logo=googlechrome&logoColor=white)](https://www.isremember.com)
  [![Versión Beta](https://img.shields.io/badge/Versi%C3%B3n-v0.1.3--Beta-8B5CF6?style=for-the-badge)](https://www.isremember.com#waitlist)
  [![Tauri](https://img.shields.io/badge/Tauri-v2.0-FFC131?style=for-the-badge&logo=tauri&logoColor=black)](https://tauri.app)
  [![Rust](https://img.shields.io/badge/Rust-2024-DEA584?style=for-the-badge&logo=rust&logoColor=black)](https://www.rust-lang.org)
  [![SQLite](https://img.shields.io/badge/SQLite-WAL%20Mode-003B57?style=for-the-badge&logo=sqlite&logoColor=white)](https://sqlite.org)
  [![Licencia](https://img.shields.io/badge/Licencia-Proprietary%20%2F%20Public%20Satellite-gray?style=for-the-badge)](https://www.isremember.com/terms)

  <br />

  [**Sitio Web Oficial**](https://www.isremember.com) • [**Solicitar Acceso a la Beta**](https://www.isremember.com#waitlist) • [**Reportar un Error (Issues)**](https://github.com/Alejandro11R/REMEMBER-desktop/issues) • [**Política de Privacidad**](https://www.isremember.com/privacy)

</div>

---

## ⚡ Filosofía Anti-Bloat & Local-First

Las aplicaciones modernas de productividad y estudio sufren de una epidemia silenciosa: **bloatware, sobrecarga de memoria RAM y dependencia permanente de servidores remotos**. Tiempos de carga interminables, spinners bloqueantes y suscripciones forzadas para guardar simples notas de texto.

**REMEMBER** fue diseñada desde los cimientos como una respuesta radical:

- 🏎️ **Cero Latencia de Red:** La base de datos SQLite vive en tu propio disco SSD, operando en modo *Write-Ahead Logging* (WAL). Cada consulta y escritura se ejecuta en microsegundos, sin importar si estás en un avión sin WiFi o en el campus universitario.
- 🪶 **Consumo Mínimo de Recursos:** Gracias a la arquitectura nativa de **Tauri v2 + Rust**, REMEMBER consume entre **35 MB y 60 MB de memoria RAM**, frente a los 600 MB a 1.5 GB de las alternativas basadas en Electron.
- 🔒 **100% Privado y Offline:** Tus apuntes, exámenes, proyectos y tarjetas de repaso nunca abandonan tu máquina. No existen rastreadores publicitarios ni telemetría invasiva.
- ⌨️ **Diseñada para el Flujo Continuo:** Navegación ultrarrápida mediante teclado y Command Palette global (`⌘K` / `Ctrl+K`).

---

## 📸 Capturas de Pantalla

<div align="center">
  <img src="assets/screenshots/notes.png" alt="Editor de Notas Markdown de REMEMBER" width="850" />
  <p><em>Editor Markdown híbrido con conversión directa de apuntes a tareas accionables.</em></p>
</div>

<br />

<div align="center">
  <img src="assets/screenshots/flashcards.png" alt="Repaso Espaciado con Algoritmo SM-2 en REMEMBER" width="850" />
  <p><em>Módulo de Flashcards con algoritmo científico de repetición espaciada SuperMemo SM-2.</em></p>
</div>

<br />

<div align="center">
  <img src="assets/screenshots/classroom.png" alt="Sincronización con Google Classroom en REMEMBER" width="850" />
  <p><em>Integración directa y segura con Google Classroom: cursos, tareas y fechas de entrega en un solo panel.</em></p>
</div>

---

## 🧠 Características Principales

### 1. 📝 Notas Markdown & Tareas Unificadas
Olvídate de copiar y pegar pendientes de tus notas a otra app de to-do. En REMEMBER, cualquier elemento o apunte se transforma con un atajo en una tarea con fecha de vencimiento que viaja automáticamente a tu tablero de hoy.

### 2. 📚 Algoritmo de Repaso Espaciado SM-2
Aprende y retén información de manera eficiente. Las tarjetas de estudio utilizan la variante optimizada del algoritmo **SuperMemo SM-2**, calculando los intervalos ideales de repetición (factor de facilidad $EF$, intervalos y calidad de respuesta) para maximizar la memoria a largo plazo antes de tus exámenes o entregas.

### 3. 🎓 Sincronización Oficial con Google Classroom
Conexión directa vía Google OAuth con permisos estrictamente limitados de lectura. Descarga automáticamente tus materias, tareas pendientes y materiales de clase directamente a tu almacenamiento local, garantizando que nunca pierdas una fecha límite.

### 4. ⏱️ Temporizador Pomodoro & Paisajes Sonoros
Entrena tu capacidad de hiperfoco con ciclos de trabajo profundo personalizables y sonidos ambientales relajantes (lluvia, ruido blanco, cafetería) ejecutados nativamente sin consumo innecesario de CPU.

### 5. 🗂️ Calendario & Gestor de Proyectos
Visualiza tu carga semanal y mensual. Planifica bloques de tiempo (time blocking), vincula proyectos y visualiza los hitos académicos y laborales en una interfaz limpia con temas oscuros de alto contraste.

---

## 💻 Plataformas Soportadas

| Sistema Operativo | Formato del Paquete | Estado |
| :--- | :--- | :--- |
| **Windows 10 / 11** | Instalador x64 (`.msi` / `.exe`) | 🟢 Beta Disponible |
| **Linux** | Paquetes nativos (`.deb` / `.AppImage`) | 🟢 Beta Disponible |
| **macOS** | Universal (`.dmg` Apple Silicon & Intel) | 🟡 En Preparación |

> 📥 **¿Cómo probar la versión preliminar?**  
> Regístrate con tu correo electrónico en [isremember.com](https://www.isremember.com#waitlist) para recibir el enlace de descarga e instrucciones de instalación.

---

## 🛠️ Stack Tecnológico

- **Core & Backend Nativo:** [Rust](https://www.rust-lang.org/) + [Tauri v2](https://tauri.app/)
- **Almacenamiento Local:** [SQLite](https://sqlite.org/) con modo WAL (Write-Ahead Logging)
- **Frontend & UI:** [React](https://react.dev/), [TypeScript](https://www.typescriptlang.org/), [Tailwind CSS](https://tailwindcss.com/)
- **Protocolos de Integración:** Google Classroom REST API v1 (OAuth 2.0 PKCE)
- **Algoritmo de Aprendizaje:** SuperMemo SM-2 Spaced Repetition Engine

---

## 🛡️ Propósito de este Repositorio Satélite

Este repositorio público actúa como el **canal comunitario oficial** de **REMEMBER**:

1. **Rastreador de Problemas (Bug Tracker):** Si experimentas un fallo o comportamiento inesperado, puedes abrir un [Issue en GitHub](https://github.com/Alejandro11R/REMEMBER-desktop/issues).
2. **Solicitud de Funciones (Feature Requests):** Propón nuevas ideas y mejoras que te gustaría ver en las próximas versiones.
3. **Registro de Cambios (Changelog) & Releases:** Consulta las notas de actualización de cada versión Beta.
4. **Seguridad y Auditoría:** Consulta nuestras políticas de reporte responsable y manejo de datos.

> 🔒 *Nota:* El código fuente del motor de la aplicación se mantiene en un repositorio privado propiedad de los desarrolladores. Este repositorio satélite no contiene el código de compilación del núcleo propietario, garantizando la seguridad del software y permitiendo al mismo tiempo la colaboración y retroalimentación transparente de la comunidad.

---

## 👥 Equipo & Creadores

Desarrollado con pasión por:

- **Hugo Alejandro Rodriguez** ([@Alejandro11R](https://github.com/Alejandro11R)) — Fundador & Arquitectura Core
- **TheBrake** ([@TheBrake](https://github.com/TheBrake)) — Co-Fundador & Diseño de Producto

---

## 📬 Contacto & Enlaces

- **Web:** [https://www.isremember.com](https://www.isremember.com)
- **Email:** [hola@isremember.com](mailto:hola@isremember.com)
- **Privacidad:** [https://www.isremember.com/privacy](https://www.isremember.com/privacy)
- **Términos:** [https://www.isremember.com/terms](https://www.isremember.com/terms)

<div align="center">
  <br />
  <sub>Hecho para quienes valoran la velocidad, la concentración y la privacidad de su información.</sub>
</div>
