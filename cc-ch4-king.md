# Chapter 4: Hall of Mountain King & Secret Canyons

**LOC_KINGHALL** — Hall of the Mountain King
> You are in the Hall of the Mountain King, with passages off in all directions.
- Short: You're in Hall of Mt King.
- Default items: SNAKE (immovable)
- Exits: stairs/up/east→LOC_MISTHALL, north/right (if snake_gone)→LOC_FLOORHOLE, south/left (if snake_gone)→LOC_SOUTHSIDE, west/forward (if snake_gone)→LOC_WESTSIDE, secret→LOC_SECRET3
- Snake blocks north/south/west. Carry caged BIRD in → snake flees permanently.
- DARK

**LOC_SOUTHSIDE** — South Side Chamber
> You are in the south side chamber.
- Default items: JEWELRY
- Exits: hall/out/north→LOC_KINGHALL
- DARK

**LOC_WESTSIDE** — West Side Chamber
> In the west side chamber of the Hall of the Mountain King. A passage continues west and up here.
- Default items: DIAMONDS
- Exits: hall/out/east→LOC_KINGHALL, west/up→LOC_CROSSOVER
- DARK

**LOC_SECRET3** — Secret E/W Canyon (above tight canyon)
> You are in a secret canyon which here runs e/w. It crosses over a very tight canyon 15 feet below. If you go down you may get stuck.
- Short: You're in secret e/w canyon above tight canyon.
- Exits: east→LOC_KINGHALL, west→LOC_SECRET5, down→LOC_WIDEPLACE
- DARK

**LOC_WIDEPLACE** — Wide Place in Canyon
> You are at a wide place in a very tight n/s canyon.
- Exits: south→LOC_TIGHTPLACE, north→LOC_TALL
- DARK

**LOC_TIGHTPLACE** — Tight Canyon
> The canyon here becomes too tight to go further south.
- Exits: north→LOC_WIDEPLACE
- DARK

**LOC_TALL** — Tall E/W Canyon
> You are in a tall e/w canyon. A low tight crawl goes 3 feet north and seems to open up.
- Exits: east→LOC_WIDEPLACE, west→LOC_BOULDERS1, north/crawl→LOC_SWISSCHEESE
- DARK

**LOC_BOULDERS1** — Dead End (boulders)
> The canyon runs into a mass of boulders — dead end.
- Exits: south→LOC_TALL
- DARK

**LOC_SECRET1** — Secret N/S Canyon above Large Room
> You are in a secret n/s canyon above a large room.
- Exits: down/slab→LOC_SLAB, south→LOC_SECRET5, north→LOC_MIRRORCANYON, reservoir→LOC_RESERVOIR
- DARK

**LOC_SECRET2** — Secret N/S Canyon above Passage
> You are in a secret n/s canyon above a sizable passage.
- Exits: north→LOC_THREEJUNCTION, down/passage→LOC_BEDQUILT, south→LOC_TOPSTALACTITE
- DARK

**LOC_SECRET4** — Secret Canyon (dragon blocks east)
> You are in a secret canyon which exits to the north and east.
- Default items: DRAGON (immovable, blocks east)
- Exits: north/out→LOC_SECRET1, east (if dragon defeated)→LOC_SECRET5
- Answer `yes` when asked to fight dragon → dragon dies.
- DARK

**LOC_SECRET5** — Secret Canyon (middle)
> You are in a secret canyon which exits to the north and east.
- Exits: north→LOC_SECRET1, east→LOC_SECRET3
- DARK

**LOC_SECRET6** — Secret Canyon (western end)
> You are in a secret canyon which exits to the east and north.
- Exits: east/out→LOC_SECRET3, north (blocked by dragon if alive)→(dragon blocks)
- DARK
