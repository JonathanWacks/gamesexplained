# I, Ball — features

Read this before annotating code. What the game is documented to do, with
verification status against the binary. Statuses: **open** (documented,
not found yet), **traced** (in the code, could not be exercised; say what
was tried), **confirmed** (in the code, consistent with the emulator),
**live** (observed directly), **differs** (the code does something else).
"Absent" is not a status.

Sources:

- C64-Wiki, "I, Ball", https://www.c64-wiki.com/wiki/I,_Ball, read 26 October 2026
- Wikipedia, "I, Ball", https://en.wikipedia.org/wiki/I,_Ball, read 26 October 2026

The two disagree on who programmed it: C64-Wiki names Andrew Betts,
Wikipedia Timothy Closs. The game's own screens may settle it; until then
it is unknown.

The contributor's image is one file loading from `$0314` to `$FFFF`, which
is how crackers packed whole-memory versions, not how the tape loads.
C64-Wiki mentions a version "improved" by the group REMEMBER, with
trainer options and two extra keys; which version this is is open.

## Features

| Feature | Status | Where |
|---|---|---|
| Vertically scrolling shoot 'em up, one player | open | |
| 16 levels; a friend rescued after every fourth (Lover Ball, Eddy Ball, Glow Ball, No Ball) | open | |
| 50-second time limit per level; running out costs a life | open | |
| Four lives | open | |
| Plain and electrified obstacles on the track; the goal is the home straight at the top | open | |
| Bonus points for the time left at the end of a level | open | |
| Extra lives only from bonus disks | open | |
| Bonus disks always arrive in the same order; losing a life removes the latest extra; disks can be shot | open | |
| Extra: Turbo Boost (faster movement) | open | |
| Extra: Single Laser (fires sideways, the way Iball faces) | open | |
| Extra: Smart Missile (destroys every alien on screen, once; Space) | open | |
| Extra: Bullet Spray (fires up and down at once) | open | |
| Extra: Molecule Bomb (stops new aliens forming for a while, once; M) | open | |
| Extra: Electro Shield (immune to electric obstacles for a while) | open | |
| Extra: Hyperspace (jump straight to the goal) | open | |
| Extra: Twin Laser (fires left and right at once) | open | |
| Extra: Fuel Injection (faster vertical movement) | open | |
| Extra: Hyper Brakes (stronger braking for a while) | open | |
| Extra: Laser Cooling Unit (laser no longer overheats) | open | |
| Extra: Rainbow Ripple Laser (a wide, many-coloured laser) | open | |
| Faulty Disk: electrifies every obstacle until a life is lost or the level ends; offered only after Twin Laser | open | |
| Other disk rewards: bonus time, points, extra lives | open | |
| The laser overheats with continuous fire | open | |
| Aliens are harmless while they flicker in as they form | open | |
| Extras' status shown in the top and bottom screen areas | open | |
| Inertia: Iball drifts and bounces | open | |
| Joystick in port (to find) moves in all directions; fire shoots | open | |
| Keys in play: Z left, X right, O up, K down, P fire | open | |
| RUN/STOP pauses and resumes | open | |
| Title screen: 1 music, 2 sound effects | open | |
| Title screen: I, O, G play the samples "IBALL!", "OH NO!", "GAME OVER!" | open | |
| Title screen: joystick forward and back raise and lower the samples' pitch | open | |
| Rob Hubbard's music, after Cabaret Voltaire's "Whip Blow" and "I Want You" | open | |
| Three digitised speech samples (credited to Simon Pick) | open | |
| No high-score table | open | |
| REMEMBER version only: CLR/HOME abandons the game, Q returns to the last starting point, trainer options | open | |
| The game's own list of disc rewards, 17 names in screen codes: TURBO BOOST, SINGLE LAZER, SMART MISSILE, EXTRA SCORE, BULLET SPRAY, ELECTRO SHIELD, EXTENDED PLAY, TWIN LASER SET, HYPERSPACE, MOLECULE BOMB, FAULTY DISC, FUEL INJECTION, BONUS BALL, HYPER BRAKES, TIMER REWIND, LAZER COOLER, RAINBOW RIPPLE | open | `$6131`-`$62B3` |
| Messages: "COMPLETED LEVEL", "YOU HAVE RESCUED" a friend, "THAT WAS INCREDIBALL YOU HAVE COMPLETED IBALL", "GAME OVER" | open | `$596E`, `$5B5F`, `$6026` |

## Beyond the documentation

Found in the code, not in the manual.

## Open questions

- Which release is this image: the original, or a crack (REMEMBER's or another)?
- Who programmed it: Andrew Betts (C64-Wiki) or Timothy Closs (Wikipedia)?
