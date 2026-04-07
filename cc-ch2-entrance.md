# Chapter 2: Cave Entrance

**LOC_BELOWGRATE** — Below the Grate
> You are in a small chamber beneath a 3x3 steel grate to the surface. A low crawl over cobbles leads inward to the west.
- Short: You're below the grate.
- Exits: up/out (if unlocked)→LOC_GRATE, crawl/cobbles/west→LOC_COBBLE, pit→LOC_PITTOP, debris→LOC_DEBRIS
- DARK (need lamp)

**LOC_COBBLE** — Cobble Crawl
> You are crawling over cobbles in a low passage. There is a dim light at the east end of the passage.
- Short: You're in cobble crawl.
- Default items: CAGE
- Exits: out/surface/east→LOC_BELOWGRATE, west/dark/debris→LOC_DEBRIS, pit→LOC_PITTOP

**LOC_DEBRIS** — Debris Room
> You are in a debris room filled with stuff washed in from the surface. A low wide passage with cobbles becomes plugged with mud and debris here, but an awkward canyon leads upward and west. A note on the wall says "Magic Word XYZZY."
- Short: You're in debris room.
- Default items: ROD
- Exits: depression→LOC_GRATE, entrance→LOC_BELOWGRATE, crawl/cobbles/east→LOC_COBBLE, canyon/west/up→LOC_AWKWARD, xyzzy→LOC_BUILDING, pit→LOC_PITTOP
- DARK

**LOC_AWKWARD** — Awkward Canyon
> You are in an awkward sloping east/west canyon.
- Exits: depression→LOC_GRATE, entrance→LOC_BELOWGRATE, east/debris→LOC_DEBRIS, west/up→LOC_BIRDCHAMBER, pit→LOC_PITTOP
- DARK

**LOC_BIRDCHAMBER** — Bird Chamber
> You are in a splendid chamber thirty feet high. The walls are frozen rivers of orange stone. An awkward canyon and a good passage exit from east and west sides of the chamber.
- Short: You're in bird chamber.
- Default items: BIRD, SPICES
- Exits: depression→LOC_GRATE, entrance→LOC_BELOWGRATE, debris→LOC_DEBRIS, canyon/east→LOC_AWKWARD, passage/pit/west→LOC_PITTOP
- Cannot catch BIRD while carrying ROD (bird is afraid of rod).
- DARK

**LOC_PITTOP** — Top of Small Pit
> At your feet is a small pit breathing traces of white mist. An east passage ends here except for a small crack leading on.
- Short: You're at top of small pit.
- Exits: depression→LOC_GRATE, entrance→LOC_BELOWGRATE, debris→LOC_DEBRIS, passage/east→LOC_BIRDCHAMBER, down/pit/steps→LOC_MISTHALL, crack/west→LOC_CRACK
- DARK

**LOC_CRACK** — Crack in Wall
> The crack is far too small for you to follow.
- Exits: (any)→LOC_PITTOP
