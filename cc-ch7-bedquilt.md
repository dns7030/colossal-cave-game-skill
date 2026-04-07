# Chapter 7: Bedquilt, Swiss Cheese, Oriental & Plover

**LOC_COMPLEX** — Complex Junction
> You are at a complex junction. A low hands and knees passage from the north joins a higher crawl from the east to make a walking passage going west. There is also a small passage going northeast.
- Short: You're at complex junction.
- Exits: up/climb/room→LOC_DUSTY, west/bedquilt→LOC_BEDQUILT, north/shell→LOC_SHELLROOM, east→LOC_ANTEROOM
- DARK

**LOC_DUSTY** — Dusty Rock Room
> Large room full of dusty rocks. Big hole in floor. Cracks everywhere, passage leading east.
- Exits: east/passage→LOC_BROKEN, down/hole/floor→LOC_COMPLEX, bedquilt→LOC_BEDQUILT
- DARK

**LOC_BEDQUILT** — Bedquilt
> You are in Bedquilt, a long east/west passage with holes everywhere. To explore at random select north, south, up or down.
- Short: You're in Bedquilt.
- Exits: west/slab→LOC_SLAB, east/complex→LOC_COMPLEX, north→LOC_DUSTY (60%) or dead end, south→LOC_SECRET2 (25%) or dead end, up→LOC_SECRET1 (50%) or dead end, down→LOC_SWISSCHEESE (75%) or dead end
- DARK

**LOC_SWISSCHEESE** — Swiss Cheese Room
> You are in a room whose walls resemble Swiss cheese. Obvious passages go west, ne, and se, less obvious ones go north and east.
- Short: You're in Swiss Cheese Room.
- Exits: ne→LOC_BEDQUILT, west→LOC_EASTEND, canyon→LOC_TALL, east→LOC_SOFTROOM, oriental/se→LOC_ORIENTAL
- DARK

**LOC_SOFTROOM** — Soft Room
> You are in the Soft Room. The walls are covered with heavy curtains of cave flower. A passage leads west.
- Short: You're in Soft Room.
- Default items: PILLOW
- Exits: west/out→LOC_SWISSCHEESE
- DARK

**LOC_ORIENTAL** — Oriental Room
> This is the Oriental Room. Ancient oriental cave drawings cover the walls. A recently hewn tunnel exits to the north, and a narrower one to the south. A low crawl exits to the west.
- Short: You're in Oriental Room.
- Default items: VASE, RUG
- Exits: se→LOC_SWISSCHEESE, west/crawl→LOC_LOWROOM, up/north/cavern→LOC_MISTY
- VASE is fragile: drop PILLOW first, then drop VASE safely.
- DARK

**LOC_MISTY** — Misty Cavern
> You are following a wide path around the outer edge of a large cavern. Far below, through a heavy white mist, strange reflections hint at a lake.
- Short: You're in misty cavern.
- Default items: TRIDENT
- Exits: south/oriental→LOC_ORIENTAL, west→LOC_ALCOVE
- DARK

**LOC_ALCOVE** — Alcove
> You are in an alcove. A small nw path seems to widen after a short distance. An extremely tight tunnel leads east. It looks like a very tight squeeze. An easier passage leads west.
- Short: You're in alcove.
- Exits: nw/cavern→LOC_MISTY, east/passage (light inventory only)→LOC_PLOVER
- DARK

**LOC_PLOVER** — Plover Room
> You're in a small chamber lit by an eerie green light. An extremely narrow tunnel leads west. A dark corridor leads ne.
- Short: You're in Plover Room.
- Default items: EMERALD
- Exits: west/passage/out (light inventory)→LOC_ALCOVE, plover (carrying EMERALD)→LOC_Y2, ne/dark→LOC_DARKROOM
- LIT room (eerie green glow — no lamp needed).

**LOC_DARKROOM** — Dark Room
> You're in the dark-room. A corridor leading south is the only exit.
- Short: You're in dark-room.
- Default items: PYRAMID, TABLET (immovable — reads "MAGIC WORD XYZZY")
- Exits: south/plover/out→LOC_PLOVER
- Despite the name, lamp illuminates it normally.
- DARK
