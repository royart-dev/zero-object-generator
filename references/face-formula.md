# Face Formula — Personality Baked In

Every object in this skill's output carries a face. Not a literal sculpted face — an *implied* face assembled from one printed mouth and one printed eye element. This is the single move that takes a render from "cold product shot" to "quietly playful designer object."

**One object = one face. No more, no less.**

## The two components

### Mouth (rubber face button)

A chunky round soft-touch rubber button, typically candy-red, with a cream silkscreened mouth graphic dead-center. Functions as a **real control** — power, snooze, unlock, print, brew, start. Never a decorative button.

### Eye (printed decal)

A printed decal sticker applied to the surface — simple 1990s sticker style with a bold black outline and a white glint. **Never sculpted into the object.** Always specify "silkscreened decal applied to the surface" so the model renders it flat.

## Variation table (required for multi-object sets)

When generating 2+ objects for a single deliverable (course cards, UI tiles, product family), the mouth×eye pair **must be unique per object**. No two objects in a set share the same pair. This keeps the set feeling like a family of distinct personalities rather than a template stamp.

| | Options |
|---|---|
| **Mouth** | classic smiley `:)` · tongue-out `:P` · surprised `:O` · deadpan `:\|` · winking `;)` · kissy `:*` |
| **Eye** | round two-eye pair · single cyclops · eyes-closed `^_^` · raised eyebrow · starry ✨ · sleepy `zzz` |

For a 5-object set, you have 36 possible pairs — plenty of room to vary.

## Placement guidance

- The mouth button goes where the real control would naturally live: front face, top, or a dedicated button panel.
- The eye decal goes on a visually prominent flat or gently-curved surface: the cheek of a shell, the upper-left of a bezel, the center facelet of a cube face.
- If the object has a naturally symmetric pair of components (e.g., the twin bells on an alarm clock), those can read as eyes/ears *in addition to* the decal — but the decal is still required.

## Example pairings (for a 5-object set)

| Object | Mouth | Eye |
|---|---|---|
| PDA | smiley `:)` | round two-eye pair |
| Barcode scanner | tongue-out `:P` | single cyclops |
| Dustbuster vacuum | winking `;)` | eyes-closed `^_^` |
| Multimeter | deadpan `:\|` | raised eyebrow |
| Magic 8-ball | surprised `:O` | starry ✨ |

## Prompt language

Phrase the mouth in the prompt like this:

> *"one chunky round soft-touch rubber power button in candy-red molded as a [MOUTH GRAPHIC] graphic on the front bezel"*

Phrase the eye like this:

> *"one printed silkscreen decal of a [EYE GRAPHIC] applied to the surface on the upper-left cheek of the shell, simple 1990s sticker style with black outline and white glint, NOT sculpted"*

The "NOT sculpted" clause is load-bearing — without it the model sometimes extrudes the eye as 3D geometry, which reads weird and breaks the flat-decal Y2K feel.
