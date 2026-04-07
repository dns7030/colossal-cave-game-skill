# Colossal Cave — Master Index

Source: Eric Raymond's Open Adventure (BSD-2-Clause), faithful to the Woods/Crowther 1977 expansion.
Always load this file first when starting Colossal Cave. Load chapter files on demand as the player moves.

---

## Chapter Map

When the player enters a room not in the currently loaded chapter, read the corresponding file.

| Chapter File | Room IDs |
|---|---|
| cc-ch1-surface.md | LOC_START, LOC_HILL, LOC_BUILDING, LOC_VALLEY, LOC_ROADEND, LOC_SLIT, LOC_GRATE, LOC_FOREST*, LOC_SEWER |
| cc-ch2-entrance.md | LOC_BELOWGRATE, LOC_COBBLE, LOC_DEBRIS, LOC_AWKWARD, LOC_BIRDCHAMBER, LOC_PITTOP, LOC_CRACK |
| cc-ch3-mists.md | LOC_MISTHALL, LOC_EASTBANK, LOC_NUGGET, LOC_WESTBANK, LOC_PARALLEL1, LOC_PARALLEL2, LOC_MISTWEST, LOC_JUMBLE, LOC_Y2, LOC_WINDOW1, LOC_FLOORHOLE, LOC_NORTHSIDE |
| cc-ch4-king.md | LOC_KINGHALL, LOC_SOUTHSIDE, LOC_WESTSIDE, LOC_SECRET1, LOC_SECRET2, LOC_SECRET3, LOC_SECRET4, LOC_SECRET5, LOC_SECRET6, LOC_WIDEPLACE, LOC_TIGHTPLACE, LOC_TALL, LOC_BOULDERS1 |
| cc-ch5-twopit.md | LOC_WESTEND, LOC_EASTEND, LOC_WESTPIT, LOC_EASTPIT, LOC_NARROW, LOC_SLAB, LOC_GIANTROOM, LOC_CAVEIN, LOC_IMMENSE, LOC_WATERFALL, LOC_INCLINE |
| cc-ch6-maze.md | LOC_ALIKE1–LOC_ALIKE14, LOC_MAZEEND1–LOC_MAZEEND12, LOC_PITBRINK |
| cc-ch7-bedquilt.md | LOC_COMPLEX, LOC_DUSTY, LOC_BEDQUILT, LOC_SWISSCHEESE, LOC_SOFTROOM, LOC_ORIENTAL, LOC_MISTY, LOC_ALCOVE, LOC_PLOVER, LOC_DARKROOM |
| cc-ch8-shell.md | LOC_ARCHED, LOC_SHELLROOM, LOC_SLOPING1, LOC_CULDESAC, LOC_ANTEROOM, LOC_WITTSEND, LOC_LONGEAST, LOC_LONGWEST, LOC_CROSSOVER, LOC_DEADEND7, LOC_DIFFERENT1–LOC_DIFFERENT5 |
| cc-ch9-deepcave.md | LOC_LOWROOM, LOC_DEADCRAWL, LOC_SWCHASM, LOC_WINDING, LOC_NECHASM, LOC_CORRIDOR, LOC_FORK, LOC_WARMWALLS, LOC_BREATHTAKING, LOC_BOULDERS2, LOC_LIMESTONE, LOC_BARRENFRONT, LOC_BARRENROOM |
| cc-ch10-reservoir.md | LOC_THREEJUNCTION, LOC_WINDOW2, LOC_TOPSTALACTITE, LOC_MIRRORCANYON, LOC_RESERVOIR, LOC_RESBOTTOM, LOC_RESNORTH, LOC_TREACHEROUS, LOC_STEEP, LOC_BROKEN |

---

## Goal & Magic Words

Collect all 15 treasures and deposit them at LOC_BUILDING (Well House). Magic words:
- **XYZZY** — teleports between LOC_BUILDING and LOC_DEBRIS
- **PLUGH** — teleports between LOC_BUILDING and LOC_Y2
- **PLOVER** — teleports between LOC_PLOVER and LOC_Y2 (requires carrying EMERALD)

Lamp required in all dark rooms. Does not run out (Layer 1).

---

## Treasures (15 total — deposit all at Well House)

| ID | Name | Starting Location |
|---|---|---|
| NUGGET | Large gold nugget | LOC_NUGGET |
| DIAMONDS | Several diamonds | LOC_WESTSIDE |
| SILVER | Bars of silver | LOC_NORTHSIDE |
| JEWELRY | Precious jewelry | LOC_SOUTHSIDE |
| COINS | Rare coins | LOC_WESTEND |
| EGGS | Golden eggs | LOC_GIANTROOM |
| TRIDENT | Jeweled trident | LOC_MISTY |
| VASE | Ming vase (fragile) | LOC_ORIENTAL |
| EMERALD | Egg-sized emerald | LOC_PLOVER |
| PYRAMID | Crystal pyramid | LOC_DARKROOM |
| PEARL | Glistening pearl | inside OYSTER (in LOC_SHELLROOM) |
| RUG | Persian rug | LOC_ORIENTAL |
| SPICES | Rare spices | LOC_BIRDCHAMBER |
| CHAIN | Golden chain | LOC_BARRENROOM (on bear) |
| JADE | Jade necklace | LOC_SWCHASM (troll drops it) |

