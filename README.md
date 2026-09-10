# Family Zoo — v04: Portable Objects

The first things the player can carry: a brochure, a map, a souvenir penny. Also the first phrase block — the brochure's text is set verbatim so its layout survives.

Step 4 of sixteen in the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial for [Chord](https://sharpee.net/chord/), the authoring language of the [Sharpee](https://sharpee.net) interactive fiction engine.

## What this step adds

- A thing with no `scenery` is takeable by default
- `readable` and `on the player reading`
- `define phrase brochure-text, verbatim` — text kept exactly as written
- TAKE, DROP and INVENTORY come from the standard library

## The source

The whole step is one file: [`familyzoo-v04.story`](./familyzoo-v04.story) — the step before it plus the ideas above. The chapter that walks through it is [`docs/v04-portable-objects.md`](./docs/v04-portable-objects.md).

## Playing and testing

```bash
npx sharpee play
npx sharpee test          # replays familyzoo-v04.tests.json
python ../tools/build.py familyzoo-v04 --force
```

## Engine

Pinned to `@sharpee/*` **5.3.0** (Chord 3.6.0), held there by an `overrides` block: 5.3.1 publishes broken subpath exports and breaks `sharpee test`.

The 0.9.x TypeScript edition this replaced is kept in [`legacy/`](./legacy).
