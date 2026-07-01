# Spacetime Lattice

A real-time, interactive visualization of gravitational spacetime curvature. A 1000³ coordinate volume of grid nodes is drawn toward a central mass — where they crowd, space glows. Built with [three.js](https://threejs.org/) / WebGL.

**▶ Live demo: https://aaronsb.github.io/spacetime-lattice/**

![Spacetime Lattice](screenshot.png)

## About

Grid nodes fold inward following a smooth radial power-law, producing a continuous density gradient that renders curvature as luminance. The instrument panel exposes controls for the lattice, gravity model, and rendering.

## Dynamic field prototype (`wave.html`)

`wave.html` replaces the analytic warp with a real simulated medium: the field is a 64³ wave-equation cellular automaton evolved on the GPU (φ, π in float-texture slice atlases), so gravity propagates at finite speed. An orbiting binary sheds spiral wavefronts, quadrupole-rate energy loss drives inspiral and momentum-conserving mergers, cross-section sliders paint a "magnet film" scan of the field on the cut plane, the laser probes the live field as a chirp sensor, and a strain strip-chart shows the LIGO-style h(t) trace. An Analytic/Dynamic toggle A/Bs against the original model.

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
