# Mijo — Descargas

**Mijo** es una interfaz visual para trabajar con agentes de IA en tus proyectos de código: chat, diffs, terminal integrado, permisos, skills, túneles remotos y más. Disponible como **app de escritorio** (macOS y Windows), **navegador/PWA** y **extensión de VS Code**.

Este repositorio es **solo para instaladores y actualizaciones**. No contiene el código fuente de la aplicación.

---

## Descargar la última versión

👉 **[Ver todas las versiones (Releases)](https://github.com/FaidersAltamar/Mijo-releases/releases/latest)** — actualmente **v1.13.60** (macOS + Windows)

| Plataforma | Archivo recomendado | Notas |
|------------|---------------------|-------|
| **macOS (Apple Silicon)** | `Mijo-*-mac-arm64.dmg` | Abre el DMG → doble clic en **`Instalar Mijo.terminal`** |
| **macOS (Apple Silicon)** | `Mijo-*-mac-arm64.pkg` | Alternativa: asistente estándar (ver abajo si macOS bloquea) |
| **macOS (Intel)** | `Mijo-*-mac-x64.pkg` / `.dmg` | Si está publicado en Releases |
| **Windows (64 bits)** | `Mijo-*-win-x64.exe` | **Usa v1.13.19 o superior** (versiones anteriores rotas) |
| **Windows (ARM)** | `Mijo-*-win-arm64.exe` | Surface / PCs con Snapdragon |

También hay archivos `.zip` por si prefieres descomprimir manualmente.

---

## Instalación en macOS (recomendada: `.dmg`)

1. Descarga `Mijo-*-mac-arm64.dmg` desde [Releases](https://github.com/FaidersAltamar/Mijo-releases/releases/latest).
2. Abre el archivo `.dmg`.
3. Haz **doble clic** en **`Instalar Mijo.terminal`** (se abre Terminal).
4. Pulsa **Instalar** en el diálogo y escribe tu contraseña de Mac si la pide.
5. Mijo se instala en **Aplicaciones** y se abre solo.

Este método evita el bloqueo de macOS (*"Apple no pudo verificar…"*) que aparece con scripts `.command` o `.pkg` sin certificado Apple.

### Alternativa: archivo `.pkg`

1. Descarga `Mijo-*-mac-arm64.pkg`.
2. Si macOS bloquea al abrirlo, pega en **Terminal**:

   ```bash
   xattr -cr ~/Downloads/Mijo-*-mac-arm64.pkg
   open ~/Downloads/Mijo-*-mac-arm64.pkg
   ```

3. Sigue el asistente (Siguiente → Instalar) y abre Mijo desde Aplicaciones.

### Instalación en Terminal (sin contraseña)

```bash
curl -fsSL https://mijocode.com/install | bash
```

Si ya descargaste el `.dmg` en Descargas:

```bash
curl -fsSL https://github.com/FaidersAltamar/Mijo-releases/releases/latest/download/install-mijo-from-downloads.sh | bash
```

---

## Instalación en Windows

1. Descarga `Mijo-*-win-x64.exe` (o `win-arm64.exe` en PCs ARM).
2. Ejecuta el instalador.
3. Si SmartScreen advierte que Windows protegió tu PC, elige **Más información** → **Ejecutar de todas formas** (build sin firma de código de Microsoft).

La app se instala para el usuario actual (no requiere administrador).

### PowerShell (recomendado)

```powershell
irm https://mijocode.com/install.ps1 | iex
```

---

## Actualizaciones automáticas

La app de escritorio comprueba nuevas versiones en **este repositorio** (`Mijo-releases`).

- En Mijo: menú o ajustes → **Buscar actualizaciones**.
- En macOS sin certificado de Apple, la app puede pedirte **descargar el instalador** manualmente. Usa el enlace del diálogo o vuelve a esta página.

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

👉 **Abrir un issue en este repositorio**

Indica tu sistema (macOS/Windows, versión de Mijo, chip Intel o Apple Silicon) y qué pasos seguiste.

---

## Sobre este repositorio

| Repositorio | Contenido |
|-------------|-----------|
| **Mijo-releases** (este, público) | `.pkg`, `.dmg`, `.exe`, `.zip`, manifiestos de auto-actualización |
| **Mijo** (privado) | Código fuente y desarrollo |

Los instaladores se generan y publican al lanzar una nueva versión.

---

## English (short)

**Download latest release** — Desktop installers for macOS and Windows. This repo has **binaries only**, no source code.

**macOS:** Open the **`.dmg`** and double-click **`Instalar Mijo.terminal`** (opens Terminal and runs the installer). Alternatively use the **`.pkg`** after `xattr -cr` if Gatekeeper blocks it.

**Windows:** Run the `.exe` installer; use “Run anyway” if SmartScreen blocks an unsigned build.

**Updates:** The desktop app checks this repo for new versions. **Report issues here.**
