# Chapter 3: Hall of Mists & Y2 Area

**LOC_MISTHALL** — Hall of Mists
> You are at one end of a vast hall stretching forward out of sight to the west. There are openings to either side. Nearby, a wide stone staircase leads downward. The hall is filled with wisps of white mist swaying to and fro almost as if alive.
- Short: You're in Hall of Mists.
- Exits: left/south→LOC_NUGGET, forward/hall/west→LOC_EASTBANK, stairs/down/north→LOC_KINGHALL, up/pit/steps/east (if carrying NUGGET)→(can't get nugget up steps), up/steps→LOC_PITTOP, y2→LOC_JUMBLE
- DARK

**LOC_EASTBANK** — East Bank of Fissure
> You are on the east bank of a fissure slicing clear across the hall. The mist is quite thick here, and the fissure is too wide to jump.
- Short: You're on east bank of fissure.
- Exits: hall/east→LOC_MISTHALL, over/across/west/cross (if fissure_bridged)→LOC_WESTBANK
- `wave rod` to create/destroy crystal bridge. Cannot jump across.
- DARK

**LOC_NUGGET** — Nugget of Gold Room
> This is a low room with a crude note on the wall. The note says, "You won't get it up the steps."
- Short: You're in nugget-of-gold room.
- Default items: NUGGET
- Exits: hall/out/north→LOC_MISTHALL
- DARK

**LOC_WESTBANK** — West Bank of Fissure
> You are on the west side of the fissure in the Hall of Mists.
- Short: You're on west bank of fissure.
- Exits: over/across/east/cross (if fissure_bridged)→LOC_EASTBANK, north→LOC_PARALLEL1, west→LOC_MISTWEST
- DARK

**LOC_PARALLEL1** — Low Wide Passage (north crawl)
> You have crawled through a very low wide passage parallel to and north of the Hall of Mists.
- Exits: (any)→LOC_MISTWEST

**LOC_PARALLEL2** — Low Wide Passage (south crawl)
> You have crawled through a very low wide passage parallel to and north of the Hall of Mists.
- Exits: (any)→LOC_WESTBANK

**LOC_MISTWEST** — West End of Hall of Mists
> You are at the west end of the Hall of Mists. Low wide crawl continues west and another goes north. To the south is a small passage six feet off the floor.
- Exits: south/up/passage/climb→LOC_ALIKE1, east→LOC_WESTBANK, north→LOC_PARALLEL2, west/crawl→LOC_LONGEAST
- DARK

**LOC_JUMBLE** — Jumble of Rock
> In a jumble of rock, with cracks everywhere.
- Exits: down/y2→LOC_Y2, up→LOC_MISTHALL
- DARK

**LOC_Y2** — Y2
> Large room with passages to south and west, and wall of broken rock to the east. There is a large "Y2" on a rock in the center of the room.
- Exits: plugh→LOC_BUILDING, south→LOC_FLOORHOLE, east/wall/broken→LOC_JUMBLE, west→LOC_WINDOW1, plover (carrying EMERALD)→LOC_PLOVER
- DARK

**LOC_WINDOW1** — Window on Pit (north side)
> You're at a low window overlooking a huge pit, which extends up out of sight. Across the pit, the window on the other side can barely be seen.
- Exits: east/y2→LOC_Y2, jump→(death — broken neck)
- DARK

**LOC_FLOORHOLE** — N/S Passage above E/W Passage
> You are in a low n/s passage at a hole in the floor. The hole goes down to an e/w passage.
- Short: You're in n/s passage above e/w passage.
- Exits: hall/out/south→LOC_KINGHALL, north/y2→LOC_Y2, down/hole→(fall — broken neck)
- DARK

**LOC_NORTHSIDE** — North Side Chamber
> You are in a small chamber just north of the Hall of the Mountain King. A low corridor leads north.
- Default items: SILVER
- Exits: south→LOC_KINGHALL, north→LOC_MISTHALL
- DARK
