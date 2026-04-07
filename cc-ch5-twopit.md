# Chapter 5: Twopit Room, Beanstalk & Giant Room

**LOC_WESTEND** — West End of Twopit Room
> You are at the west end of the Twopit Room. There is a large hole in the floor. Through it you can see a profusion of leaves. Two passages exit from east and west ends of the room.
- Short: You're at west end of Twopit Room.
- Default items: COINS
- Exits: east/across→LOC_EASTEND, west/slab→LOC_SLAB, down/pit→LOC_WESTPIT
- DARK

**LOC_EASTEND** — East End of Twopit Room
> You are at the east end of the Twopit Room. The floor here is littered with thin shards of orange rock. In the pit, the top of a stalactite is visible.
- Short: You're at east end of Twopit Room.
- Exits: east→LOC_SWISSCHEESE, west/across→LOC_WESTEND, down/pit→LOC_EASTPIT
- DARK

**LOC_WESTPIT** — West Pit
> You are at the bottom of the western pit in the Twopit Room. There is a large hole in the wall.
- Short: You're in west pit.
- Default items: PLANT (immovable)
- Exits: up/out→LOC_WESTEND, climb (if plant_watered >= 2)→LOC_NARROW
- Pour water on plant twice to grow it to ceiling. Then climb.
- DARK

**LOC_EASTPIT** — East Pit
> You are at the bottom of the eastern pit in the Twopit Room. There is a small pool of oil in one corner of the pit.
- Short: You're in east pit.
- Exits: up/out→LOC_EASTEND
- Fill bottle with oil here (alternative to water).
- DARK

**LOC_NARROW** — Narrow Corridor
> You are in a long, narrow corridor stretching out of sight to the west. A rock bears a scrawled note: "Do not step on the grass."
- Short: You're in narrow corridor.
- Exits: down/climb/east→LOC_WESTPIT, west/giant→LOC_GIANTROOM
- DARK

**LOC_SLAB** — Slab Room
> You are in a large low circular chamber whose floor is an immense slab fallen from the ceiling. The air smells damp, and there is a continuing sound of dripping water.
- Short: You're in Slab Room.
- Exits: south→LOC_WESTEND, up/climb→LOC_SECRET1, north→LOC_BEDQUILT
- DARK

**LOC_GIANTROOM** — Giant Room
> You are in the Giant Room. The ceiling here is too high up for your lamp to illuminate it. Cavernous passages lead east, north, and south. On the west wall is scrawled the inscription, "Fee Fie Foe Foo" [sic].
- Short: You're in Giant Room.
- Default items: EGGS
- Exits: south→LOC_NARROW, east→LOC_CAVEIN, north→LOC_IMMENSE
- DARK

**LOC_CAVEIN** — Cave-in Passage
> The passage here is blocked by a recent cave-in.
- Exits: south/giant/out→LOC_GIANTROOM
- DARK

**LOC_IMMENSE** — Immense N/S Passage
> You are at one end of an immense north/south passage.
- Exits: south/giant→LOC_GIANTROOM, north/enter/cavern (if lamp lit)→LOC_WATERFALL
- DARK

**LOC_WATERFALL** — Cavern with Waterfall
> You are in a magnificent cavern with a rushing stream, which cascades over a sparkling waterfall into a roaring whirlpool which disappears through a hole in the floor. Passages exit to the south and west.
- Short: You're in cavern with waterfall.
- Exits: south/out→LOC_IMMENSE, giant→LOC_GIANTROOM, west→LOC_INCLINE
- DARK

**LOC_INCLINE** — Steep Incline above Large Room
> You are at the top of a steep incline above a large room. You could climb down here, and you see passages leading further uphill to the north.
- Short: You're at steep incline above large room.
- Exits: north/cavern/passage→LOC_WATERFALL, down/climb→LOC_LOWROOM
- DARK
