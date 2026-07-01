# Spacetime Lattice

A real-time, interactive visualization of gravitational spacetime curvature. A 1000³ coordinate volume of grid nodes is drawn toward a central mass — where they crowd, space glows. Built with [three.js](https://threejs.org/) / WebGL.

**▶ Live demo: https://aaronsb.github.io/spacetime-lattice/**

![Spacetime Lattice](screenshot.png)

## About

Grid nodes fold inward following a smooth radial power-law, producing a continuous density gradient that renders curvature as luminance. The instrument panel exposes controls for the lattice, gravity model, and rendering.

## Running locally

It's a single self-contained HTML file — just open it in a browser:

```bash
open index.html      # macOS
xdg-open index.html  # Linux
```

Or serve it:

```bash
python3 -m http.server
```
