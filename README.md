# あntLAU ⚒
### Minecraft Launcher — Beta Privada v0.4.5

> Un launcher de Minecraft hecho a mano en Venezuela con amor, rabia y demasiado café.
> Funciona. No te preguntes cómo. No lo toques.

---

## ¿Qué es esto?

**あntLAU** es un launcher personalizado para Minecraft Forge construido con Electron + Node.js, pensado para servidores privados cracked. Sin Mojang. Sin login. Sin que te pregunten nada.

Actualmente soporta **Forge 1.20.1** de forma estable. Las otras versiones están en proceso — tranquilo que ya van.

---

## Características

- ⚒ **Lanzador Forge 1.20.1** funcional (cracked / offline)
- 🧩 **Gestión de mods** — íconos, activar/desactivar, eliminar, activar todos / desactivar todos
- 🗂 **Perfiles de mods** — crea, carga, exporta e importa perfiles `.json`
- 🎨 **Skins** — integración con [ely.by](https://ely.by) + [CustomSkinLoader](https://modrinth.com/mod/customskinloader) (descarga directa desde Modrinth)
- 🖼 **Fondo de pantalla custom** — con opacidad ajustable mediante `.opa`
- 📋 **Logs** — launcher, lanzamientos diarios y log del juego en tiempo real
- 🖥 **Servidor local** — consola, mods/plugins, whitelist, propiedades y editor MOTD
- 🔧 **Modo Admin** — herramientas de diagnóstico ocultas, actívalo con `.adminAT` en la consola de logs
- 💾 **Config persistente** en `%AppData%\antLAU\config.json`
- ☕ **Java auto-detección** — busca el más nuevo, ignora los de 32-bit (como debe ser)

---

## Requisitos

- Windows 10/11 x64
- Java 17+ (se auto-detecta, pero si no lo tienes, instálalo pues)
- Minecraft Forge 1.20.1 ya instalado en tu carpeta mcdata

---

## Instalación

### Opción A — Ejecutable (recomendado)
Descarga el instalador desde [Releases](../../releases) y ejecútalo. Listo. No hay paso 2.

### Opción B — Desde el código fuente
```bash
git clone https://github.com/TU_USUARIO/antlau.git
cd antlau
npm install
npm start
```

### Compilar `.exe`
```bash
npm run build
```
El resultado queda en `dist/antLAU Setup 0.4.5.exe`

---

## Modo Admin

Dentro del launcher, ve a **Logs → Launcher** y escribe en la consola:

```
.adminAT
```

Se desbloquea el servidor local y las herramientas de diagnóstico. Escribe `.help` para ver todos los comandos disponibles.

| Comando | Descripción |
|---|---|
| `.sysinfo` | RAM, Java, rutas del sistema |
| `.ping [host]` | Latencia TCP a un servidor |
| `.checknet` | Verifica conectividad a Mojang, ely.by, Modrinth y más |
| `.pconfig` | Imprime el config.json completo en consola |
| `.changelog` | Historial de versiones |
| `.opa [ui%] [bg%]` | Ajusta opacidades de la UI y el fondo |
| `.cleanlogs` | Limpia los archivos `.log` del directorio antLAU |
| `.restart` | Reinicia el launcher |
| `...` | y más — escribe `.help` |

---

## Historial de versiones

| Versión | Cambios |
|---|---|
| `v0.4.5-bp` | Defaults de opacidad 60/40, visibilidad de botones al 65% |
| `v0.4.4-bp` | Comando `.opa` para opacidad personalizable |
| `v0.4.3-bp` | Fix `.changelog`, `.pconfig`, versionado semántico |
| `v0.4.2-bp` | Fix carga de config y RAM al inicio |
| `v0.4.1-bp` | Iconos reales, fixes de UI, eliminación del instalador automático |
| `v0.4.0-bp` | Modo Admin con herramientas de diagnóstico |
| `v0.3.0-bp` | Perfiles de mods + wallpaper personalizado |
| `v0.2.0-bp` | Skins ely.by + CustomSkinLoader |
| `v0.1.0-bp` | Lanzador base funcional |

---

## Stack

- [Electron](https://electronjs.org) 28
- Node.js 22
- HTML/CSS/JS vanilla — sin frameworks, porque aquí somos así de tercos

---

## Licencia

**Copyright © 2025 AntLGあ — Todos los derechos reservados.**

Consulta el archivo [LICENSE](LICENSE) para los términos completos.

---

<div align="center">
  Hecho con ⚒ por <strong>AntLGあ</strong> — Venezuela 🇻🇪
</div>
