# Space Prime

## Play

**[Play Space Prime](https://archonlancelot.github.io/Space-Prime/)**

Click the link above and play in a desktop browser. No download, no install.

*Note for Hark: replace the placeholder above with the real, working play link as soon as the first playable build exists, and keep it working on every later build. If the hosting ever changes, update this link in the same change.*

## Current version: v0.1.0 (first playable)

Made by Hark. 2D, side-on view (like Spaceflight Simulator), one `index.html` file, runs in any desktop browser.

### Your world is always saved

- Everything saves by itself every second, and when you close the tab: every ship, where it is, how fast it's going, its fuel, dropped boosters, landers left on Luna, milestones, records, the world clock, and your zoom/map view.
- A ship left floating in orbit is still there, on the same orbit, when you come back. A lander parked on Luna stays parked.
- The world clock only moves while you play, so nothing happens to your ships while the game is closed.
- The save lives in this browser on this PC. To keep it extra safe (or move PCs), open the menu (`Esc`) and use **Download a backup of my save**, and **Load a backup file** to bring it back.
- Starting over is only possible from the title screen ("Start a brand new world"), and it asks twice.

### Controls

| Key | What it does |
|---|---|
| `W` / `S` (hold) | Throttle up / down (`Shift` also throttles up) |
| `Z` / `X` | Full throttle / cut engine |
| `A` / `D` or arrow keys | Turn left / right |
| `T` | SAS on/off (when on, the rocket stops spinning by itself) |
| `Space` | Drop the bottom stage |
| `M` | Map view (drag to move, `C` to recentre) |
| `,` / `.` | Slow down / speed up time (limited when low, in the air, or burning) |
| Mouse wheel | Zoom |
| `H` | Help |
| `Esc` | Menu: Tracking Station, new rocket, restart flight, sound, backups |

### Rockets

| Rocket | Feel | Stages | Δv | Safe landing |
|---|---|---|---|---|
| **Sparrow** | Nimble trainer. Turns fast, fuel is tight; a careful pilot just reaches orbit. | 1 | 4,315 m/s | 6 m/s |
| **Heron** | Moon lander. Booster gets you out of the air, the light upper stage goes to Luna and back. | 2 | 7,915 m/s | 8 m/s |
| **Mule** | Heavy hauler. Slow to turn, big tank, tough legs; can reach Luna one-way. | 1 | 5,769 m/s | 12 m/s |

### The worlds

- **Terra**, home planet: 600 km radius, air up to 70 km (air slows you down). Launch pad on top.
- **Luna**, the moon: 200 km radius, no air, orbits Terra at 12,000 km once every ~38.6 hours.

### What you see while flying

- Left panel: altitude, vertical speed, speed, apoapsis/periapsis (highest/lowest points of your orbit), throttle, fuel for the current stage, Δv left, thrust-to-weight, time warp, SAS.
- Bottom dial: yellow line = where the rocket points, green circle = direction you're moving (prograde), red X = backwards (retrograde), top = straight up.
- Map: your orbit in blue with Ap/Pe markers, Luna's path and sphere of influence, other ships, and a purple **Luna encounter** marker plus a box telling you when you'll arrive and how close you'll pass.
- Crash or land: crashes explode and offer a quick relaunch; landing on Luna (or making it home from Luna) gets a celebration screen.

### Milestones

First Launch · Reach Space · Orbit Terra · Reach Luna · Orbit Luna · Land on Luna · There and Back. See them, your records, and every ship in the **Tracking Station** (`Esc` menu), where you can switch to any ship, or recover/delete it.

### How to reach orbit

Full throttle straight up. Around 10 km start leaning toward the side; by about 40 km point almost sideways. Burn until Apoapsis is above 80 km, cut the engine, warp to the apoapsis, then burn sideways again until Periapsis is above 70 km.

### How to reach Luna

From orbit, open the map. When Luna is a bit more than a quarter turn ahead of you, burn prograde (green marker) until the purple Luna encounter box shows up. Near Luna, burn retrograde (red X) to slow down, then land upright and slowly.

### Changelog

- **v0.1.0**: First playable. Three rockets, Terra and Luna, real orbits (patched conics, exact on-rails orbits during time warp), air drag, staging, landing/crash rules, map with orbit and encounter prediction, time warp, Tracking Station, milestones, records, sound, and a fully persistent auto-saved world with backup download/upload.

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
