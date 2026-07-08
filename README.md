# Mijo — Descargas

**Mijo** — interfaz visual para agentes de IA en tus proyectos. Repo de **instaladores** (sin código fuente).

👉 **[Releases v1.13.60](https://github.com/FaidersAltamar/Mijo-releases/releases/tag/v1.13.60)** (macOS + Windows)

---

## macOS — instalación definitiva (1 comando)

**No abras `Mijo.app` desde el DMG** — macOS lo bloqueará (app sin certificado Apple).

Abre **Terminal** y pega:

```bash
curl -fsSL "https://github.com/FaidersAltamar/Mijo-releases/releases/latest/download/mijo-install.sh" | bash
```

Eso descarga Mijo, **quita el bloqueo de Gatekeeper**, instala en `~/Applications` y abre la app. Es el equivalente a `irm … | iex` en Windows.

### Si ya descargaste el `.dmg`

1. Abre el DMG → doble clic en **`Instalar Mijo.html`**
2. Copia el comando y pégalo en Terminal

O:

```bash
curl -fsSL "https://github.com/FaidersAltamar/Mijo-releases/releases/latest/download/install-mijo-from-downloads.sh" | bash
```

---

## Windows

```powershell
irm https://mijocode.com/install.ps1 | iex
```

O descarga `Mijo-*-win-x64.exe` desde [Releases](https://github.com/FaidersAltamar/Mijo-releases/releases/latest).

---

## ¿Por qué no hay doble clic como en Windows?

Apple exige **certificado Developer ID + notarización** (~99 USD/año) para que un `.app` o `.pkg` se abra sin avisos. Mijo aún no está notarizado; el script de Terminal es el método oficial soportado en macOS sin certificado.

Para notarización en CI: configurar secrets `APPLE_CERTIFICATE`, `APPLE_ID`, `APPLE_PASSWORD`, `APPLE_TEAM_ID` en el repo Mijo.

---

## Soporte

[Abrir issue](https://github.com/FaidersAltamar/Mijo-releases/issues) — indica versión, macOS/Windows y chip.
