# Jelly Shell — The Workhorse Creative Twist

The semi-translucent tinted polycarbonate jelly shell is the single most forgiving and reliable creative twist in this skill. When in doubt, use it. It carries the Y2K / iMac G3 / Game Boy Color reference cleanly, gives the object a face-friendly surface, and is what NB2 renders best.

## What "jelly shell" means here

A **tinted, semi-translucent polycarbonate outer shell** — not fully clear, not fully opaque. The 1999 iMac G3 and the Game Boy Color "Atomic Purple" edition are the canonical references. You can see shapes *through* the shell, but as quiet silhouettes, not as exposed circuit-board detail.

## The translucency calibration (most important thing on this page)

This is where most prompts fail. NB2 treats transparency as binary — either the shell reads as a lightly-tinted overlay (too opaque, looks like painted plastic) or it renders fully see-through with every PCB trace, chip, and screw exposed (too transparent, looks like a clear acrylic model, not a jelly shell).

You want the **middle**: interior components present as **faint darker shapes**, not as crisp hardware.

### Softening language to use

Use phrases like these, verbatim where possible:

- *"semi-translucent tinted polycarbonate jelly shell"*
- *"interior components softly visible as faint darker shapes through the tint"*
- *"gentle silhouettes of the internal chassis visible through the shell"*
- *"quiet interior geography, not crisp component detail"*
- *"the tint carries the shell, the interior reads as subtle depth behind it"*

### Forbidden language (always over-transparents the shell)

Do NOT use:

- *"clearly visible through the shell"*
- *"bold interior geography"*
- *"visible component outlines"*
- *"exposed PCB"*
- *"all internal components visible"*
- *"crystal clear"*
- *"see the circuit board"*

Even one of these phrases will tip the render fully see-through. NB2 over-weights transparency cues.

## Saturation rule (stacks with translucency)

The tint must be **candy-saturated, iMac G3 / Game Boy Color bright.** A translucent shell at pale saturation renders washed-out and milky. Always include the saturation lock:

> *"saturated candy-[color] polycarbonate — iMac G3 saturation, rich and candy-bright, fully saturated, NOT pale, NOT milky, NOT washed out"*

The "NOT pale NOT milky NOT washed out" triple is load-bearing. It is the single most reliable anti-washout phrase this skill has found.

See `palette.md` for the full approved color list.

## What the shell does vs what the other components do

The jelly shell is the **primary body**. Supporting components stay **opaque in neutral materials** for contrast:

- Cream/off-white ABS (knobs, buttons, bezels)
- Brushed steel (handles, pivots, small chrome accents)
- Graphite-dark matte (screens, rubber grips)
- Candy-red rubber (the mouth face button — the one high-saturation accent)

This **translucent shell + opaque neutral components** pattern is what separates a calibrated Zero render from a generic transparent-toy render. If every component were also translucent, the object would collapse into a clear-plastic prototype look. The contrast between jelly shell and opaque supports is what sells the Y2K product register.

## When NOT to use a jelly shell

- **Spheres in dark tints** — purple/violet on a spherical surface renders chromatic/metallic rather than jelly. Switch to candy-red / coral / amber / mint, or switch to a different twist.
- **Objects with mostly-metal real-world referents** where the metal itself is the design point (e.g., a brushed-steel thermos). Consider the material-swap twist instead — or combine jelly shell on one component with metal on another.
- **Very small objects** where the interior geography is too small to read. The softening rule depends on having *some* interior to see softly.

## Combining jelly shell with other twists

Jelly shell pairs especially well with **electronic graft**: a non-electronic object gets a small retrofit LCD + rubber button pod, and the main body is the jelly shell. This is how the padlock-with-keypad, thermos-with-display, and notebook-with-LCD renders work.

A prompt may combine two twists (jelly shell + electronic graft is the workhorse combo) but never three — three twists confuses the silhouette and the render loses coherence.

## Example shell clause (ready to drop into a prompt)

> *"The primary body is a semi-translucent tinted polycarbonate jelly shell in saturated candy-[COLOR] — iMac G3 saturation, rich and candy-bright, fully saturated, NOT pale, NOT milky, NOT washed out. The interior chassis and components sit softly visible as faint darker shapes behind the tint — quiet interior geography, not crisp component detail. The shell has a subtle satin sheen, not a mirror gloss."*
