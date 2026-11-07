# Slopefall · The Seam of Ash

A short single-player top-down browser adventure for MATH 101. Learn the controls at Lantern Camp, then descend through Lantern Causeway, the Spikeworks, and the Hollow Vault. Align each bridge, take the ladders down, and recover the Ember Lens.

## Run and play

Open [dist/index.html](dist/index.html) in a current desktop browser. Keep the dist/assets folder beside the HTML file for the title artwork and dungeon sprites. The game has no external dependencies. To play on Android, serve the dist folder over HTTP or HTTPS and open that address in the phone browser. The game fills the viewport. Settings includes a Fullscreen toggle where the browser permits it.

| Action | Desktop | Touch |
| --- | --- | --- |
| Move | WASD or arrow keys | Left thumbstick |
| Interact | E | Interact |
| Dash | Space | Dash |
| Strike | J | Attack |
| Pause or go back | Esc | Pause or Back |

Amber circles warn of steam bursts and spikes. Red arrows warn of creature lunges. Walk around danger, dash through it, or face a creature and strike within reach. At zero health, choose **Retry checkpoint**. Checkpoints are recorded when you enter a floor and when its bridge aligns. Each ladder starts the next floor at full health. Supply chests on the deeper floors restore one heart when opened while injured. **Resume** preserves the current run. **Continue** restores the saved checkpoint. Volume controls persist in browsers that allow local storage.

## Deploy on Vercel

Import this GitHub repository in Vercel and leave **Root Directory** at the repository root. The included `vercel.json` selects the **Other** framework preset, skips install and build, and publishes `dist`. Select **Deploy**. The game opens at the deployment's root URL.

For an existing Vercel project, check its root directory and redeploy the latest commit from `main`.

## Classroom demo

1. Start a new run. Point out the camp marker, the objective, and the dash cooldown. Follow the lanterns east.
2. At the bridge, leave the lever at **b = 0**. Walk east along the left deck and try crossing. Show the two edge markers and the blocked seam.
3. Open **How it works** on the lever or read the stone tablet. For x < 2, the profile is f(x) = x + 1. For x ≥ 2, it is f(x) = x + b. At b = 0 the left-hand limit is 3 and the right-hand limit is 2. The two-sided limit does not exist, so the crossing stays closed.
4. Set **b = 1**. The right deck rises and both one-sided limits equal 3. Since the function is defined at the seam and f(2) = 3, the profile is continuous at x = 2. Wait for the deck to lock, cross, and interact with the ladder. Repeat the mechanic on the deeper floors and retrieve the lens in the Hollow Vault. Setting **b = 2** puts the right edge at 4 and also blocks the crossing.

## Credits

Original game, knight sprite, map, interface, sound effects, and synthesized looping score created for Slopefall. The knight armor uses colors from the supplied Knight Studio preset. Dungeon props, floor textures, and trap frames come from Medieval + Dungeon Pixel Bundle (CC0). Void Abyss Jelly and Magma Rune Golem animations come from Fantasy Creatures Bundle (CC0 1.0). The lantern knight title illustration was generated for this game. The art direction draws on the compact top-down readability of Soul Knight and the shadowed atmosphere of Hollow Knight. Course references are MATH 101 Chapter 4, *Limits and Continuity*, and the *Semestral Project Guidelines*. Basic Trigonometric Derivatives is reserved as a separate concept for a future revision.
