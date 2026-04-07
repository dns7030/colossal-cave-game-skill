# Chapter 8: Shell Room, Anteroom, Witt's End & Long Halls

**LOC_ARCHED** — Arched Hall
> You are in an arched hall. A coral passage once continued up and east from here, but is now blocked by debris. The air smells salty. A passage continues down and to the east.
- Short: You're in arched hall.
- Exits: down/shell/out→LOC_SHELLROOM
- DARK

**LOC_SHELLROOM** — Shell Room
> You're in a large room carved out of sedimentary rock. The floor and walls are littered with bits of shells embedded in the stone. A shallow passage proceeds downward, and a somewhat steeper one leads up. A low hands and knees passage leads north, and a final passage leads se.
- Short: You're in Shell Room.
- Default items: CLAM
- Exits: up/hall→LOC_ARCHED, down→LOC_SLOPING1, south/se→LOC_COMPLEX
- `open clam` → becomes OYSTER → `open oyster` → yields PEARL (treasure).
- DARK

**LOC_SLOPING1** — Sloping Corridor
> You are in a long sloping corridor with ragged sharp walls.
- Exits: up/shell→LOC_SHELLROOM, down→LOC_CULDESAC
- DARK

**LOC_CULDESAC** — Cul-de-sac
> You are in a cul-de-sac about eight feet across.
- Exits: up/out→LOC_SLOPING1, shell→LOC_SHELLROOM
- DARK

**LOC_ANTEROOM** — Anteroom
> You are in an anteroom leading to a large passage to the east. Small passages go west and up. A sign reads: "Cave under construction beyond this point. Proceed at own risk. [Witt Construction Company]"
- Short: You're in anteroom.
- Default items: MAGAZINE
- Exits: up→LOC_COMPLEX, west→LOC_BEDQUILT, east→LOC_WITTSEND
- DARK

**LOC_WITTSEND** — Witt's End
> You are at Witt's End. Passages lead off in *ALL* directions.
- Short: You're at Witt's End.
- Default items: VENDING (immovable)
- Exits: east→LOC_ANTEROOM, all other directions → futile 95% of the time (keep trying east to leave)
- DARK

**LOC_LONGEAST** — East End of Long Hall
> You are at the east end of a very long hall apparently without side chambers. To the east a low wide crawl slants up. To the north a round hole leads through a low cobbled passage.
- Short: You're at east end of long hall.
- Exits: east/up/crawl→LOC_MISTWEST, west→LOC_LONGWEST, north/down/hole→LOC_CROSSOVER
- DARK

**LOC_LONGWEST** — West End of Long Hall
> You are at the west end of a very long featureless hall. The hall joins up with a narrow north/south passage.
- Short: You're at west end of long hall.
- Exits: east→LOC_LONGEAST, north→LOC_CROSSOVER, south→LOC_DIFFERENT1
- DARK

**LOC_CROSSOVER** — Crossover
> You are at a crossover of a high n/s passage and a low e/w one.
- Exits: west→LOC_LONGEAST, north→LOC_DEADEND7, east→LOC_WESTSIDE, south→LOC_LONGWEST
- DARK

**LOC_DEADEND7** — Dead End
> Dead end.
- Exits: south/out→LOC_CROSSOVER
- DARK

## Maze of Twisting Passages (All Different)

All five rooms: "You are in a maze of twisting little passages, all different."
All DARK. Exits are asymmetric (different from the Alike maze).

**LOC_DIFFERENT1**
- Default items: SAPPHIRE (treasure)
- Exits: n→LOC_DIFFERENT2, s→LOC_DIFFERENT3, e→LOC_DIFFERENT4, w→LOC_LONGWEST, u→LOC_DIFFERENT5, d→LOC_DIFFERENT3

**LOC_DIFFERENT2**
- Exits: s→LOC_DIFFERENT1, n→LOC_DIFFERENT3, w→LOC_DIFFERENT4, e→LOC_DIFFERENT5, u→LOC_DIFFERENT3, d→LOC_DIFFERENT4

**LOC_DIFFERENT3**
- Default items: AMBER (treasure)
- Exits: n→LOC_DIFFERENT2, e→LOC_DIFFERENT1, s→LOC_DIFFERENT4, w→LOC_DIFFERENT5, u→LOC_DIFFERENT1, d→LOC_DIFFERENT5

**LOC_DIFFERENT4**
- Default items: SILVER (treasure — note: bars of silver are also in LOC_NORTHSIDE; use whichever is canonical for your run)
- Exits: n→LOC_DIFFERENT1, s→LOC_DIFFERENT5, e→LOC_DIFFERENT3, w→LOC_DIFFERENT2, u→LOC_DIFFERENT2, d→LOC_DIFFERENT1

**LOC_DIFFERENT5**
- Exits: n→LOC_DIFFERENT4, s→LOC_DIFFERENT2, e→LOC_DIFFERENT1, w→LOC_DIFFERENT3, u→LOC_DIFFERENT4, d→LOC_DIFFERENT2