---

## Non-Treasure Objects

| ID | Name | Start | Use |
|---|---|---|---|
| KEYS | Set of keys | LOC_BUILDING | Unlock grate |
| LAMP | Brass lantern | LOC_BUILDING | Light dark rooms (`lamp on` / `on`) |
| CAGE | Wicker cage | LOC_COBBLE | Catch bird |
| ROD | Black rod | LOC_DEBRIS | Wave → crystal bridge at fissure |
| BIRD | Little bird | LOC_BIRDCHAMBER | Catch with cage; frightens snake |
| FOOD | Tasty food | LOC_BUILDING | Tame bear |
| BOTTLE | Bottle of water | LOC_BUILDING | Water plant; fill at stream |
| PILLOW | Velvet pillow | LOC_SOFTROOM | Cushion vase drop |
| SNAKE | Fierce snake | LOC_KINGHALL | Immovable; bird frightens away |
| FISSURE | Crystal bridge | LOC_EASTBANK | Immovable; wave rod to toggle |
| TABLET | Stone tablet | LOC_DARKROOM | Immovable; reads "MAGIC WORD XYZZY" |
| CLAM | Giant clam | LOC_SHELLROOM | Force open → OYSTER → PEARL |
| PLANT | Beanstalk | LOC_WESTPIT | Water twice → climable to LOC_NARROW |
| BEAR | Cave bear | LOC_BARRENROOM | Feed food → tamed; drives troll away |
| TROLL | Ugly troll | LOC_SWCHASM | Blocks chasm; driven off by bear |
| DRAGON | Fierce dragon | LOC_SECRET4 | Say YES to fight → dies |
| MAGAZINE | "Spelunker Today" | LOC_ANTEROOM | Readable flavor item |
| VENDING | Vending machine | LOC_DIFFERENT1 | Immovable |

---

## Puzzle Rules

**Grate**: Need KEYS → `unlock grate` at LOC_GRATE → enter LOC_BELOWGRATE

**Fissure bridge**: Need ROD → `wave rod` at LOC_EASTBANK or LOC_WESTBANK → bridge appears/disappears

**Snake** (LOC_KINGHALL): Need BIRD in CAGE → carry into hall → snake flees permanently. Cannot catch bird while carrying rod.

**Plant** (LOC_WESTPIT): Need BOTTLE with water → `pour water` → water twice for full growth → climb stalk to LOC_NARROW

**Dragon** (LOC_SECRET4): Answer `yes` when asked to fight → dragon dies. No weapon needed.

**Troll** (LOC_SWCHASM): Option A: throw treasure at troll (lose it). Option B: lead tamed bear → troll flees, drops JADE.

**Bear** (LOC_BARRENROOM): `feed bear` with FOOD → tamed, follows you, CHAIN becomes takeable.

**Oyster/Pearl**: `open clam` at LOC_SHELLROOM → becomes OYSTER → `open oyster` → yields PEARL.

**Vase**: Fragile. Drop PILLOW in room first, then drop VASE → safe landing.

**Plover Room**: Enter from LOC_ALCOVE east (light inventory only), or say `plover` while carrying EMERALD at LOC_Y2.

---

## Starting State (new game)

```json
{
  "game": "colossal-cave",
  "version": 1,
  "current_room": "LOC_START",
  "current_chapter": "cc-ch1-surface.md",
  "inventory": [],
  "lamp_lit": false,
  "visited": [],
  "room_items_delta": {},
  "puzzle_state": {
    "grate_locked": true,
    "fissure_bridged": false,
    "snake_gone": false,
    "dragon_alive": true,
    "troll_present": true,
    "bear_tamed": false,
    "plant_watered": 0,
    "oyster_open": false,
    "treasures_deposited": []
  },
  "score": 0
}
```

`room_items_delta` only stores rooms where items have moved from their default position. Default positions are in the Treasures and Objects tables above.

---

## Scoring

- Each treasure deposited at LOC_BUILDING = 12 points (15 × 12 = 180 max)
- Rooms visited bonus (up to ~100 points)
- Max score = ~350 points
- `score` command shows current score

---

## Opening Text

```
COLOSSAL CAVE ADVENTURE
Original by Will Crowther (1976) & Don Woods (1977)
This port: Layer 1 (faithful map, no dwarf AI or lamp timer)

Somewhere nearby is Colossal Cave, where others have found fortunes in
treasure and gold, though it is rumored that some who enter are never
seen again. Magic is said to work in the cave. I will be your eyes and
hands. Direct me with commands of 1 or 2 words.
─────────────────────────────────────────
```
