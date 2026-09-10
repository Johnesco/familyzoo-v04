# v04 — Portable Objects

The first things the player can carry: a brochure, a map, a souvenir penny. Also the first phrase block — the brochure's text is set verbatim so its layout survives.

## What this step adds

- A thing with no `scenery` is takeable by default
- `readable` and `on the player reading`
- `define phrase brochure-text, verbatim` — text kept exactly as written
- TAKE, DROP and INVENTORY come from the standard library

## The source

The whole step is one file: [`familyzoo-v04.story`](../familyzoo-v04.story). Read it top to bottom — it is the previous step plus what is listed above.

## Running it

```bash
npx sharpee play
npx sharpee test          # replays familyzoo-v04.tests.json
```

Chord language reference: <https://sharpee.net/chord/>
