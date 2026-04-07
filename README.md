# Colossal Cave Adventure

> *"Somewhere nearby is Colossal Cave, where others have found fortunes in treasure and gold, though it is rumored that some who enter are never seen again. Magic is said to work in the cave."*

Play the game that invented the text adventure genre — directly inside Claude. No browser, no emulator, no setup.

---

## What is this?

**Colossal Cave Adventure** (1976/1977) by Will Crowther and Don Woods is the grandfather of every RPG, dungeon crawler, and adventure game ever made. Zork, Nethack, Baldur's Gate — they all trace their DNA back to this cave.

This skill brings it to life inside Claude chat with full save/load support and faithful puzzle logic.

---

## How to play

Type `/text-rpg` in any Claude session. The game starts immediately.

```
COLOSSAL CAVE ADVENTURE

Somewhere nearby is Colossal Cave, where others have found fortunes in
treasure and gold, though it is rumored that some who enter are never
seen again. Magic is said to work in the cave.
─────────────────────────────────────────

Road End
You are standing at the end of a road before a small brick building.
Around you is a forest. A small stream flows out of the building and
down a gully.

Exits: west, enter/east, south/down, north, depression
Carrying: nothing
```

Commands are plain English: `go north`, `take lamp`, `unlock grate`, `wave rod`, `feed bear`. One or two words, just like the original.

---

## What's inside

- **130+ rooms** across 10 geographic areas: the surface, cave entrance, Hall of Mists, Hall of the Mountain King, the Twopit Room, a maze of twisty passages (all alike), Bedquilt, the Shell Room, the deep cave, and the underground reservoir
- **15 treasures** to find and carry back to the Well House: gold nuggets, diamonds, a Ming vase, a Persian rug, a glistening pearl, and more
- **Classic puzzles** — all faithfully implemented:
  - Unlock the grate with the keys
  - Light dark rooms with the brass lantern
  - Wave the rod to raise a crystal bridge over the fissure
  - Catch the bird, use it to frighten the snake
  - Water the plant twice to grow a beanstalk
  - Say YES to fight the dragon (no weapon needed — that's the puzzle)
  - Tame the bear with food, lead it to the troll bridge
  - Navigate the maze by dropping items as markers
- **Magic words**: XYZZY, PLUGH, PLOVER — teleport between key locations
- **Save / Load** — progress persists between sessions

---

## Tips for new players

1. Start at the building — pick up everything inside
2. Find the depression in the forest and unlock the grate
3. Light your lamp before going underground
4. The note in the debris room is a hint
5. Dropping items in the maze is the only way to map it
6. Some puzzles require items you haven't found yet — explore widely before concluding something is impossible

---

## Technical notes

- World data is split into 10 chapter files loaded on demand — no token limit issues
- Save files stored at `~/.claude/saves/colossal-cave.json`
- Layer 1 port: full map and all puzzles, no dwarf AI or lamp timer (those are Layer 2)
- Source: Eric Raymond's Open Adventure (BSD-2-Clause), faithful to the 1977 Woods expansion

---

## What's coming (Layer 2)

- Roaming dwarves that throw axes
- The pirate who steals your treasures
- Lamp oil timer (330 turns)
- Cave closing endgame sequence
- Score classification messages

---

*This skill contains no API keys, no external calls, and no tracking. Just you, the cave, and your wits.*
