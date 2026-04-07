# Chapter 1: Surface Area

**LOC_START** — Road End / Well House Exterior
> You are standing at the end of a road before a small brick building. Around you is a forest. A small stream flows out of the building and down a gully.
- Short: You're in front of building.
- Exits: west/road/hill→LOC_HILL, enter/building/east→LOC_BUILDING, south/down/gully/stream→LOC_VALLEY, north/forest→LOC_FOREST, depression→LOC_GRATE
- LIT room

**LOC_HILL** — Hill in Road
> You have walked up a hill, still in the forest. The road slopes back down the other side of the hill. There is a building in the distance.
- Short: You're at hill in road.
- Exits: building/east→LOC_START, west→LOC_ROADEND, north→LOC_FOREST, south/forest→LOC_FOREST

**LOC_BUILDING** — Inside Building (Well House)
> You are inside a building, a well house for a large spring. The stream flows out through pipes. It is light here.
- Short: You're inside building.
- Default items: KEYS, LAMP, FOOD, BOTTLE
- Exits: out/west→LOC_START, xyzzy→LOC_DEBRIS, plugh→LOC_Y2, down/stream→LOC_SEWER
- LIT room. **Deposit treasures here** to score points.

**LOC_VALLEY** — Valley
> You are in a valley in the forest beside a stream tumbling along a rocky bed.
- Short: You're in valley.
- Exits: upstream/building/north→LOC_START, east/forest→LOC_FOREST, west→LOC_FOREST, south/down→LOC_SLIT, depression→LOC_GRATE

**LOC_ROADEND** — End of Road
> The road, which approaches from the east, ends here amid the trees.
- Short: You're at end of road.
- Exits: road/east/up→LOC_HILL, building→LOC_START, south/forest→LOC_FOREST, west→LOC_FOREST, north→LOC_FOREST

**LOC_SLIT** — Slit in Streambed
> At your feet all the water of the stream splashes into a 2-inch slit in the rock. Downstream the stream bed is bare rock.
- Short: You're at slit in streambed.
- Exits: building→LOC_START, upstream/north→LOC_VALLEY, east/forest→LOC_FOREST, west→LOC_FOREST, south/depression→LOC_GRATE
- Note: Slit is too small to enter.

**LOC_GRATE** — Outside Grate
> You are in a 20-foot depression floored with bare dirt. Set into the dirt is a strong steel grate mounted in concrete. A dry streambed leads into the depression.
- Short: You're outside grate.
- Exits: east/forest→LOC_FOREST, south→LOC_FOREST, west→LOC_FOREST, building→LOC_START, upstream/north→LOC_SLIT, down/enter (if unlocked)→LOC_BELOWGRATE
- Grate locked by default. `unlock grate` with KEYS to open.

**LOC_FOREST** — Forest (all 22 forest locations)
> You are wandering aimlessly through the forest.
- LIT room (daylight).
- Exits vary — forest paths loop. Persist in one direction to find: LOC_START, LOC_HILL, LOC_ROADEND, LOC_VALLEY, LOC_GRATE, or LOC_SLIT.
- Note: Forest is intentionally hard to navigate. Try `building` or a compass direction repeatedly.

**LOC_SEWER** — Sewer Pipe Exit
> The stream flows out through a pair of 1-foot diameter sewer pipes. It would be advisable to use the main entrance.
- Exits: (any)→LOC_BUILDING
