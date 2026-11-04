# Foxtrail

A cosy hidden-path puzzle. Hop Pip the rabbit home to his burrow, read the clue numbers to dodge hidden snares, and stay one step ahead of the wolf.

**Play:** open `index.html` in any browser. No install, no build step.

## Features

- 100 levels across 10 worlds, from Meadow to Moonrise. A solver checked that every level can be won.
- Wolf events: moves every hop or every second hop, two-tile lunges, sleepers you must not wake, two wolves at once.
- Special tiles: hedges, bushes, streams and stepping stones, carrots, wormholes, mud with move limits, fog, one-way fences.
- Animated Pip and wolf, drawn in SVG, with expressions for every moment: hunting, snarling, howling, getting snared, catching Pip, sulking when he gets home.
- Sound effects synthesized in the browser with the Web Audio API. Mute from the speaker button in the game or the switch in Profile.
- Stars, stats, a daily meadow and a family to rescue. Progress is saved in the browser (localStorage).

## How to play

1. Tap a tile with a ring to hop Pip one tile up, down, left or right.
2. Each tile Pip lands on shows how many snares hide in the 8 tiles around it. His ears twitch once per nearby snare.
3. Stepping on a snare costs a life.
4. The Next hops strip shows which wolf moves after each of your hops. A faint paw marks where a wolf will step next.
5. Wolves can't see snares. Lead one over a hidden snare and it's stuck for 2 turns.

## Project

The whole game is one self-contained file, `index.html`: HTML, CSS, JavaScript, the SVG characters and the sound code. The only external request is the Onest font from Google Fonts. Without it, the game falls back to the system font.

The Profile sheet has a "Testing: unlock all 100 levels" switch for development. Remove it before a public release.
