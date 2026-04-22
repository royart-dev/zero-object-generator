# Modes — A / B / C Input Handling

The skill handles three input modes. Identifying the mode first is the single biggest efficiency gain — it determines whether you write the prompt immediately or confirm first.

## Mode A — Named object

The user has already picked the object.

> *"Render a walkie-talkie in our style."*
> *"Make an NB2 prompt for a Casio calculator."*
> *"Do a dustbuster."*

**What to do:** Go straight to the prompt. No confirmation step. The user named the object; second-guessing it wastes a turn. Move to the 6-layer structure (see `rules.md`).

The one exception: if the named object has a **locked color pairing** (see `palette.md`), silently apply it. If it doesn't, pick an approved color that suits the object and proceed.

## Mode B — Concept

The user described an idea, a feeling, a UI state, or a category — not an object.

> *"I need a hero image for the empty search state — something that feels like 'nothing to find yet.'"*
> *"Give me a visual for trust."*
> *"Render something that represents patience."*
> *"Course card for a module on debugging."*

**What to do:** Pick an object that carries the concept, then **confirm back in one line before writing the prompt.**

> *"I'll render a magnifying glass with a tiny 'no results' LCD readout — does that work, or would you rather a different object?"*

This one-line check is cheap. It saves a wasted render when your object pick doesn't match what the user had in mind. Wait for confirmation (or a pivot), then write the prompt.

When picking, prefer objects that already have a locked pairing or an obvious Y2K form. A barcode scanner reads as "scan" more instantly than a sextant does.

## Mode C — Reference image

The user dropped an image and asked for "our style," "this in Zero," or "make a render version of this."

> *[attaches a photo of a retro camera]* *"Do this in our style."*
> *[attaches a screenshot of a concept sketch]* *"Render this."*

**What to do:** Two steps.

1. **Identify the object.** Name it back in one line: *"That's a late-90s Polaroid i-Zone — want me to render it?"* — this catches the case where you misread the image.
2. **Strip the reference's aesthetic.** The user wants the *object* from the image, not its materials, lighting, mood, or color. Discard:
   - Source image's palette (unless it happens to be an approved tint — confirm, don't assume)
   - Source image's lighting / grading / film look
   - Source image's background, surface, shadow, props
   - Source image's wear, patina, age, scratches
   - Source image's brand marks, logos, visible text

   Then apply the Zero palette + jelly shell + face formula + 6-layer structure from scratch, as if the object had been named in Mode A.

The failure mode to avoid: carrying the reference image's aesthetic into the prompt. If the reference is a dusty 1970s calculator shot on film, the render should NOT be dusty, beige, or film-graded — it should be candy-saturated jelly shell with a face, factory-fresh, on pure white.

## Quick decision tree

```
User input has an image attached?
├── Yes → Mode C (identify + strip + confirm)
└── No
    ├── Input names a specific object? → Mode A (go)
    └── Input describes a concept/feeling/state? → Mode B (pick object + confirm)
```

## Confirmation phrasing

Keep the confirm line to one sentence. Don't list options unless the user's brief is genuinely ambiguous across 2-3 equally-strong candidates.

Good:
> *"I'll render a Polaroid i-Zone in candy-coral jelly — sound right?"*

Bad:
> *"I could render this as a Polaroid, or a disposable camera, or a point-and-shoot, or a Game Boy Camera — which do you prefer? Also, what color? And should it have a face?"*

The one-line confirm is a redirect point, not a design meeting.
