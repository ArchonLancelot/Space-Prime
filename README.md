# Space Prime

## Play

**[Play Space Prime](https://archonlancelot.github.io/Space-Prime/)**

Click the link above and play in a browser on your PC or your phone. No download, no install.

*Note for Hark: replace the placeholder above with the real, working play link as soon as the first playable build exists, and keep it working on every later build. If the hosting ever changes, update this link in the same change.*

## Current version: v0.6.0 (smaller phone UI, 3 launch pads)

Made by Hark. 2D, side-on view (like Spaceflight Simulator), one `index.html` file, runs in any desktop or phone browser.

### PC or Mobile?

Every time you open the game it asks **PC** or **Mobile** first. It asks every time on purpose (it doesn't remember), so the same link works on both.

- **PC**: keyboard and mouse.
- **Mobile**: touch buttons round the edges of the screen, sized for thumbs (since v0.6.0 smaller and tidier, so you can actually see your rocket).
- Picked the wrong one? Change it any time from the menu (**Controls: ...**) or the title screen. Your flight is not affected.

### Your rocket: the Kestrel

There is now one rocket, and it can do everything:

| Part | What it does |
|---|---|
| **Booster** (bottom) | The big, heavy first stage. Lifts you out of the thick air. 377 kN of push on the ground, 420 kN once the air is thin. |
| **Upper stage** (middle) | Light and efficient (50 kN in space). Has landing legs. Finishes getting you to orbit, flies you to Luna and lands there, or slows you down to come home. |
| **Crew capsule** (top) | No engine. Has a **heat shield** on its bottom and a **parachute** on top. This is what comes home to Terra. |
| **Fairing** (nose cone) | A pointed cover over the capsule for the climb through the air. 300 kg of extra weight once you're up high, so drop it. |

Numbers: 27.1 t on the pad, thrust/weight 1.42 at launch, about 6,575 m/s of Δv in total. Air push limit (max-Q) 40 kPa. Safe touchdown: 8 m/s on the legs, 9 m/s for the capsule on land, 14 m/s in the ocean. Parachute: open below 250 m/s.

What a good pilot can do with it:
1. **Reach orbit** around Terra with about 3,000 m/s of Δv to spare.
2. **Fly to Luna and land** on the upper stage's legs (with the capsule on top). Coming back from Luna's surface is not possible with this rocket.
3. **Come home from orbit**: drop back into the air, survive the heat, open the parachute and land (or splash down). That earns **Round Trip**.

Sparrow, Heron and Mule are **retired**: you can't launch them any more. Any that were already flying in your saved world are still there: they show up in the Tracking Station and you can still fly them.

### Sound, music and settings (new in v0.5.0)

Every sound is made by the game itself while you play (no sound files), so it's still just one `index.html`.

- **Engines roar, and each one sounds different.** The Kestrel booster is a deep, crackling roar; the Kestrel upper stage is a higher, smoother hiss with a faint whine. The retired ships have their own voices too: Sparrow buzzes and rattles, Heron's booster pulses, Heron's lander whines higher, and the Mule is a slow, thundering rumble.
- **The roar follows the throttle and the air.** More throttle = louder. As you climb, the air thins and the roar gets quieter and muffled. In space you only hear the low rumble coming through the ship itself (quiet, but not silent).
- **Sounds for the big moments:** countdown beeps (higher for the last three), ignition, the clamps letting go at liftoff, staging bangs, the fairing popping off, the parachute opening, touchdown, splashdown, explosions, the max-Q alarm, milestones and a little fanfare for Mission Complete.
- **Soft space music** plays quietly in the background while you fly.
- **Camera shake:** a light wobble at liftoff, near max-Q, at staging and in a crash.
- **Settings:** Menu (`Esc` / **☰ Menu**) → **Settings: sound, music & shake**. Sliders for **Master**, **Effects** and **Music** volume, **Sound on/off**, and **Camera shake on/off**. They're saved on this device (your world backup file doesn't change them).
- Sound starts after your first click, tap or key press (phones and browsers require that). It goes quiet while the game is paused (menus) and when you switch to another tab or app.

### What you'll see (new in v0.5.0)

- **Terra:** clouds you fly up through (they drift slowly), sandy beaches and pale shallow water along the coasts, and **day and night**. The sun goes round once per Terra day (24 hours on the game clock); a new world starts at midday over the launch pad. At sunrise and sunset the sky glows orange and pink, and from orbit you can see the glow along Terra's edge. The map shows Terra's and Luna's night sides.
- **Luna:** rolling hills and craters (up to about 12 km across, with flat floors and gentle walls). The ground you see is exactly the ground you land on, so the rocket never floats above it or sinks into it. On a slope the downhill landing leg reaches down to the ground. Any lander you parked on Luna in an older version is stood on the new ground when your save loads. **Altitude** near Luna now means height above the ground right under you.
- **Dust and smoke:** the engine kicks up a spray of dust when you land on Luna, and blasts smoke sideways across the pad and the ground on Terra.
- **Bigger explosions:** a flash, fire, dark smoke and pieces of the rocket tumbling away. The camera stays on the wreck.

### Stars, results and personal bests (new in v0.5.0)

When you finish a mission, the gold **MISSION COMPLETE** banner shows first, then a **results screen** with:
- **Time** from liftoff to done (game clock, so time warp counts),
- **Fuel left** in the upper stage and **fuel used** (all stages),
- **Touchdown speed** (Luna landing),
- **1 to 3 stars**, and your **personal bests**.

**Star rules:** ★ for finishing the mission, **+★ Fuel saver**, **+★ Neat finish**:

| Mission | Fuel saver (fuel left in the upper stage) | Neat finish |
|---|---|---|
| Low orbit (LEO) | at least 60% | highest and lowest point no more than 15 km apart |
| Medium orbit (MEO) | at least 33% | no more than 300 km apart |
| High orbit (GEO) | at least 28% | no more than 1,221 km apart |
| Luna orbit | at least 30% | lowest and highest point both between 50 and 200 km |
| Luna landing | at least 10% | touch down at 3 m/s or slower |

Following the pink guidance carefully earns all three stars on every mission (that's how the limits were set: the test pilot that follows only the arrows gets 3 stars, with a little to spare).

**Personal bests** are kept for each mission: best stars, **fastest** time, **least fuel used**, and **softest touchdown** (Luna landing). Beat one and the results screen says **new best!**. They're saved in your progress and shown in the **Tracking Station** under each mission.

### Launch pads (new in v0.6.0)

Terra now has **three launch pads** on its big continent. On the pad, the **Pick a mission** panel has a **Launch pad** row under the missions. They are listed in the order they sit on Terra, left to right on screen:

| Pad | Where | What it's like |
|---|---|---|
| **Cape Halcyon** | about **390 km to the left** of Prime Field | A coastal pad, about 1.5 km from the beach. Tall white tower, lightning masts and a water tower. Fly left (the usual way) and you go out over the sea, like real coastal spaceports. |
| **Prime Field** | in the middle (the original pad) | The pad you've always launched from. Still the default. |
| **Redrock Range** | about **210 km to the right** of Prime Field | An inland desert pad (about 85 km from the coast), on sandy ground with red rock mesas and a flame trench. |

Why those distances: Terra is about a tenth of Earth's size, so 210 km and 390 km here are like roughly 2,000 and 4,000 km on Earth, about how far apart real spaceports are.

- **Pick a pad**: click it (PC) or tap it (Mobile) while the clock holds at **T-10 HOLD**. Your rocket moves to that pad straight away, ready to go.
- Once the countdown is running the pad is fixed (the buttons go grey).
- The pad you pick is **remembered**: every new rocket launches from it until you pick another. **Restart this flight from the pad** uses the same pad.
- Everything else works the same from every pad: countdown, clamps, missions, the pink guidance and the stars. Orbits and Luna trips don't care which pad you used.
- The **map** shows all three pads as little markers on Terra (the one you're using in yellow), with their names when you zoom in.
- The pads are set up so more can be added later.

### Missions and guidance (new in v0.4.0, optional)

When your Kestrel is on the pad, a **Pick a mission** panel appears (on the right on PC, top-left on a phone). You don't have to use it: ignore it, or pick **Free flight**, and fly anywhere like before.

| Mission | Goal | Counts as done when |
|---|---|---|
| **Low orbit (LEO)** | Circle Terra about **100 km** up | Lowest and highest point both between 80 and 120 km, engine off |
| **Medium orbit (MEO)** | Circle Terra **2,000 km** up | Both points between 1,800 and 2,200 km |
| **High orbit (GEO)** | Circle Terra **8,140 km** up. Up there one lap takes exactly one Terra day (24 hours on the game clock), like a real GEO | Both points between 7,733 and 8,547 km (within 5%) |
| **Luna orbit** | Fly to Luna and get caught by it | An orbit around Luna with its lowest point above 10 km and highest below 500 km |
| **Luna landing** | Fly to Luna and land | Touch down on the legs, upright, slower than 8 m/s |

Why those heights: Terra is much smaller than Earth, so the real heights were scaled down. They all sit well inside the 84,000 km edge of Terra's pull and below Luna's path (12,000 km out), so Luna never gets in the way.

- **Pick one**: click it (PC, or press `1`–`5`, `0` = free flight) or tap it (Mobile). The chosen one gets a yellow outline and a short description.
- **Change your mind** any time until liftoff, even during the countdown. **Hide** folds the panel into a small bar; **Show** opens it again.
- Then start as usual: `Enter` / **START**.
- **In flight** a pink panel tells you the next step in a few words, for example *"Tilt left to 45°"*, *"Cut engine now"*, *"Wait — warp to Ap"*, *"Burn prograde at Ap"*, *"Burn prograde to Luna"*, *"Fine-tune: burn at the arrow"*, *"Landing burn: nose up, follow the throttle"*. Under it are little tags: the **throttle** to use (FULL, CUT or a %), what to press (*"Press Space: drop the booster"*), and **Warp OK** when it's safe to speed up time.
- **Pink arrows show where to point**: one next to your rocket (with a curved arrow saying *turn left* / *turn right*) and a pink marker on the dial.
- **Left or right, both work (v0.5.0).** The guidance leans you left (the way Luna goes round, which is a bit cheaper). If you lean clearly to the right before 1.5 km, it follows you and flies the whole mission round Terra the other way, including the trip to Luna ("Wait until Luna is 102° behind").
- **Time warp slows down by itself** before the next burn, so you can't warp past it.
- Do what it says and you get there. When you make it, a gold **MISSION COMPLETE** banner appears. It's saved straight away, and the **Tracking Station** shows a ★ next to each mission you've done (and how many times).
- Changed your mind in flight? Menu → **Stop the mission (fly free)**.
- **Restart this flight from the pad** keeps the same mission.

### The Angle reading (new in v0.4.0)

The flight panel now shows **Angle**: how far your nose is above the horizon. **90° up** = straight up, **0°** = flat along the horizon, negative = nose below the horizon (**-90° down** = straight down). It also says **left** or **right** (which way you're leaning). It's measured against the ground right under you: Terra's horizon near Terra (and anywhere out to deep space), Luna's horizon near Luna. The guidance uses the same numbers ("Tilt left to 45°").

### PC controls

| Key | What it does |
|---|---|
| `Enter` | On the pad: **start the countdown**. Press it again during the countdown to launch straight away |
| `1`–`5`, `0` | On the pad: **pick a mission** (1 LEO, 2 MEO, 3 GEO, 4 Luna orbit, 5 Luna landing, 0 free flight) |
| `W` / `S` (hold) | Throttle up / down (`Shift` also throttles up) |
| `Z` / `X` | Full throttle / cut engine |
| `A` / `D` or arrow keys | Turn left / right |
| `Space` | Drop the bottom stage (first the booster, later the upper stage) |
| `F` | **New:** drop the fairing |
| `P` | **New:** open the parachute |
| `T` | SAS on/off (when on, the rocket stops spinning by itself) |
| `M` | Map view (drag to move, `C` to recentre; if your ship is far away, `C` also zooms out to show it) |
| `,` / `.` | Slow down / speed up time (limited when low, in the air, burning, or counting down; you can warp while the rocket waits on the pad) |
| Mouse wheel | Zoom |
| `H` | Help |
| `Esc` | Menu: Tracking Station, new rocket, restart flight, **Settings** (sound, music, shake), backups |

### Mobile controls

Hold your phone sideways (landscape). If you hold it upright, the game pauses and asks you to turn it; you can also tap **Play in portrait anyway**.

**v0.6.0: a smaller, tidier phone screen.** Everything is smaller and pushed to the edges so the middle of the screen (your rocket) stays clear:
- The flight numbers are a small panel in the top-left corner (held sideways) or bottom-left (held upright). It starts **short** (altitude, speed, angle, Ap, Pe, fuel). **Tap it** for the full list (vertical speed, Δv, air push and heat too), tap again to shorten it. The game remembers your choice on this phone (also in Menu → Settings → **Flight info**).
- The clock, the pink guidance strip and messages sit in a narrow strip at the top. Messages that would cover the rocket go beside it instead.
- On the pad, the mission and pad picker is a compact panel in the corner.
- Buttons are 44 px (40 px on the smallest phones), still easy to hit with a thumb.
- Checked on iPhone SE, iPhone 14, iPhone 15, iPhone 15 Pro Max, Pixel 7, Galaxy S24, Galaxy S9+ and Moto G4, held sideways and upright: nothing overlaps, nothing is cut off, nothing sits on the rocket. The game's controls take up about a third to almost half less of the screen than in v0.5.0.
- The PC screen is exactly the same as before (apart from the new launch pad row in the mission panel).

| Button | Where | What it does |
|---|---|---|
| **Action button** (green) | bottom left, next to the turn buttons (above them in portrait) | **New.** Changes with the moment: **START** on the pad (starts the countdown), then **SKIP** during the countdown (launch now), then **FAIRING** in flight (drop the nose cover), then **CHUTE** when the capsule is coming home (open the parachute). It turns **orange** when it isn't safe yet ("air thick", "too fast", "no air"). |
| **Mission & pad picker** | top left, on the pad | Tap a mission (or Free flight) and a launch pad. **Hide** / **Show** folds it into a small chip. In flight the guidance shows in a strip at the top |
| **Throttle slider** | right side | Drag up for more power, down for less |
| **FULL** / **CUT** | above / below the slider | Full power / engine off |
| **⟲** / **⟳** (hold) | bottom left | Turn left / right. You can hold one with your left thumb while dragging the throttle with your right |
| **STAGE** | bottom, next to the zoom buttons (upright: bottom left, next to the action button) | Drop the bottom stage (booster first, then the upper stage) |
| **SAS** | right edge | On/off (green = on) |
| **Map** | right edge | Map view. Drag with one finger to move around, **Centre** to snap back (and zoom out to a far-away ship) |
| **Warp +** / **Warp −** | right edge | Speed up / slow down time |
| **Pinch**, or **+** / **−** (hold) | anywhere / above STAGE (upright: right edge) | Zoom in / out |
| **☰ Menu** | top right | Pause: Tracking Station, new rocket, restart, **Settings** (sound, music, shake), backups, switch to PC controls |

In flight the buttons are 44 px (40 px on the smallest phones) and never overlap; menus keep their bigger 48 px buttons. Held upright, the **+ / − zoom** buttons sit in the right-hand column, and the action button and **STAGE** sit just above the turn buttons.

### What's new in the flying (in plain words)

- **Countdown.** A new rocket waits on the pad with the clock holding at **T-10 HOLD**. Nothing happens until you press `Enter` (PC) or tap **START** (Mobile). Then the 10-second countdown runs with beeps. At T-3 the engines light (the sound builds up) while clamps on the tower hold the rocket down. At zero the clamps swing away and you lift off. During the countdown, `Enter` again / **SKIP** launches straight away.
- **The sky changes.** Blue near the ground, darker as you climb, black with stars in space.
- **The flame changes.** Down low it's a tight, bright flame (thick air squeezes it). Up high it spreads out wide and soft.
- **Engines get stronger as you climb.** Thick air pushes back on the engine's exhaust, so engines are a bit weaker on the ground and at full strength in space.
- **Max-Q (air push).** Going fast in thick air pushes hard on the rocket. The left panel shows it as **Air push** in kPa. Above 70% of the limit a red **MAX-Q** warning flashes: throttle down a little or turn over more gently. Above 40 kPa the rocket breaks apart. A normal climb stays around 18 kPa.
- **Heavy rockets turn slowly.** The engines swivel a little to steer, so a full, heavy rocket turns slowly and a light upper stage turns faster. With the engines off only a small spinning wheel inside can turn you, which is very slow on a big rocket.
- **Live Ap / Pe.** Your apoapsis (highest point) and periapsis (lowest point) are shown all the time, also right above the dial. A green **prograde** marker floats next to your rocket, showing which way you're actually moving.
- **Staging.** Dropping a stage gives a small push that sends the two parts apart, with a puff of smoke.
- **Fairing.** Keeping it on means extra weight and a wider nose (more drag). Drop it once you're above about 45 km. Try it in thick air and the game warns you first; do it anyway in really thick air and the halves knock the rocket into a spin.
- **Coming home.** Hitting the air at orbital speed heats the ship and it glows. The **Heat** reading shows how close you are to the limit. Only the capsule has a heat shield, so drop the upper stage first, and keep the shield (the capsule's bottom) facing the way you're moving. The capsule tends to swing that way by itself in the air. Come in too steep or too fast and it burns up. A periapsis of about 25–35 km is a gentle way down.
- **Parachute.** Only works in the air and below 250 m/s. Open it faster than that and it tears off (one chute, no spare). Under the parachute the capsule comes down at about 6.5 m/s.
- **Land or ocean.** Terra now has continents and oceans. Landing on land and splashing down in the ocean both count.

### How to reach orbit

Easiest way: pick the **Low orbit** mission on the pad and follow the pink arrows. By hand: press `Enter` / tap **START** to start the countdown (press `Enter` again / tap **SKIP** to go straight away). Full throttle straight up. Around 2 km start leaning **left**, gently: a full rocket turns slowly. Left is the way Luna goes round Terra, which makes a Luna trip cheaper later. Aim for about 40° over at 10 km and 70° at 30 km. Keep an eye on the **Air push** reading. When the booster runs dry, drop it. Above about 45 km drop the fairing. Keep burning, nearly sideways, until **Periapsis** is above 70 km (cut the engine for a while if Apoapsis climbs well past 80 km while you're still low).

### How to reach Luna

From orbit, open the map. When Luna is a bit more than a quarter turn ahead of you, burn prograde (green marker) until the purple Luna encounter box shows up. Near Luna, burn retrograde (red X) to slow down, then land upright on the legs, slower than 8 m/s. No air there, so no parachute.

### How to come home (Round Trip)

From orbit, point retrograde (red X) and burn until Periapsis is about 25–35 km. Drop the upper stage. Keep the heat shield forward while the capsule glows. When you're below 250 m/s, open the parachute. Touch down, or splash down, and you've earned **Round Trip**.

### The edge of Terra's pull (deep space)

- Terra's pull reaches **84,000 km** out. On the map this is the dashed yellow circle, labelled **Edge of Terra's pull**.
- If you go faster than escape speed, **Apoapsis** says **Escaping** and the map marks the spot where you'll leave ("Leaves Terra's pull").
- Past the edge you're in **deep space**: nothing pulls on you, so the ship coasts in a straight line. Altitude keeps counting up in km, then in million km. Apoapsis and Periapsis both say **Escaping** while you drift away.
- You can still fly: turn round and burn towards Terra. The status changes to "Deep space, coming back", and once you're back inside the circle Terra's pull takes over again.
- In the map, if your ship is off the screen, an arrow at the edge points to it with its distance. `C` / **Centre** zooms out to show it.
- Time warp works normally out there, and saving/reloading keeps the ship exactly where it was.

### Your world is always saved

- Everything saves by itself every second, and when you close the tab: every ship, where it is, how fast it's going, its fuel, dropped boosters, landers left on Luna, milestones, records, the world clock, and your zoom/map view.
- A ship left floating in orbit is still there, on the same orbit, when you come back. A lander parked on Luna stays parked.
- The world clock only moves while you play.
- The save lives in the browser on the device you play on. To keep it extra safe, or to move it to another device, use **Download a backup of my save** in the menu, and **Load a backup file** to bring it back.
- **New in v0.6.0:** the launch pad you picked is saved (and each ship remembers which pad it launched from). The "short flight info" choice is saved with your settings on this device.
- **New in v0.4.0:** your chosen mission and where you are in it are saved with the ship, so after a reload the guidance carries on from the same step. Finished missions are saved in your records.
- Saves from v0.1.0 to v0.5.0 still load in v0.6.0: they simply use Prime Field (the original pad), and you can pick another pad any time. Saves from v0.1.0 to v0.4.0 still load in v0.5.0 (the results and bests are new, optional parts of your progress). Saves from v0.1.0, v0.2.0, v0.3.0 and v0.3.1 still load in v0.4.0 (and a v0.4.0 save still opens in v0.3.1, which just ignores the mission parts): the old Sparrows, Herons and Mules keep flying; milestones and records stay. Each version only adds new information to the save, it doesn't change the old parts. If an older version had thrown a ship impossibly far away (see v0.3.1 below), loading puts it back at the edge of Terra's pull so you can fly it again.
- Starting over is only possible from the title screen ("Start a brand new world"), and it asks twice.

### The worlds

- **Terra**, home planet: 600 km radius, air up to 70 km, continents and oceans. Three launch pads on the big continent: Cape Halcyon (coast, left), Prime Field (middle, on top at the start) and Redrock Range (desert, right). Its pull reaches 84,000 km out; past that is deep space.
- **Luna**, the moon: 200 km radius, no air, orbits Terra at 12,000 km once every ~38.6 hours.

### Milestones

First Launch · Reach Space · Orbit Terra · **Round Trip** (new) · Reach Luna · Orbit Luna · Land on Luna · There and Back. See them, your records (now also splashdowns and your softest touchdown), and every ship in the **Tracking Station**.

### Changelog

- **v0.6.0** (smaller phone UI, 3 launch pads):
  - **Phone screen made much smaller and tidier** (Armando: "UI (only in mobile) is like way too big"). Smaller text and buttons (44 px, 40 px on the smallest phones), everything grouped at the edges, the rocket in the middle always visible. The flight panel starts short and opens to the full list with a tap (remembered on your phone). The mission picker is compact, messages move aside instead of covering the rocket, and the dial and its Ap/Pe line fit between the buttons. Works held sideways and upright on small and big phones. PC looks exactly as before.
  - **Two new launch pads**: **Cape Halcyon** (a coastal pad about 390 km to the left, rockets fly out over the sea) and **Redrock Range** (a desert pad about 210 km to the right). Pick one on the pad in the mission panel; the rocket moves there at once. Each has its own tower, clamps, ground and buildings. Countdown, clamps, missions and the pink guidance work the same from all three, and the map shows all three pads.
  - Saves: same format (v: 1). Old saves load and use Prime Field. Your pad choice is saved, and so is each ship's pad.

- **v0.5.0** (sound, looks and rewards):
  - **Sound:** a real engine roar that follows the throttle and fades and muffles as the air thins (in space just the rumble through the ship). Every engine sounds different: Kestrel booster, Kestrel upper stage, and the retired Sparrow, Heron (booster and lander) and Mule. Sounds for the countdown, ignition, liftoff clamps, staging, fairing, parachute, touchdown, splashdown, explosions, the max-Q alarm, milestones and Mission Complete. Soft space music. All made in code, so it's still one file.
  - **Settings** in the menu: master / effects / music volume, sound on/off, camera shake on/off. Saved on this device. Sound starts after your first tap/click/key and pauses with the game and when the tab is hidden.
  - **Camera shake** (light) at liftoff, max-Q, staging and crashes.
  - **Looks:** Luna has hills and craters (and you land on exactly what you see); Terra has clouds, beaches and shallow water at the coasts, and day and night with orange sunrise/sunset glows (also seen along Terra's edge from orbit and on the map). Dust sprays on Luna landings, smoke billows across the ground on Terra, and explosions now have a flash, smoke and tumbling debris.
  - **Rewards:** a results screen after Mission Complete (time, fuel left, fuel used, touchdown speed) with 1–3 stars (rules above), and personal bests per mission (fastest, least fuel, softest touchdown, best stars), saved and shown in the Tracking Station.
  - **Fixes:** iPhone SE held upright: the bottom buttons no longer overlap (zoom buttons moved to the right-hand column, the dial sits above the buttons, and only the two newest messages show). Luna guidance now works whichever way round Terra you fly (before, it asked you to orbit the other way if you went right).
  - Saves: still the same format (v: 1). Old saves load; stars and bests are only added. Settings are stored separately, per device.

- **v0.4.0** (missions and guidance):
  - **Pick a mission on the pad (optional):** Low orbit (100 km), Medium orbit (2,000 km), High orbit (8,140 km, one lap per Terra day), Luna orbit, Luna landing, or Free flight. Click / press 1–5 on PC, tap on Mobile. You can change it or go back to free flight until liftoff. The countdown still waits for you (Enter / START).
  - **Step-by-step guidance in flight:** a short instruction ("Tilt left to 45°", "Cut engine now", "Wait — warp to Ap", "Burn prograde at Ap", "Burn prograde to Luna", "Landing burn"...), a throttle tag, pink arrows next to the rocket and on the dial, and time warp that slows down by itself before each burn. Following it really does get the Kestrel there: it was tested by a robot pilot that only looks at the arrows and tags, on PC and on touch, for all five missions, and also with a deliberately slow, late-reacting pilot.
  - **Mission Complete:** a gold banner when you make it, saved to your progress, with ★ stars in the Tracking Station.
  - **Angle reading** in the flight panel (90° = straight up, 0° = flat), on PC and phones.
  - Menu: **Stop the mission (fly free)**. Restarting a flight keeps its mission. Help screen and the launch screen explain missions.
  - Saves: still the same format; old saves load, and the new parts are only added.

- **v0.3.1** (bug fixes):
  - **Flying far away no longer breaks the game.** Before, if you flew fast enough to escape Terra, the ship could suddenly jump off the map and Altitude / Periapsis showed a giant frozen number (like 22,152,993,979,...). The cause: the maths that moves ships along their path during time warp made a bad first guess on escape paths and never checked its answer, so it could throw the ship to an impossible distance. Now every answer is checked and redone in smaller steps if it's wrong, so the numbers are always real and keep updating.
  - **Terra's pull now has an edge** at 84,000 km, drawn on the map. Past it is **deep space**, where the ship coasts in a straight line and can burn back home (see "The edge of Terra's pull" above). Apoapsis/Periapsis show **Escaping**, distances show in km and million km, and the map can zoom out far enough to follow you, with an arrow pointing to your ship when it's off screen.
  - A ship that an older version had already thrown impossibly far is put back at the edge of Terra's pull when your save loads (you'll see a message). The "highest above Terra" record is fixed too.
  - **The countdown no longer starts by itself.** After picking the Kestrel, the clock holds at **T-10 HOLD**. Press `Enter` (PC) or tap **START** (Mobile) to start it. During the countdown, `Enter` / **SKIP** still launches straight away. You can time-warp while waiting on the pad (handy for waiting for Luna). Help screens, hints and this README now all say the same thing.
- **v0.3.0**: One rocket, the **Kestrel**: booster, upper stage with legs, crew capsule with heat shield and parachute, and a nose fairing. Sparrow/Heron/Mule retired (old ones still load and fly). Launch countdown with clamps and engine sound that builds up (skippable). Sky fades from blue to black; the flame is tight low down and wide in space. Engines are weaker in thick air. Max-Q readout, warning and breakup. Heavy rockets turn slowly (engine steering plus a small reaction wheel). Live Ap/Pe above the dial and a prograde marker next to the rocket. Stages push apart with a smoke puff. Fairing drop (warned in thick air). Reentry heating and glow, burn-up if too steep, heat shield. Parachute (tears if opened too fast). Land or splash down on Terra's new continents and oceans. New milestone **Round Trip**. New keys `Enter`, `F`, `P`; new Mobile action button (SKIP / FAIRING / CHUTE). Help screens updated for both. Saves from v0.1.0 and v0.2.0 still load.
- **v0.2.0**: Plays on phones. A PC or Mobile choice every time the game opens (also switchable from the menu). Mobile mode has on-screen buttons: throttle slider with FULL/CUT, hold-to-turn buttons, STAGE, SAS, Map, time warp, zoom (pinch or buttons) and Menu, and several fingers work at once. Bigger, tidier menus on small screens, a "turn your phone sideways" hint, notch-safe layout, and a lighter graphics setting on phones for smooth play. PC mode plays exactly as before, and v0.1.0 saves still load.
- **v0.1.0**: First playable. Three rockets, Terra and Luna, real orbits (patched conics, exact on-rails orbits during time warp), air drag, staging, landing/crash rules, map with orbit and encounter prediction, time warp, Tracking Station, milestones, records, sound, and a fully persistent auto-saved world with backup download/upload.

## What this is

Space Prime is a rocket flight game inspired by Ellipse: Rocket Simulator and Spaceflight Simulator. It is an original game: do not copy art, assets, music, or code from those games, just the kind of play they offer — launch a rocket, fly it, get into orbit, and land on other worlds.

## Who plays, and on what

- One player only: Armando. Single-player only. No multiplayer, no accounts, no login needed to play.
- PC in a desktop browser (keyboard and mouse), and, since v0.2.0 at Armando's request, phones in a mobile browser (on-screen touch buttons).

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
