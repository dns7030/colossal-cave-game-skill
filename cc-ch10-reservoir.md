# Chapter 10: Reservoir, Mirror Canyon & Upper Reaches

**LOC_THREEJUNCTION** — Junction of Three Secret Canyons
> You are in a secret canyon at a junction of three canyons, one from the north, one from the ne, and one below. Above you is a large dome with gleaming formations.
- Short: You're at junction of three secret canyons.
- Exits: se→LOC_BEDQUILT, south→LOC_SECRET2, north→LOC_WINDOW2
- DARK

**LOC_WINDOW2** — Window on Pit (south side)
> You're at a low window overlooking a huge pit, which extends up out of sight. Across the pit, the window on the other side can barely be seen.
- Short: You're at window on pit.
- Exits: west→LOC_THREEJUNCTION, jump→(death)
- DARK

**LOC_TOPSTALACTITE** — Top of Stalactite
> A large stalactite extends from the roof and almost reaches the floor below. You could climb down it, and jump from it to the floor (risky).
- Short: You're at top of stalactite.
- Exits: north→LOC_SECRET2, down/jump/climb→LOC_ALIKE6 (may land in various maze rooms)
- DARK

**LOC_MIRRORCANYON** — Mirror Canyon
> You are in a north/south canyon about 25 feet across. The floor is covered by white mist seeping in from the north. The walls extend upward for well over 100 feet. Suspended from some unseen point far above, an enormous lighted crystal glows, lighting everything with a sparkling blue radiance. There is a mirror on the west wall, 15 feet up.
- Short: You're in Mirror Canyon.
- Exits: south→LOC_SECRET1, north/reservoir→LOC_RESERVOIR
- LIT room (crystal light)

**LOC_RESERVOIR** — Reservoir
> You are at the edge of a large underground reservoir. An opaque cloud of white mist fills the room and rises rapidly. The drop to the water and the mist are damp and cold. The only exit is to the south, back toward the mirror canyon.
- Short: You're at reservoir.
- Exits: south/out→LOC_MIRRORCANYON, north/across/cross→LOC_RESBOTTOM
- Fill BOTTLE here with water.
- LIT room (glowing mist)

**LOC_RESBOTTOM** — Bottom of Reservoir
> You are walking across the bottom of the reservoir. Walls of water rear up on either side. The roar is overwhelming.
- Short: You're at bottom of reservoir.
- Exits: north→LOC_RESNORTH, south→LOC_RESERVOIR
- DARK

**LOC_RESNORTH** — North of Reservoir
> You are at the northern edge of the reservoir. A northwest passage leads sharply up from here.
- Exits: south/across/cross→LOC_RESBOTTOM, northwest/up/out→LOC_TREACHEROUS
- DARK

**LOC_TREACHEROUS** — Treacherous Passage
> You are scrambling along a treacherously steep, rocky passage.
- Exits: up/northwest→LOC_STEEP, down/southeast→LOC_RESNORTH
- DARK

**LOC_STEEP** — Steep Incline
> You are on a very steep incline, which widens as it goes upward.
- Exits: down/southeast→LOC_TREACHEROUS, up/northwest→LOC_CLIFFBASE
- DARK

**LOC_CLIFFBASE** — Base of Cliff
> You are at the base of a nearly vertical cliff. Slim footholds enable climbing up.
- Exits: up/climb→LOC_CLIFFTOP, down→LOC_STEEP
- DARK

**LOC_CLIFFTOP** — Top of Cliff
> You have climbed to the top of the cliff. The cave continues here.
- Exits: down→LOC_CLIFFBASE
- DARK

**LOC_BROKEN** — Broken Neck (death)
> You are at the bottom of the pit with a broken neck.
- Death room. You have died.
