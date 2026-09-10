# Family Zoo — v04 — Portable Objects

Introduces takeable items — a zoo map, a bag of feed, a souvenir penny — that the player can pick up, carry between rooms, and drop. Establishes that portability is the default and SceneryTrait is what removes it.

Step 4 of the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial — a progressive walkthrough of the [Sharpee](https://sharpee.net) TypeScript interactive fiction engine, from a single room to a full multi-file story.

## What this step teaches

- EntityType.ITEM for portable objects
- Built-in take, drop, inventory, and take all actions
- Items traveling with the player automatically
- Loose objects appearing in room listings
- The portable-by-default design philosophy

## Playing

Open `play.html`, or preview the folder:

```bash
python -m http.server 8000 --directory familyzoo-v04
```

## Building

This is a **frozen 0.9.x TypeScript version**. The built player in this folder is the published artifact; it is re-laid from `browser/` by the workspace build:

```bash
python ../tools/build.py familyzoo-v04
python C:/code/ifhub/tools/ship.py familyzoo-v04
```

The authoring tree for every version lives in the [familyzoo](https://github.com/Johnesco/familyzoo) repo.
