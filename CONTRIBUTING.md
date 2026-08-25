# Contributing to the Flower of Life Composer

Welcome. The barrier to entry here is a text editor and curiosity. The whole app is one HTML file you can read in twenty minutes.

## The doors

**Pattern makers** — bring a construction from your tradition. If you can describe how it is drawn with compass and straightedge, it can become a module. Open an issue describing the construction (a photo of a hand drawing is a perfectly good specification).

**Coders** — the app is structured in three regions inside `index.html`:

- **model** — pure state: `{ rings, removed, boundary, weight }`, the lattice math, and `metrics()`
- **render** — the on-screen view only; ghosts of removed circles and hover highlights live here and never reach the export
- **serialize** — a pure function from state to SVG text; deterministic, no DOM

Good first territories: save/load of compositions as small text files, a square lattice, polar construction for mandalas, touch support, color-respecting print exports.

**Geometers and historians** — the constructions deserve documentation of their lineage, so the tool teaches as it draws. Prose contributions are contributions.

**Makers** — test the exports against real machines and materials: laser cutters, embroidery, vinyl, CNC. Tell us where the lines fail.

**Everyone else** — compose something and share it. The gallery begins the moment two people have traded a pattern.

## Principles

1. **Construction, never image.** Every pattern must be expressible as geometry anyone can re-derive by reading the code.
2. **One file, no dependencies, as long as possible.** Simplicity is the front door. A framework has to earn its way in against that.
3. **The export is sacred.** Files the tool produces must be deterministic, clean, and free of any interface artifacts.
4. **One stroke color per export.** The moment this tool grows a palette it stops producing marks and starts producing illustrations.

## Process

Fork, change, open a pull request. For anything substantial, open an issue first so the conversation can happen before the work.
