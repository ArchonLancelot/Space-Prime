# Space Prime

## Play

**[Play Space Prime](PLAY_LINK_TO_BE_SET_BY_HARK)**

Click the link above and play in a desktop browser. No download, no install.

*Note for Hark: replace the placeholder above with the real, working play link as soon as the first playable build exists, and keep it working on every later build. If the hosting ever changes, update this link in the same change.*

## What this is

Space Prime is a rocket flight game inspired by Ellipse: Rocket Simulator and Spaceflight Simulator. It is an original game: do not copy art, assets, music, or code from those games, just the kind of play they offer — launch a rocket, fly it, get into orbit, and land on other worlds.

## Who plays, and on what

- One player only: Armando. Single-player only. No multiplayer, no accounts, no login needed to play.
- PC only, in a desktop browser. Keyboard and mouse controls.
- No phone / touch version needed.

## A decision that is Hark's, not Hsin's

**2D vs 3D is Hark's call.**

Pick whichever you can get playable, smooth, and fun fastest in a desktop browser, under these constraints:

- It must open from the README play link with no download or install.
- It must run well on a normal PC browser.
- Controls must be clear on keyboard and mouse, and documented in this README.

Do not let the 2D/3D choice block the first playable version — ship the core flight loop first, then expand.

## Version 1 scope — prebuilt rockets

Start with **prebuilt, unique rockets, not a part-by-part rocket builder.**

Each rocket in the roster should feel different, for example in thrust, fuel, mass, handling, or what missions it suits. Give each one a name and a short description in-game so the player can tell them apart at a glance.

First playable version should include, at minimum:

1. A rocket select screen with at least one or two distinct rockets.
2. Launch from a home planet.
3. Throttle and steering, gravity, and fuel that actually runs out.
4. Speed, altitude, and fuel shown clearly while flying.
5. A way to reach orbit, and a Moon (or one other body) to aim for and land on.
6. Clear success / crash outcomes, and an easy restart.

Later versions can add more rockets, more planets/moons, and missions — but v1 is the flight loop above, working end to end.

## Core feel to aim for

- Flying should feel like rocket flight, not arcade shooting: gravity pulls, orbits are possible, going too fast or landing too hard has consequences.
- The player should always know what the rocket is doing: speed, altitude, fuel, and whether they are on course.
- Controls should be simple to learn and listed in this README (throttle, steer, stage if staging exists, restart).

## How Hark should work in this repo

- Hsin writes docs and briefs only. Hsin does not code this game.
- Hark codes the game.
- Every change that affects how Armando plays must keep the README play link at the top of this file working.
- When you add a feature, update this README in the same change: what was added, how to control it, and what the player should see.
- If a choice would force Armando to download, install, or log in to play, do not make it without asking him first.

## Open for Hark to decide

- 2D or 3D (see above).
- Engine / framework, as long as it delivers a browser play link.
- Hosting for the play link, as long as it opens for Armando with no install.
- The exact first set of rockets, planets, and missions, within the v1 scope above.
