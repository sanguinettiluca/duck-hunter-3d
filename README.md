# 🦆 Duck Hunt 3D

> **Edición Arcade 2026** — First Person Shooter en el navegador, sin dependencias, un solo archivo HTML.

![Duck Hunt 3D](https://img.shields.io/badge/version-1.0-ffcc02?style=flat-square&labelColor=111)
![Three.js](https://img.shields.io/badge/Three.js-r128-white?style=flat-square&labelColor=111)
![Sin dependencias](https://img.shields.io/badge/dependencias-ninguna-4af?style=flat-square&labelColor=111)
![Standalone](https://img.shields.io/badge/standalone-1%20archivo-4ade80?style=flat-square&labelColor=111)

---

## 🎮 Descripción

Duck Hunt 3D es un juego de disparos en primera persona completamente funcional que corre directo en el navegador. Inspirado en el clásico Duck Hunt de NES, reimaginado con gráficos 3D, mecánicas FPS modernas, modo cooperativo local y soporte para control PS5 DualSense.

**100% standalone** — un solo archivo `.html`, sin servidor, sin instalación, sin internet (excepto para las fuentes de Google Fonts).

---

## ✨ Características

### Gameplay
- 🦆 **100 patos** volando con IA y alas animadas
- 🎯 Objetivo: **600 puntos** en **2 minutos**
- 💥 Modelo 3D de **AK-47** con animación de retroceso
- 🔥 Power-up **Minigun** (drop raro al matar patos) — 6 cañones giratorios, disparo automático 10 segundos
- 🌲 **Easter egg secreto** — disparale 3 veces al árbol especial...

### Movimiento
- **WASD** — movimiento
- **Espacio** — salto
- **Shift** — dash direccional con efecto FOV
- **Mouse** — apuntar en 360°

### Armas & Combate
- 6 balas por cargador, recarga manual o automática
- Raycasting preciso con detección esférica
- Partículas de plumas al matar un pato

### Modos de juego
| Modo | Descripción |
|------|-------------|
| 🎯 **Un Jugador** | Clásico, teclado + mouse |
| 👥 **Coop Local** | Pantalla dividida horizontal, 2 jugadores en el mismo teclado o con controles |

### Coop Local — Controles P2
| Acción | Tecla |
|--------|-------|
| Mover | `I J K L` |
| Disparar | `U` |
| Recargar | `O` |
| Saltar | `L` (doble función) |
| Dash | `P` |
| Mirar | `Q` / `E` |

### 🎮 Soporte PS5 DualSense
Compatible con el Gamepad API del navegador. Conectá el control por USB o Bluetooth:

| Botón | Acción |
|-------|--------|
| L✦ (stick izq.) | Mover |
| R✦ (stick der.) | Apuntar |
| R2 / R1 | Disparar |
| ✕ Cross | Saltar |
| □ Square | Dash |
| ○ Circle | Recargar |
| Options | Pausa |
| D-Pad | También mueve |

> En modo Coop, el **control 1 = P1** y el **control 2 = P2**. Se puede mezclar: un jugador con teclado/mouse y el otro con control.

### 🏆 Scoreboard local
- Guarda automáticamente el **top 10** de puntajes en `localStorage`
- Distingue entre partidas **Solo** y **Coop**
- Muestra medallas 🥇🥈🥉, puntos, patos matados, tiempo y fecha
- Aparece en el menú principal

---

## 🕹️ Controles completos (Un Jugador)

| Acción | Control |
|--------|---------|
| Mover | `W A S D` |
| Disparar | Click izquierdo |
| Recargar | Click derecho |
| Saltar | `Espacio` |
| Dash | `Shift` |
| Pausa | `ESC` |

---

## 🚀 Cómo jugar

### Opción A — Abrir localmente
Descargá el archivo `index.html` y abrilo directo en el navegador. No requiere servidor.

```
Doble click en index.html → listo
```

### Opción B — Deployar en Cloudflare Pages
1. Renombrá el archivo a `index.html` si no lo está
2. Entrá a [Cloudflare Pages](https://pages.cloudflare.com)
3. Creá un nuevo proyecto → **"Upload assets"**
4. Arrastrá el archivo `index.html`
5. Deploy → ¡listo en segundos!

> ⚠️ Asegurate de que el archivo se llame exactamente `index.html` para que Cloudflare lo sirva en la raíz.

---

## 🛠️ Tecnologías

| Tecnología | Uso |
|------------|-----|
| [Three.js r128](https://threejs.org) | Renderizado 3D, modelos, escena |
| Web Audio API | Todos los sonidos generados proceduralmente |
| Gamepad API | Soporte PS5 DualSense |
| localStorage | Scoreboard persistente |
| CSS3 / Google Fonts | UI y menús |

Sin bundler, sin npm, sin frameworks. Todo vanilla.

---

## 📁 Estructura

```
index.html          ← el juego completo (~3000 líneas)
README.md           ← este archivo
```

---

## 🎨 Créditos

Desarrollado por **Luca Sanguinetti**
