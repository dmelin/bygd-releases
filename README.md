<p align="center">
  <img src="images/logo.png" alt="BYGD - a real-time hex-tile builder" width="460">
</p>

**Bygd** is a small real-time hex-tile builder. You draw terrain tiles, match patterns for coins (*Tegn*), spend them on farms, wells,
wood cutters and markets, and keep your villages supplied so they grow. Let a district go hungry or thirsty and it shrinks again.

This is an **early playtest build for friends** (version **0.6.1.1**). It is unfinished, it will have rough edges, and your feedback is exactly what it is for.

<p align="center">
  <img src="images/island.jpg" alt="An island with a walled town, farms, a market and a quarry" width="900">
</p>

<p align="center">
  <img src="images/levels.png" alt="One tile growing from a Village to a Big Town" width="900">
</p>

<p align="center">
  <img src="images/screenshot-game.png" alt="The game: the start of a run" width="800">
</p>

<p align="center"><a href="images/bygd_trailer.mp4"><b>Watch the 48-second trailer</b></a> (an early build: a map growing from nothing, no interface)</p>

## What is new in 0.6

- **The Fishing Hut** (unlocked with the Market): the only building that goes on water, on a water tile with grass next to it. It fishes for food from a boat, like a small farm.
- **New patterns:** for 20 Tegn all three patterns are replaced, and water, desert and mountain are much more likely than usual.
- **Pause:** press **Space** to stop the clock (nothing produces, nothing is eaten, no chests fill). It turns to night and the lights glow; the animations go on.
- **Gift tiles:** the Wood Cutter, the Quarry and the Mine each come with a tile in your Stash (a forest, a mountain, a mountain). Mountains also turn up more often, and a tile that has
  not been drawn for a while is drawn next.
- **Buy tiles** costs more each time you buy, and a warning under the Stash tells you when placing your last tile would end the game.
- **Smaller things:** Esc backs out of the menu step by step, the compass turns the camera back when clicked, tooltips are easier to read, less lag while you drag the map, and a few things
  to find. 0.5.0 brought the progression, the bigger towns and the market chests.

## Download and play (Windows)

1. Download the game from **[bygdgame.com](https://bygdgame.com)** (the button on the page), or directly: [Bygd-windows.zip](https://bygdgame.com/download/Bygd-windows.zip) (about 54 MB).
2. Unzip it anywhere and run **`Bygd.exe`**. There is no installer, and nothing else is needed.
3. Windows SmartScreen may say the app is unrecognised, because the build is not code-signed. Click **More info**, then **Run anyway**.

Needs a Windows 10 or 11 PC (64-bit) with a graphics card that supports Vulkan (anything from the last ten years or so). The interface
scales with the UI scale option in Settings.

## How to play

- **Tiles.** You get 60 terrain tiles in a run: three in the *Stash* on the left, the rest in a pile. Drag a tile onto a lit slot next to
  your land. Water, grass, forest, mountain and desert all behave differently.
- **Patterns.** The box at the bottom offers patterns such as "two forests and a lake". Click a pattern, then click the matching tiles on the
  board to claim it for Tegn. Every asset standing on the claimed tiles adds 10% to the reward.
- **Assets.** The toolbar at the top sells what you can build. Drag an item onto a free land tile; the price is taken when you drop it. New items appear as you progress.
  - **Village**: needs water and food. It grows with them and becomes a **Big Village** (needs wood too), a **Small Town** (stone goods) and a **Big Town** (tools). A settlement
    is worth 1, 3, 5 or 7 points by level. A settlement cannot level up while a neighbour is of a lower level.
  - **Well**: gives water, but only with a water tile within 2 hexes (the tiles that are too far light up amber while you drag it).
  - **Farm**: gives food and needs water. Drag another Farm onto it to level it up (sheep, then cows), which takes a pen tile with it.
  - **Wood Cutter**: goes on or next to a forest and takes the timber of one forest. Stack a second one for a Logging Camp, which needs a second forest next to it.
  - **Market**: gathers up to four producers and delivers their goods to the settlements around it. Its chest earns Tegn: click the Market to collect.
  - **Quarry and Mine**: on a mountain. A **Stone Mason** or **Smithy** right next to one turns its rock into stone goods, or its iron into tools.
  - **Fishing Hut**: goes on a water tile with grass next to it and fishes for 3 food; a Market can catch it. It cannot be upgraded.
  - **Demolish**: free; blows up a tile if you change your mind.
- **Supply.** Producers reach as far as their range allows, and roads make it reach further. A storage only takes what it can hold plus what it uses, so what one house does not
  need goes to the next. Roads and bridges appear by themselves between nearby assets.
- **Warnings.** A turning triangle over an asset means it is missing something. A green arrow over a village means it would level up with more supplies. Hover or click an asset
  to see exactly what it takes in, puts out and stores.
- **Out of tiles?** Once the pile and your hand are empty, **Buy tiles** lights up on the toolbar: three tiles for a price that climbs the more you have placed. If you place
  your last tile and cannot afford more, the run ends with a **Game Over** and your total score. You can close that panel to look at your world (and press U to bring it back).

### Controls

| Key | |
|---|---|
| Space | Pause and unpause (night falls while it is paused) |
| Esc | The menu: Resume, three save slots, Settings, Quit |
| Right-drag, Q / E | Rotate the camera |
| Middle-drag, Shift + drag, W A S D | Pan the camera |
| Mouse wheel | Zoom |
| U | Hide or show the interface (good for screenshots) |
| F3 | Frame rate and render stats |
| F6 / F7 | Try-out: level the settlement under the mouse up or down |

### Saving

Three save slots. The game saves itself into the slot you started it in every 20 seconds, when you open the menu and when you quit.
Pick a used slot in the menu to load or delete it. Every new game uses a fresh random world.

The settings menu has options for shadows, light, animations, MSAA, glow, depth of field, UI scale and volume. If it runs slowly,
turn off shadows or the effects first.

## Known gaps

Most sound effects (clicks and animals), balance, and what the desert is good for are all still to do. Market assignment is "sticky" after roads change. If you find a bug, a
confusing moment or a number that feels wrong, please tell me what you did, what you expected, and the version and seed shown in the top-left corner when you can.

## Credits

A game by Crooked Nail (Daniel Melin). Built with [Godot 4](https://godotengine.org). Made with help from Claude.
