# CME P00 — Interactive Playground

Interactive 3D visualization of **Carrier Manifold Encoding (P00)** stack combinations across all carriers. Runs on **GitHub Pages** with zero build step.

## Quick start

1. Copy `docs/cme-playground/` into your repo.
2. GitHub: **Settings → Pages → Source: Deploy from branch `main`, folder `/docs`**.
3. URL: `https://<username>.github.io/<repo>/cme-playground/`

For root URL (`github.io/repo/`), put `index.html` at repo root and set Pages source to `/root`.

## Link from README

GitHub does not run `<script>` in markdown — link to Pages:

```markdown
**→ [Open interactive demo](https://YOUR_USERNAME.github.io/YOUR_REPO/cme-playground/)**
```

## Local preview

```bash
cd docs/cme-playground
python3 -m http.server 8080
# open http://localhost:8080
```

Must use HTTP (not `file://`) for ES module imports.

## Rendering

- **InstancedMesh** icosahedra — crisp opaque dots, no blurry GL_POINTS overlap
- **EdgesGeometry** carrier outline — clean wireframe
- No fog, no transparency blending on trajectory dots
