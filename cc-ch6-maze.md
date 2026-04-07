# Chapter 6: Maze of Twisty Little Passages (All Alike)

All rooms: "You are in a maze of twisty little passages, all alike."
Dead ends: "Dead end."
All DARK. Drop items to mark rooms — exits are asymmetric.

## Room Connections

**LOC_ALIKE1**
- Exits: n→LOC_ALIKE2, s→LOC_ALIKE4, e→LOC_ALIKE3, w→LOC_ALIKE3, u→LOC_ALIKE5, d→LOC_ALIKE3, ne→LOC_ALIKE3, se→LOC_ALIKE3, sw→LOC_ALIKE6, nw→LOC_ALIKE7, up/passage/climb→LOC_MISTWEST

**LOC_ALIKE2**
- Exits: n→LOC_ALIKE3, s→LOC_ALIKE3, e→LOC_ALIKE4, w→LOC_ALIKE1, u→LOC_ALIKE3, nw→LOC_ALIKE3

**LOC_ALIKE3**
- Exits: n→LOC_ALIKE3, s→LOC_MAZEEND9, e→LOC_ALIKE3, w→LOC_ALIKE3, u→LOC_ALIKE3, d→LOC_ALIKE4, ne→LOC_ALIKE3, se→LOC_ALIKE3, sw→LOC_ALIKE3, nw→LOC_ALIKE3

**LOC_ALIKE4**
- Exits: n→LOC_ALIKE1, s→LOC_ALIKE3, e→LOC_ALIKE3, w→LOC_ALIKE3, u→LOC_ALIKE3, d→LOC_ALIKE3, ne→LOC_ALIKE3, se→LOC_ALIKE3, nw→LOC_ALIKE3

**LOC_ALIKE5**
- Exits: n→LOC_ALIKE3, s→LOC_ALIKE3, e→LOC_ALIKE3, w→LOC_ALIKE3, u→LOC_ALIKE3, d→LOC_ALIKE1, ne→LOC_ALIKE3, se→LOC_ALIKE3, nw→LOC_ALIKE3

**LOC_ALIKE6**
- Exits: n→LOC_ALIKE3, s→LOC_ALIKE3, e→LOC_ALIKE3, w→LOC_ALIKE3, u→LOC_ALIKE3, d→LOC_ALIKE3, ne→LOC_ALIKE1, se→LOC_ALIKE3, sw→LOC_ALIKE3, nw→LOC_ALIKE3

**LOC_ALIKE7**
- Exits: n→LOC_ALIKE3, s→LOC_ALIKE3, e→LOC_ALIKE3, w→LOC_ALIKE3, u→LOC_ALIKE3, d→LOC_ALIKE3, ne→LOC_ALIKE3, se→LOC_ALIKE1, sw→LOC_ALIKE3, nw→LOC_ALIKE3

**LOC_ALIKE8**
- Exits: n→LOC_ALIKE9, e→LOC_ALIKE9, s→LOC_ALIKE3, w→LOC_ALIKE3, u→LOC_MAZEEND11, d→LOC_ALIKE3, sw→LOC_ALIKE3

**LOC_ALIKE9**
- Exits: n→LOC_ALIKE3, s→LOC_ALIKE8, e→LOC_ALIKE3, w→LOC_ALIKE8, ne→LOC_ALIKE3, nw→LOC_ALIKE3

**LOC_ALIKE10**
- Exits: w→LOC_PITBRINK, n→LOC_ALIKE3, e→LOC_ALIKE3, s→LOC_ALIKE3, u→LOC_ALIKE3, d→LOC_ALIKE3

**LOC_ALIKE11**
- Exits: n→LOC_ALIKE1, e→LOC_MAZEEND8, s→LOC_ALIKE11, w→LOC_ALIKE11

**LOC_ALIKE12**
- Exits: s→LOC_PITBRINK, e→LOC_ALIKE13, w→LOC_MAZEEND10, n→LOC_ALIKE3

**LOC_ALIKE13**
- Exits: n→LOC_PITBRINK, w→LOC_ALIKE12, nw→LOC_MAZEEND12, e→LOC_ALIKE3, s→LOC_ALIKE3

**LOC_ALIKE14**
- Exits: u→LOC_ALIKE4, d→LOC_ALIKE4

## Dead Ends
LOC_MAZEEND1 through LOC_MAZEEND12: all say "Dead end." Single exit back to the maze room they branch from.

## Key Maze Entry/Exit Points
- Enter maze: from LOC_MISTWEST south/climb → LOC_ALIKE1
- Enter maze: from LOC_PITBRINK → LOC_ALIKE10 (west), LOC_ALIKE12 (north), LOC_ALIKE13 (north)
- Exit maze: LOC_ALIKE1 → LOC_MISTWEST (south/up/passage)
- Exit maze: LOC_ALIKE10 → LOC_PITBRINK (west)

## LOC_PITBRINK — Brink of Pit
> You are on the brink of a thirty foot pit with a massive orange column down one wall. Cavernous passages lead east, west, and north.
- Short: You're at brink of pit.
- Exits: down/climb→LOC_BIRDCHAMBER, west→LOC_ALIKE10, south→LOC_MAZEEND6, north→LOC_ALIKE12, east→LOC_ALIKE13
- DARK
