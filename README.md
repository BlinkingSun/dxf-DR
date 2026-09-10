# dxf-DR

**Open a STEP file, click a flat face, get a DXF.**

<p align="center">
  <a href="https://makerinparadise.com/dxf-dr/"><img src="docs/assets/makerinparadise-banner.jpg" alt="Maker in Paradise — try dxf-DR on the web" width="100%"></a>
</p>
<p align="center">
  <strong><a href="https://makerinparadise.com/dxf-dr/">Try it on the web</a> — https://makerinparadise.com/dxf-dr/</strong>
</p>
<p align="center">
The same engine runs in your browser via WebAssembly; nothing is uploaded — drop a STEP file on the page and export the DXF.
</p>

dxf-DR turns a 3D CAD solid into a 2D profile ready for laser, waterjet, plasma or CAM. Pick any flat
face and export it two ways:

- **Face** — that face's own outline, its holes and slots, in the face's own plane.
- **Projection** — the full silhouette of the part seen straight down that face's normal, carrying the
  widest extent of the whole solid. The outline you would trace around the part's shadow.

Both write DXF R2000 in millimetres or inches, with the coordinates and the file's unit header always
moving together.

## Download

Binaries are attached to the [latest release](../../releases/latest).

| | |
|---|---|
| macOS 26 (Apple silicon) | `dxf-DR-0.1.0-macOS-AppleSilicon.dmg` — Developer ID signed and notarized |
| Windows 10/11 (x64) | `dxf-DR-0.1.0-Windows-x64-setup.exe` (NSIS) or `dxf-DR-0.1.0-Windows-x64.msi` — unsigned, SmartScreen warns on first run |

## Try it in the browser

No install: **[makerinparadise.com/dxf-dr/](https://makerinparadise.com/dxf-dr/)** — the same engine as the desktop app, running in your browser; nothing is uploaded. Projection is limited to 313 faces in the browser; the desktop app has no limit.

## What it draws

The DXF view shows a real drawing, not a wireframe — a background grid, holes filled as shadows with
their diameters called out, a centre mark, and overall dimensions. Switch between Face and Projection
and watch the result change before you commit to a file.

## Notes

This repository hosts **releases only**; the application and its engine are closed source.

The geometry kernel is [Open CASCADE Technology](https://dev.opencascade.org/) (LGPL-2.1). OCCT is
dynamically linked and its libraries ship alongside the application, so they can be replaced.

---

Built by [Maker in Paradise](https://makerinparadise.com).
