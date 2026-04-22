# Rules — Absolute Constraints + 6-Layer Prompt Structure

These rules are non-negotiable. They were locked after 33 iterative test renders. Breaking any of them produces a predictable, known failure mode.

## Absolute rules

### Staging

- **Pure white background** `#ffffff`, completely flat, no gradient.
- **Single object.** No multi-object compositions, no props, no hands, no stands, no surfaces, no plinths, no shelves.
- **Floating, shadowless.** Object floats freely in mid-air on pure white. **NO contact shadow, NO ground shadow, NO plinth, NO surface implied.** Assume no ground exists at all — the object has no spatial grounding whatsoever.
- **No bases, pedestals, stands, or feet.** Objects must be single self-contained floating forms. If the real-world reference typically sits on a base (CRT monitor, microscope, lamp), render the baseless/tabletop variant or the body alone.
- **No cables, wires, or cords exiting the object silhouette.** Wires contained within the object body are fine (visible through a jelly shell, coiled on-object, terminating at a connector on the object). Any cable trailing onto the white background breaks isolation.
- **Compact.** One cohesive object silhouette, not a cluster.

### Object content / materials

- **No fluids** of any kind — no gas, water, steam, smoke, mist, flames, melted wax, droplets, clouds.
- **No externally-emitting beams** (laser lines, projected light, mist, steam) on pure-white backgrounds — they bleed outside the silhouette. Light must stay contained inside the object (LED glow, LCD illumination, light inside a tinted window is fine).
- **No sci-fi / futuristic metaphors** — no glowing lattices, no holograms, no "data cubes," no speculative tech. Retro-tech yes, future-tech no.
- **No transparent hero materials** — no clear glass bodies, no acrylic, no resin shells. *Exception: tinted translucent polycarbonate jelly shells (Y2K aesthetic) are approved — see `jelly-shell.md`.*
- **No knots, coils, bends, or twists** as the hero twist. High failure variance — the model defaults to stacked rings or cheats the cross-section.
- **No monochromatic single-material flattening** on complex objects — one material everywhere produces toy look. Use per-component palette.
- **No wood** as a material.
- **No dirt, dust, fingerprints, scratches, patina, oxidation, wear, or aging.** Every object is factory-fresh, showroom-clean, pristine.
- **No mirror-polish as the default primary body.** Reserve gloss for small components (knobs, buttons, LCD glass, lens bezels). Primary bodies default to matte, satin, soft-touch, or eggshell.

### Text and branding

- **Never write "Zero" or any Zero wordmark anywhere.**
- **No brand names visible on objects, real or invented.** Only model codes (e.g., "CRT-1700 / VGA", "RC-3000 / 27-CORE"), product-category copy, spec/regulatory text, and warning decals. Wordmarks like "PALM", "Symbol", "iRobot", "Fluke", "Mattel", "Black+Decker", or invented substitutes (DataPilot, ScanCore, DustLogic) all read as distracting text anchors.
- **All text is diegetic** — printed, silkscreened, embossed, or stamped onto the object, not floating labels.

### Aesthetic register

- **Not toy.** Saturated but not candy, matte not plastic-molded-kids'-toy.
- **Not sterile hero-render.** Tactile, consumer-grade, catalog-honest.
- **Not jewelry/luxury.** No high-gloss mirror finishes across the whole body.

---

## The 6-layer prompt structure

Every prompt stacks these six layers in order. See `canonical-examples.md` for three fully-worked examples.

### 1. Opening — object identification

One sentence: object type, framing, angle, white-background staging.

> *"A single compact Y2K-styled [object] floating in mid-air on a pure white #ffffff background, flat, no gradient, no contact shadow, no ground shadow, no surface, no spatial grounding."*

### 2. Creative twist — the hero move

What makes this a designer piece. One of:

- **Semi-translucent tinted jelly shell** — the workhorse, most forgiving. See `jelly-shell.md`.
- **Material swap** — ordinary object in unexpected opaque material. The swap must be obvious at half-a-second glance. Matte/satin finishes work better than mirror.
- **Electronic graft** — non-electronic object with a small retrofit electronics pod (thermos with LCD temp display, padlock with keypad).
- **Hybrid / morph** — two objects merging at a natural collar.
- **Impossible balance** — rigid object in impossible gravitational pose.

