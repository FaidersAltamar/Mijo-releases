# Mijo — Descargas

**Mijo** es una interfaz visual para trabajar con agentes de IA en tus proyectos de código: chat, diffs, terminal integrado, permisos, skills, túneles remotos y más. Disponible como **app de escritorio** (macOS y Windows), **navegador/PWA** y **extensión de VS Code**.

Este repositorio es **solo para instaladores y actualizaciones**. No contiene el código fuente de la aplicación.

---

## Descargar la última versión

👉 **[Ver todas las versiones (Releases)](https://github.com/FaidersAltamar/Mijo-releases/releases/latest)**

| Plataforma | Archivo recomendado | Notas |
|------------|---------------------|-------|
| **macOS (Apple Silicon)** | `Mijo-*-mac-arm64.pkg` | Instalador estándar (recomendado) |
| **macOS (Apple Silicon)** | `Mijo-*-mac-arm64.dmg` | Arrastra a Aplicaciones (alternativa) |
| **macOS (Intel)** | `Mijo-*-mac-x64.pkg` / `.dmg` | Si está publicado en Releases |
| **Windows (64 bits)** | `Mijo-*-win-x64.exe` | La mayoría de PCs con Windows |
| **Windows (ARM)** | `Mijo-*-win-arm64.exe` | Surface / PCs con Snapdragon |

También hay archivos `.zip` por si prefieres descomprimir manualmente.

---

## Instalación en macOS (recomendada: `.pkg`)

1. Descarga `Mijo-*-mac-arm64.pkg` desde [Releases](https://github.com/FaidersAltamar/Mijo-releases/releases/latest).
2. Abre el archivo `.pkg`.
3. Sigue el asistente de instalación (Siguiente → Instalar).
4. Si macOS pregunta si confías en el instalador, elige **Abrir** o **Continuar**.
5. Abre **Mijo** desde Aplicaciones.

El instalador `.pkg` copia la app a **Aplicaciones** y quita el bloqueo de descarga de internet automáticamente.

### Alternativa: archivo `.dmg`

1. Abre el `.dmg`.
2. **Arrastra el icono de Mijo a la carpeta Aplicaciones** (como cualquier app de Mac).
3. La primera vez, si macOS bloquea la app: clic derecho en **Mijo** → **Abrir** → **Abrir**.

No hace falta ningún script ni archivo de texto adicional dentro del DMG.

---

## Instalación en Windows

1. Descarga `Mijo-*-win-x64.exe` (o `win-arm64.exe` en PCs ARM).
2. Ejecuta el instalador.
3. Si SmartScreen advierte que Windows protegió tu PC, elige **Más información** → **Ejecutar de todas formas** (build sin firma de código de Microsoft).

La app se instala para el usuario actual (no requiere administrador).

---

## Actualizaciones automáticas

La app de escritorio comprueba nuevas versiones en **este repositorio** (`Mijo-releases`).

- En Mijo: menú o ajustes → **Buscar actualizaciones**.
- En macOS sin certificado de Apple, la app puede pedirte **descargar el instalador `.pkg`** manualmente. Usa el enlace del diálogo o vuelve a esta página.

---

## ¿Qué incluye Mijo?

- Chat con agentes de IA y línea de tiempo (deshacer / rehacer / ramas).
- Vista de diffs, archivos y permisos con interfaces claras.
- Terminal integrado por proyecto.
- Dictado por voz y lectura en voz alta.
- Multi-agente con worktrees aislados.
- Flujos Git y GitHub (commits, PRs, issues).
- Catálogo de skills y automatizaciones reutilizables.
- **Escritorio:** Mini Chat flotante, varias ventanas, notificaciones nativas, túneles, SSH remoto.
- **Web/PWA:** acceso desde el móvil o navegador con túnel.
- **VS Code:** extensión con el mismo motor.

---

## Soporte, errores y sugerencias

El código fuente de Mijo es privado. Para reportar problemas o pedir ayuda con los instaladores:

👉 **[Abrir un issue en este repositorio](https://github.com/FaidersAltamar/Mijo-releases/issues)**

Indica tu sistema (macOS/Windows, versión de Mijo, chip Intel o Apple Silicon) y qué pasos seguiste.

---

## Sobre este repositorio

| Repositorio | Contenido |
|-------------|-----------|
| **Mijo-releases** (este, público) | `.pkg`, `.dmg`, `.exe`, `.zip`, manifiestos de auto-actualización |
| **Mijo** (privado) | Código fuente y desarrollo |

Los instaladores se generan y publican automáticamente al lanzar una nueva versión.

---

## English (short)

**[Download latest release](https://github.com/FaidersAltamar/Mijo-releases/releases/latest)** — Desktop installers for macOS and Windows. This repo has **binaries only**, no source code.

**macOS:** Prefer the **`.pkg`** installer (standard wizard). Alternatively, open the **`.dmg`** and drag Mijo to Applications; if blocked, right-click → Open once.

**Windows:** Run the `.exe` installer; use “Run anyway” if SmartScreen blocks an unsigned build.

**Updates:** The desktop app checks this repo for new versions. **[Report issues here](https://github.com/FaidersAltamar/Mijo-releases/issues).**
