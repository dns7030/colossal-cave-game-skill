# Chapter 9: Deep Cave — Fork, Chasm, Volcano & Barren Room

**LOC_LOWROOM** — Large Low Room
> You are in a large low room. Crawls lead north, se, and sw.
- Short: You're in large low room.
- Exits: bedquilt→LOC_BEDQUILT, sw→LOC_WINDING, north→LOC_DEADCRAWL, se/oriental→LOC_ORIENTAL
- DARK

**LOC_DEADCRAWL** — Dead End Crawl
> Dead end crawl.
- Exits: south/crawl/out→LOC_LOWROOM
- DARK

**LOC_WINDING** — Long Winding Corridor
> You are in a long winding corridor sloping out of sight in both directions.
- Short: You're in sloping corridor.
- Exits: down→LOC_LOWROOM, up→LOC_SWCHASM
- DARK

**LOC_SWCHASM** — Southwest Side of Chasm
> You are on one side of a large, deep chasm. A heavy white mist rising up from below obscures all view of the far side. A sw passage leads away from the chasm.
- Short: You're on sw side of chasm.
- Notes: TROLL blocks crossing by default. JADE necklace appears here after troll is driven away.
- Exits: sw→LOC_WINDING, over/across/cross/jump (if troll_present=false)→LOC_NECHASM
- To cross: Option A: throw a treasure at troll (lose it, he lets you pass once). Option B: lead tamed BEAR here → troll flees, JADE drops.
- DARK

**LOC_NECHASM** — Northeast Side of Chasm
> You are on the far side of the chasm. A northeast passage leads away from the chasm.
- Short: You're on ne side of chasm.
- Exits: ne→LOC_CORRIDOR, over/across/cross (if troll_present=false)→LOC_SWCHASM, fork→LOC_FORK, view→LOC_BREATHTAKING
- DARK

**LOC_CORRIDOR** — Long Corridor
> You're in a long east/west corridor. A faint rumbling noise can be heard in the distance.
- Short: You're in corridor.
- Exits: west→LOC_NECHASM, east/fork→LOC_FORK, view→LOC_BREATHTAKING, barren→LOC_BARRENFRONT
- DARK

**LOC_FORK** — Fork in Path
> The path forks here. The left fork leads northeast and the right fork leads southeast. Both look equally promising.
- Short: You're at fork in path.
- Exits: west→LOC_CORRIDOR, ne/left→LOC_WARMWALLS, se/right/down→LOC_LIMESTONE, view→LOC_BREATHTAKING
- DARK

**LOC_WARMWALLS** — Junction with Warm Walls
> The walls are quite warm here. From the north can be heard a steady roar, so loud that the entire cave seems to be trembling. Another passage leads south, and a low crawl goes east.
- Short: You're at junction with warm walls.
- Exits: south/fork→LOC_FORK, north/view→LOC_BREATHTAKING, east/crawl→LOC_BOULDERS2
- DARK

**LOC_BREATHTAKING** — Breathtaking View
> You are on the edge of a breath-taking view. Far below you is an active volcano, from which great gouts of molten rock are belched. The glowing rock fills the farthest reaches of the cavern with a blood-red hue, giving everything an eerie, macabre appearance.
- Short: You're at breath-taking view.
- Exits: south/passage/out→LOC_WARMWALLS, fork→LOC_FORK, jump→(gruesome death)
- LIT room (volcano light)

**LOC_BOULDERS2** — Chamber of Boulders
> You are in a small chamber filled with large boulders. The walls are very warm, causing the air to be almost stifling from the heat. The only exit is a crawl going west, towards cooler air.
- Short: You're in Chamber of Boulders.
- Exits: west/out/crawl→LOC_WARMWALLS, fork→LOC_FORK, view→LOC_BREATHTAKING
- DARK

**LOC_LIMESTONE** — Limestone Passage
> You are walking along a gently sloping north/south passage lined with oddly shaped limestone formations.
- Short: You're in limestone passage.
- Exits: north/up/fork→LOC_FORK, south/down/barren→LOC_BARRENFRONT, view→LOC_BREATHTAKING
- DARK

**LOC_BARRENFRONT** — Front of Barren Room
> You are standing at the entrance to a large, barren room. A notice above the entrance reads: "Caution! Bear in room!"
- Short: You're in front of Barren Room.
- Exits: west/up→LOC_LIMESTONE, fork→LOC_FORK, east/in/barren/enter→LOC_BARRENROOM, view→LOC_BREATHTAKING
- DARK

**LOC_BARRENROOM** — Barren Room
> You are inside a barren room. The center of the room is completely empty except for some dust. Marks in the dust lead west towards the exit.
- Short: You're in Barren Room.
- Default items: BEAR (immovable until tamed), CHAIN (locked on bear until tamed)
- Exits: west/out→LOC_BARRENFRONT, fork→LOC_FORK, view→LOC_BREATHTAKING
- `feed bear` with FOOD → bear tamed, CHAIN becomes takeable (treasure), bear follows you.
- DARK