A prompt may combine two (jelly shell + electronic graft is very common) but never three.

### 3. Per-component material palette

Bulleted or inline list. Every named component gets its assigned material. At least 5 components, typically 7–10. Materials should read as their real-world type: ABS plastic, soft-touch rubber, brushed steel, chrome, powder-coated metal, porcelain, enamel, anodized aluminum, cream-colored cast plastic. Every boundary between materials is a **crisp hard line** — no gradient, no bleed.

The primary body defaults to **matte, satin, soft-touch, or eggshell.** Gloss reserved for small components (LCD glass, button tops, lens bezels, tiny chrome accents).

### 4. Electronic touch (always include)

If the object is natively electronic, surface one component as a specific personality anchor (smiley power button, pixel emoticon on an LCD). If the object is non-electronic, graft ONE small electronics module onto it — a rectangular pod, a control panel, a tiny LCD window. The electronic touch always includes:

- A small LCD or pixel screen (with specific diegetic text — e.g., "$ HELLO WORLD_", "SOLVE 00:42", "DC 3.142 V")
- A chunky soft-touch rubber face button (see `face-formula.md`)
- A small LED dot, gently lit
- Silkscreened labels identifying the controls

### 5. Y2K diegetic detail (restrained but information-dense)

Target **8–10 detail elements per prompt** — matching real Y2K product packaging density. A full set:

- **Model code only, no brand wordmark** (e.g., "CRT-1700 / VGA", "RC-3000 / 27-CORE", "LS-02 / READ")
- Lit LCD with specific diegetic readout text
- Spec line (TRUE RMS / CAT III 600V, 60Hz / 1024×768, 4.3×10¹⁹ STATES)
- **Functional labels on dials / ports / buttons** (OFF / mA / VΩ / BEEP / HOLD / RANGE / MENU / AUTO / + / −) — these are the single biggest density booster
- Warning decal (voltage warning, safety-class label)
- Foil barcode sticker with serial ("SN 0027-B")
- Holographic QC sticker
- Cartoon-eye decal (the personality hero — see `face-formula.md`)
- Face button (the face mouth — see `face-formula.md`)
- Gently-lit LED dot
- Wire/cable where natural — **contained within the silhouette** (coiled on body, looped, terminating at a connector that sits on the object)

Rule: information-dense but typographically organized. Real product packaging, not sticker-bombing.

### 6. Closing technical block

Use this near-verbatim at the end of every prompt:

> *Critical material and component accuracy: every named component displays its assigned material with a crisp hard boundary where materials meet — no bleed, no monochromatic flattening. Labels and stickers sit ON the surface as real decals, not painted patterns.*
>
> ***Surface finish realism:*** *color saturation sits IN the material, not painted over it. PBR shading is physically accurate: correct specular response for each material type. Default to matte, satin, soft-touch, or eggshell finishes on primary bodies — reserve gloss for small functional components (knobs, buttons, LCDs, lens glass). Factory-fresh clean — no dust, no fingerprints, no scratches, no wear, no patina, no aging of any kind — but tactile and consumer-grade, not CGI-candy, not mirror-chrome. Tints are saturated, candy-bright, iMac G3 saturation — NOT pale, NOT milky, NOT washed out.*
>
> ***Staging:*** *the object floats in mid-air on pure white. NO contact shadow, NO ground shadow, NO plinth, NO surface implied. Assume no ground exists. NO base, pedestal, stand, or foot. NO cables, wires, or cords exiting the silhouette — wires contained within the object are fine.*
>
> *Styled as if shot on [Phase One XT 55mm OR Hasselblad X2D 100mm macro] at f/5.6. Lighting: crisp directional studio key from upper-left; cool/warm controlled fill from the right.*
>
> *Backdrop: pure white (#ffffff), completely flat, no gradient. Aspect ratio 1:1, centered. Mood: [one-line mood tag]. Only the text/labels/stickers specified above, no other text, no watermarks, no additional objects.*
