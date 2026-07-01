# Spacetime Lattice

A real-time, interactive visualization of gravitational spacetime as a **dynamic simulated medium**. The field is a 64³ wave-equation cellular automaton evolved on the GPU (φ, π in float-texture slice atlases), so gravity propagates at finite speed rather than snapping to an analytic warp. Built with [three.js](https://threejs.org/) / WebGL.

**▶ Live demo: https://aaronsb.github.io/spacetime-lattice/**

![Spacetime Lattice](screenshot.png)

## About

An orbiting binary sheds spiral wavefronts into the lattice; quadrupole-rate energy loss drives inspiral and momentum-conserving mergers. Cross-section sliders paint a "magnet film" scan of the field on the cut plane, the laser probes the live field as a chirp sensor, and a strain strip-chart shows the LIGO-style h(t) trace.

An **Analytic/Dynamic toggle** A/Bs the live simulation against the original analytic model — a 1000³ coordinate volume of grid nodes drawn toward a central mass along a smooth radial power-law, rendering curvature as luminance where the nodes crowd.

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
