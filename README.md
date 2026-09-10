# dxf-DR

**Open a STEP file, click a flat face, get a DXF.**

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
| macOS (Apple silicon) | `dxf-DR-macOS-AppleSilicon.dmg` — Developer ID signed and notarized |
| Windows (x64) | see the release page |

## Try it in the browser

No install: **[makerinparadise.com/dxf-dr/](https://makerinparadise.com/dxf-dr/)**

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
