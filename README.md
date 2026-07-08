# Mijo — Descargas

**Mijo** es una interfaz visual para trabajar con agentes de IA en tus proyectos de código: chat, diffs, terminal integrado, permisos, skills, túneles remotos y más. Disponible como **app de escritorio** (macOS y Windows), **navegador/PWA** y **extensión de VS Code**.

Este repositorio es **solo para instaladores y actualizaciones**. No contiene el código fuente de la aplicación.

---

## Descargar la última versión

👉 **[Ver todas las versiones (Releases)](https://github.com/FaidersAltamar/Mijo-releases/releases/latest)** — actualmente **v1.13.60** (macOS + Windows)

| Plataforma | Archivo recomendado | Notas |
|------------|---------------------|-------|
| **macOS (Apple Silicon)** | `Mijo-*-mac-arm64.dmg` | Abre el DMG → doble clic en **`Instalar Mijo.html`** |
| **macOS (Apple Silicon)** | `Mijo-*-mac-arm64.pkg` | Asistente estándar (ver abajo si macOS bloquea) |
| **macOS (Intel)** | `Mijo-*-mac-x64.pkg` / `.dmg` | Si está publicado en Releases |
| **Windows (64 bits)** | `Mijo-*-win-x64.exe` | **Usa v1.13.19 o superior** (versiones anteriores rotas) |
| **Windows (ARM)** | `Mijo-*-win-arm64.exe` | Surface / PCs con Snapdragon |

También hay archivos `.zip` por si prefieres descomprimir manualmente.

---

## Instalación en macOS

Mijo aún **no tiene certificado Apple notarizado**. macOS bloquea al doble clic archivos como `.command`, `.terminal` o `.pkg` sin firma (*"Apple no pudo verificar…"*). Por eso el instalador usa una guía HTML que **sí se abre sin bloqueo**.

### Opción A — DMG (recomendada)

1. Descarga `Mijo-*-mac-arm64.dmg` desde [Releases](https://github.com/FaidersAltamar/Mijo-releases/releases/latest).
2. Abre el `.dmg`.
3. Haz doble clic en **`Instalar Mijo.html`** (se abre en el navegador).
4. Pulsa **Copiar comando**, abre **Terminal** y pega el comando → **Enter**.
5. Mijo se instala en `~/Applications` y se abre solo.

### Opción B — Un solo comando en Terminal

```bash
curl -fsSL https://mijocode.com/install | bash
```

### Opción C — Arrastrar a Aplicaciones

1. Abre el `.dmg`.
2. Arrastra **Mijo** a la carpeta **Aplicaciones**.
3. Si macOS bloquea la primera apertura: clic derecho en **Mijo** → **Abrir** → **Abrir**.

### Opción D — Archivo `.pkg`

```bash
xattr -cr ~/Downloads/Mijo-*-mac-arm64.pkg
open ~/Downloads/Mijo-*-mac-arm64.pkg
```

---

## Instalación en Windows

1. Descarga `Mijo-*-win-x64.exe` (o `win-arm64.exe` en PCs ARM).
2. Ejecuta el instalador.
3. Si SmartScreen advierte que Windows protegió tu PC, elige **Más información** → **Ejecutar de todas formas**.

### PowerShell (recomendado)

```powershell
irm https://mijocode.com/install.ps1 | iex
```

---

## Actualizaciones automáticas

La app de escritorio comprueba nuevas versiones en **este repositorio** (`Mijo-releases`).

- En Mijo: menú o ajustes → **Buscar actualizaciones**.

---

## Soporte

👉 **[Abrir un issue](https://github.com/FaidersAltamar/Mijo-releases/issues)** — indica macOS/Windows, versión de Mijo y chip (Intel o Apple Silicon).

---

## English (short)

**macOS:** Open the `.dmg`, double-click **`Instalar Mijo.html`**, copy the Terminal command, and run it. Or run `curl -fsSL https://mijocode.com/install | bash`.

**Windows:** Run the `.exe` installer; use “Run anyway” if SmartScreen blocks it.

**Updates:** The desktop app checks this repo. **Report issues here.**
