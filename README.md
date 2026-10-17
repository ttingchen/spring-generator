# Coilwright — Spring Generator

A single-page web app that generates 3D helical springs and exports them as **STL** or **OBJ**.

**Live site: https://ttingchen.github.io/spring-generator/**

You can also open `index.html` locally in a browser — no build step, no server.

## Spring types

- **Compression** — free length, end type (closed & ground, closed, open), optional taper (conical)
- **Extension** — coil gap, machine-loop hooks, hook alignment (0° / 90° / 180°)
- **Torsion** — leg length, leg offset angle, coil gap

Shared parameters: wire diameter, outer diameter, active coils, wind direction, mesh detail (sides around the wire, segments per coil), material and finish.

## Engineering readout

Spring rate (N/mm, or N·mm/° for torsion), spring index D/d, pitch, solid height, wire length and mass, plus warnings for coil bind, buckling risk, extreme spring index, and touching coils that would fuse when 3D printed.

## Export

Watertight swept-tube mesh, millimetres, Z-up. Binary STL or OBJ.

Built with [three.js](https://threejs.org/) r128.
