<h1 align="center">Flight</h1>

<p align="center">A graphics and application SDK for AI agents.</p>
<p align="center"><em>explicit · grepable · nothing hidden</em></p>

---

Flight's API is **cellular** — every function is self-contained, legible in
isolation, and free of hidden state. Explicit inputs, explicit outputs, no
globals to trace, no implicit runtime behavior. An agent reading one function
understands and applies it without context from anywhere else in the codebase.

The same properties that make Flight easy to reason over make bundles small.
Nothing runs at import time — renderers, update loops, and listeners are all
opt-in — so a build ships only what it uses.

Flight spans the full stack an interactive app needs:

- **Scene graph** — display objects, shapes, text, sprites, tilemaps.
- **Multi-backend rendering** — one scene, drawn through DOM, Canvas, WebGL 2, or WebGPU.
- **Offscreen image processing** — read and generate pixel data with no display attached.
- **Application layer** — animation, input, audio, video, filters, windowing, and platform integration.

### Principles

- **Explicit, not magic** — rendering, allocation, and update passes are invoked by name.
- **Plain data** — colors are packed integers, filters are descriptors, transforms write to out-params.
- **Self-identifying names** — every export carries the full type it operates on; grepable by design.
- **Bounded & owned** — tree-shakable packages you can import in isolation and understand in full.

### Explore

- 🌐 **[flighthq.ai](https://flighthq.ai)** — overview, live demo, and bundle-size story
- 🧩 **[Example explorer](https://flighthq.github.io/flight)** — every scene across each renderer
- 📦 **[github.com/flighthq/flight](https://github.com/flighthq/flight)** — the monorepo
