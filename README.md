# Zen Garden

**AppADay 064** · Interactive · Shipped 2026-07-10

A karesansui — a dry rock garden — that you rake with your finger. Carve grooves in raked sand, set stones and moss and a lantern, and ripple the sand around them.

## What it does

The sand is a real height field. Every groove you draw is lit from the upper left and shadowed on its far wall, with a small ridge of displaced sand along each edge, so the patterns read as carved rather than painted.

**Rakes**

- **Finger** — a single soft groove.
- **Rake** — three tines.
- **Wide rake** — six tines.
- **Ripples** — tap the sand to set concentric rings, or tap a stone to wrap rings around it.
- **Smoothing brush** — wipe grooves back to flat.

**Elements**

Stone, mossy stone, pebbles, maple leaf, blossom, and a stone lantern. Tap an element in the rack, then tap the sand to set it. Drag any element to move it — heavier ones plow a furrow behind them as they go. Drop an element on the bar that appears at the bottom of the garden to remove it; its imprint stays in the sand until you rake it out.

**Flatten the sand** returns the whole field to flat while leaving your elements in place. **Save image** downloads a PNG of the garden, stamped with a vermilion seal.

## Design

Dark cedar frame against pale raked sand. Nothing persists between sessions — a garden is raked fresh each time, which is also the honest behavior inside a sandboxed browser frame where local storage is unavailable.

## Stack

Single-file vanilla HTML, CSS, and JavaScript. No build step, no frameworks, no dependencies. The sand simulation is a `Float32Array` height field rendered to an offscreen canvas via `ImageData` and upscaled to the display canvas. Pointer events only, so it works identically with a finger or a mouse.

## Run it

Open `index.html` in any modern browser, or visit the live version:

https://augustineiacopelli.github.io/appaday-064-zen-garden/

---

Part of [AppADay](https://augustineiacopelli.github.io/appaday/) — one complete web app, every day.
