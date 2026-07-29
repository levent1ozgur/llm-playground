## Task
Generate character-design prompts for DALL·E. Each prompt describes one isolated anime character for 3D model reference — no scenes, no backgrounds, no props unless worn/carried by the character.

## Objective
Produce N prompts, each independently sufficient (a 3D modeler could work from it with zero additional context), covering a specified spread of subgenres/archetypes so the batch isn't repetitive.

## Required fields per character (in order — front-loaded terms carry more weight)
1. **Core identity**: age bracket, role/archetype (e.g. "disgraced court alchemist")
2. **Silhouette-defining trait**: the one visual element that reads at a glance (asymmetric horn, mechanical arm, oversized collar)
3. **Hair**: color + cut + one texture/behavior detail ("windswept," "braided with wire")
4. **Eyes**: color/shape — only add heterochromia or unusual iris detail if it's load-bearing for the concept
5. **Clothing**: 2–3 concrete garment/material terms, not abstract genre words ("frayed wool trench, brass buckles" beats "steampunk outfit")
6. **One behavioral/prop quirk**: a held object or pose tic, stated plainly
7. **Art-style anchor**: one concrete reference ("Yoshitaka Amano linework," "early-2000s cel shading")
8. **Isolation clause** (fixed): "isolated on flat neutral background, no scenery"
9. **Technical spec** (fixed): "4K, clean linework, character reference sheet framing"

## Constraints
- No conflicting style terms in the same prompt (photorealistic + chibi, painterly + cel-shaded)
- No weighting syntax (`::1.5` etc.) — DALL·E doesn't support it; emphasize by stating a term first and restating it once
- Vary archetype, silhouette trait, and art-style anchor across the batch — no two of the N should default to the same shape
- Keep each prompt to 2–3 sentences
