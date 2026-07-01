# Mijo — Descargas

**Mijo** es una interfaz visual para trabajar con agentes de IA en tus proyectos de código: chat, diffs, terminal integrado, permisos, skills, túneles remotos y más. Disponible como **app de escritorio** (macOS y Windows), **navegador/PWA** y **extensión de VS Code**.

Este repositorio es **solo para instaladores y actualizaciones**. No contiene el código fuente de la aplicación.

---

## Descargar la última versión

👉 **[Ver todas las versiones (Releases)](https://github.com/FaidersAltamar/Mijo-releases/releases/latest)**

| Plataforma | Archivo recomendado | Notas |
|------------|---------------------|-------|
| **macOS (Apple Silicon)** | `Mijo-*-mac-arm64.dmg` | Mac con chip M1/M2/M3/M4 |
| **macOS (Intel)** | `Mijo-*-mac-x64.dmg` | Si está publicado en Releases |
| **Windows (64 bits)** | `Mijo-*-win-x64.exe` | La mayoría de PCs con Windows |
| **Windows (ARM)** | `Mijo-*-win-arm64.exe` | Surface / PCs con Snapdragon |

También hay archivos `.zip` por si prefieres descomprimir manualmente en lugar del instalador.

---

## Instalación en macOS

Los instaladores actuales **no están firmados con certificado de Apple** (sin notarización). La primera vez, macOS puede mostrar:

> *«Apple no pudo verificar que Mijo esté libre de malware…»*

**No pulses «Mover al basurero».** Sigue estos pasos:

### Opción recomendada (desde el DMG)

1. Abre el archivo `.dmg` que descargaste.
2. **No hagas doble clic en `Mijo.app` dentro del volumen del DMG.**
3. Haz doble clic en **`INSTALAR MIJO.command`**.
4. Si macOS pregunta si confías en el archivo, elige **Abrir**.
5. Pulsa **Continuar** en el diálogo del instalador.
6. Mijo se copia a **Aplicaciones** y se abre solo.

### Si el instalador también se bloquea

**Clic derecho:** clic derecho en `INSTALAR MIJO.command` → **Abrir** → **Abrir**.

**Terminal** (ajusta el nombre del volumen si tu versión es distinta):

```bash
bash "/Volumes/Mijo 1.13.17/INSTALAR MIJO.command"
```

**Si ya copiaste la app a Aplicaciones:**

```bash
xattr -cr /Applications/Mijo.app
open /Applications/Mijo.app
```

**Ajustes del sistema:** **Privacidad y seguridad** → **Abrir de todas formas** (aparece tras el primer intento bloqueado).

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
- En macOS, con builds sin firma de Apple, la actualización in-app puede pedirte **descargar el DMG manualmente** en lugar de reiniciar para aplicar el parche. Usa el enlace que muestra el diálogo o vuelve a esta página.

Publicar una versión nueva aquí **no requiere** que el código fuente sea público.

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
| **Mijo-releases** (este, público) | `.dmg`, `.exe`, `.zip`, manifiestos de auto-actualización |
| **Mijo** (privado) | Código fuente y desarrollo |

Los instaladores se generan y publican automáticamente al lanzar una nueva versión.

---

## English (short)

**[Download latest release](https://github.com/FaidersAltamar/Mijo-releases/releases/latest)** — Desktop installers for macOS and Windows. This repo has **binaries only**, no source code.

**macOS:** Open the DMG and run **`INSTALAR MIJO.command`** (do not double-click `Mijo.app` inside the DMG). Unsigned builds trigger Gatekeeper; use Right-click → Open or `xattr -cr /Applications/Mijo.app`.

**Windows:** Run the `.exe` installer; use “Run anyway” if SmartScreen blocks an unsigned build.

**Updates:** The desktop app checks this repo for new versions. **[Report issues here](https://github.com/FaidersAltamar/Mijo-releases/issues).**
