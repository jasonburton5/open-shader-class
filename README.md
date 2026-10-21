# Open Shader Class

Open course material for learning real-time shaders and neural material techniques, built in public one lesson at a time.

Each lesson is a small, self-contained, compilable example with a short write-up. The goal is teaching: every shader here is written to be read, not just run.

## What's here

- `lessons/` — numbered lessons, each with its own README, source, and a minimal scene to open it in
- `common/` — shared helper functions and utility shaders used across lessons
- `docs/` — the course outline and background notes

The catalog grows over time. Lessons marked **(planned)** in the outline have no code yet.

## Course outline (living document)

1. **Foundations** — the graphics pipeline, vertex vs. fragment work, UVs, normals, and what a shader actually computes
2. **Surface shading** — a physically based material from scratch: diffuse, specular, roughness, metalness, Fresnel
3. **Procedural materials** — noise, domain warping, layering, and masking (lava, rock, wood, fabric)
4. **Material behaviors** — animated and reactive surfaces, blending between materials, parameter-driven interiors
5. **Neural materials** — small learned networks as material approximators: dataset capture from a Cornell box, training a tiny MLP, running inference inside a shader
6. **Image-driven material selection** — using an open image-tagging model to pick and blend library materials at runtime
7. **Portability** — moving the same shader across engines and backends with minimal changes

## Engines and targets

Primary target is Unreal Engine with a Godot fallback for each lesson where practical. Shaders are written to be as backend-neutral as possible; vendor-specific paths are isolated and clearly labeled.

## Requirements

- A current release of Unreal Engine or Godot
- A GPU with modern shader model support
- Python 3.10+ for the training lessons (see each lesson's README for packages)

## Using this material

Everything here is released under the Apache License 2.0 (see `LICENSE`). You may use, modify, teach from, and redistribute it, including commercially, with attribution and the license notice intact.

If you teach from this material, a link back is appreciated but not required.

## Contributing

Issues and pull requests are welcome, especially corrections, clearer explanations, and ports to other engines. Keep contributions self-contained and documented in the same lesson format.

## Author

Jason Burton

## Changelog

- **2026-10-21** — repository created; README and license added.
