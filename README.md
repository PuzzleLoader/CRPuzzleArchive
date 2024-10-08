# CosmicArchive
An Archive Of Every Cosmic Reach Version

<img src="/image.png"></img>

# Changelogs

# Pre-ALpha 0.3.2-pre5
Another discord-only development release, to hold you over for those who really can't wait for the fully fledged update.
- Fixed being unable to break leaves in multiplayer
- Disconnects are handled properly
- Fixed english tips being replaced by hungarian ones
- No clip flying down is now the same speed as flying up
- Fixed block positions causing crashes in negative coordinates

## Pre-Alpha 0.3.2-pre4
- Fix default path for windows causing crash on first save
- **This server is compatible with 0.3.2-pre2 clients**

## Pre-Alpha 0.3.2-pre3
- Potential fix for windows
- **This server is compatible with 0.3.2-pre2 clients**

## Pre-Alpha 0.3.2-pre2
Another discord-only development release, to hold you over for those who really can't wait for the fully fledged update.
- Chat is limited to 256 chars per message
- Fixed credits using the wrong charset
- Join message whenever a player enters the server
- Server uses jar location to store worlds + config
- Can break, place and interact with blocks in servers now. (some block events are only partially implemented)
- Various networking crashes fixed

## Pre-Alpha 0.3.2-pre1
This is a discord-only development release intended for modloaders to adapt to the new systems for multiplayer. Multiplayer will not function properly outside of basic actions like moving around.
- Added basic multiplayer via netty
- The client save directory is used, and the server cannot be configured yet
- All clients + server must have the same mods for expected results
- No account auth is used yet.

## Pre-Alpha 0.3.1
- Fixed axes not being effective towards wooden crates
- Fixed sounds not loading from their resource locations
- Fixed credits screen crashing
- Better error handling on block events
- Better logging on block state generators

## Pre-Alpha 0.3.0
- All mods and assets are now namespaced, data mods must be in the path `/mods/YOUR_NAMESPACE/YOUR_ASSET_FOLDER/YOUR_ASSET`
- For example, if I added a banana item, it would be under the path in the save directory `/mods/my_banana_mod/items/banana.json`
- Please refer to the base assets as examples on how to migrate your data mods to 0.3.0
- Items now have tooltips
- Credits scroll faster when holding the sprint or jump keybinds
- Tools are only damaged if blocks have a hardness greater than 0
- Saplings no longer block light
- Normals on saplings are now fixed
- Saplings can only plant on valid blocks now
- Added `canPlace` predicate to sapling
- Dropped block_ prefix from block json file names
- Moved `isTransparent` and `cullsSelf` flags to from blockstate to model files
- Models and textures are now referenced by their identifier in files
- Refactored language files to support tooltips and mods, added translation keys for blocks and items

## Pre-Alpha 0.2.5
- Added /skylight command
- Added credits screen
- Added community contribution: 3D Item models
- Reduced frequency of iron ore generation
- Poplar trees now have their own leaves and saplings
- Added new block event: `base:loot_drop` which allows blocks to have a custom loot table

## Pre-Alpha 0.2.4
- You can now paste seeds directly in the world creation screen
- The cursor now resets to the center of the screen when opening the inventory
- Fixed nostalgic islands world type never loading in
- Fixed mesh glitches when too many blocks are edited at once
- Fixed a bug where a single-block layer would upgrade to a bit layer with the wrong block
- Fixed respawning whenever the game restarts
- Fixed camera getting stuck looking straight down when away from the world origin

## Pre-Alpha 0.2.3
- Fix player respawning every time the world is loaded

## Pre-Alpha 0.2.2
- Fix crash in F3 debug menu when not looking at blocks
- Potential fix for cropped screenshots on certain mac computers

## Pre-Alpha 0.2.1
- Reduced vertex size
- Reduced in-memory representation of blocks and world sizes on disk
- Remove metal blocks from interceptor loot
- Fix spawn point to be dependent on the world seed
- Fixed world spawn being set in the air or in water
- Fixed bug where player is spawned with 10 out of 3 max HP
- Fixed block selection being interrupted while moving
- Fix mod asset loading for windows (Testers wanted!)
- Potential screenshot fix for mac (Testers wanted!)

## Pre-Alpha 0.2.0
- Added the new "Survival" world type
- Added `/time` command
- Added Poplar trees
- Added per-face normals, and blocks are now lit by the position of the sun
- Added iron and aluminium tools
- Added block hardness
- Spawn position is now random in a 5000 block radius from 0, 0
- Default sky for non-moon worlds is now dynamic, temporarily removed the lighting options
- Fixed bug freezing player on first world load
- Fixed falling through the floor when away from the original camera position on load
- Fixed modded items and recipes not loading on windows
- Removed `generateSlabs` flag from block states

## Pre-Alpha 0.1.50
- Fix crashing on breaking block in new world
- Fix crash on modded item overwriting an existing one

## Pre-Alpha 0.1.49
- Added item durability
- Furnaces now explode when smelting C4
- Temporarily added a rare chance for interceptors to drop gold ingots
- Allied interceptors are now cyan instead of green
- Furnace screen now closes when the furnace is broken
- Fixed modded items + recipes not loading in
- Fixed crash when a missing block is replaced with a modded item

## Pre-Alpha 0.1.48
- Items, furnace recipes, crafting recipes, and loot now load from data ( and data mods! )
- Player now starts at 3 max HP
- Added gold, aluminium, and iron for both ores and ingots
- Added a gold medkit, which increases your max HP by 1 up to a max of 10
- Can now tame interceptors using a gold ingot
- Can now double jump in creative to go into no-clip
- Sticks now take two planks instead of one
- Fixed player freezing upon teleporting or respawning
- Fixed bug where a crash would occur on absurd amounts of leaves
- Fixed furnace dropping its lit variant
- Fixed furnace being lit with a non fuel item in fuel slot
- Fixed bug where shift clicking into furnace caused a crash
- Fixed duplication bug when pressing drop item key in the crafting output
- Added a crash guard as a temporary fix until a rare bug with large amounts of meshes can be diagnosed

## Pre-Alpha 0.1.47
- Fixed tools not working

## Pre-Alpha 0.1.46
- Added a furnace
- Takes logs, planks, sticks, leaves, wooden crates, or magma as fuel
- Can smelt sand into glass, and stone into magma
- Added `/nightvision` command
- Added short aliases for commands (use the `/help` command for more details)
- Inventory UI now has higher contrast
- The world now saves its current time
- Fixed a huge lag spike when placing or breaking blocks near rainbows (_yes really_)
- Fixed a bug where clicking an empty item slot may crash the game
- Fixed severe flickering of water and leaves in the batch renderer

## Pre-Alpha 0.1.45
- Added block tags (For data modders: an arbitrary list of strings called `tags` in a blockstate)
- "Flicking" an item on the ground now plays a small sound
- Fixed a bug where selecting a different block would not reset the breaking timer
- Fixed the bug where player would freeze on making a new world
- Fixed ghost transparent blocks in the batch renderer
- Fixed bug where cursor slot had the wrong perspective for an item
- Fixed shifting clicking crafting outputs not stacking + output slot is now coloured differently
- Fixed sticks not stacking
- Fixed rare crash when breaking animation is exactly one
- Allow survival mode players to disable no-clip via hotkey
- Fixed shovels not being effective towards dirt
- Fixed missing block related crash when breaking with tool

## Pre-Alpha 0.1.44
- Added crafting system
- Added "2d" items
- Added medkit
- Added stick
- Added stone axe, pickaxe, and shovel
- Added `/die` command
- Added `/teleport` command
- Added `/gamemode` command (Use `/gamemode creative` and `/gamemode survival`)
- Can no longer instant-break blocks in survival mode
- Hitting items on the ground knocks them back
- Dynamic sky colour is now brighter on the horizon
- Chat text shadow is now darker
- Can no longer no-clip via hotkey in survival
- Fixed bottom of water clipping
- Adjusted metal panel + drone textures to be more saturated
- Debug screen shows bounding boxes of entities

## Pre-Alpha 0.1.43
- Held item is now independent of FOV
- Made picking up items easier
- Random ticks now only occur in immediately surrounding regions
- Fixed a bug where the player would freeze when making a new world
- Fixed item jitter
- Added commands, notably /noclip and /summon
- Sprinting now influences the FOV
- Adjusted sprinting and walking speed
- Fixed a rare batch rendering crash

## Pre-Alpha 0.1.42
- Fixed the stars spinning like crazy.

## Pre-Alpha 0.1.41
- The currently selected item is now shown in your first person "right hand".
- Support non english world names
- Fixed bug where you could drop the wrong hotbar item if the cursor is hidden and hovered over
- The world loader thread now sleeps when idle
- Really really long world names are truncated in the world selection menu
- Fixed leaf decay crash
- Item drops float when "inside" blocks
- Can pick up items one block up
- Stars now rotate in the Dynamic sky
- Gravity is stronger, the player is now less "floaty"
- Crates drop items when destroyed
- Items correctly display "0" when count is 0, and no longer display if count is 1.
- @Language Contributor  Localized the percent format for the loading screen
- Fixed the drone texture
- Camera far clipping plane now shrinks with lesser render distances

## Pre-Alpha 0.1.40
- Blocks now drop as items
- New block event: `base:item_drop`, which can take in a position and optionally `dropId` as an input parameter
- Picking block now chooses the "correct" block state
- Pressing the drop item key in the inventory can drop the item in the hovered slot
- Stairs and vertical slabs now placed based on camera orientation rather than raycast position
- Fixed freeze when picking up similar items in inventory
- Fixed being unable to reliably leave water when swimming
- Worlds are now sorted by last played
- All saved strings + files use UTF-8 wherever possible
- Fixed being able to go fullscreen with the mouse causing the game to be unplayable

## Pre-Alpha 0.1.39
- Fixed placed coconuts despawning after some time instead of growing trees
- Fixed leaf blocks growing into trees
- Fixed being unable to shift-click items when the hotbar is full

## Pre-Alpha 0.1.38
- Added coconut trees
- The nostalgic islands world type is now the default
- Added random ticks, available now in block events with the `onRandomTick` trigger
- Added the `base:increment_param` block event action
- Fixed storage screen flickering on the first frame
- Fixed being able to drop an item from another world
- Meshing optimizations
- Clicking outside of the inventory drops the cursor's item
- Clicking in the item catalog now deletes the cursor's item
- Health bar now flashes when dropping
- Fixed game not pausing after loading if window unfocused
- Drones no longer drop dirt, grass or tree logs

## Pre-Alpha 0.1.37
- Added a flying drone called the Interceptor
- Added a trap which spawns Interceptors
- Added a death screen
- Added damage effects
- Improved the main menu
- Added a difficulty setting: Currently only peaceful and normal are used.
- Can now drop items out of the inventory
- Fixed crash when creating a new world or respawning
- Fixed lighting calculations
- Moved game tick updates to a separate thread
- Fixed random frame-dependent camera jitter
- Fixed background threads not closing properly when the game crashes
- Region file version bumped to version 2
- Game can now save and load entities

## Pre-Alpha 0.1.36
- Fixed bug with black screen on creating a new world
- Fixed bug where cycling item types of a missing block would cause a crash

## Pre-Alpha 0.1.35
- Fixed bug where world would crash upon entering

## Pre-Alpha 0.1.34
- Can now cycle block types in hotbar, e.g. blocks/slabs/stairs (set to the " ` " keybind by default)
- Can now set the save game directory with command line option -s or --save-location
- World info now stores additional metadata
- Added 3D audio, with new play_sound_3d block event
- Fixed a bug where picking a missing block would cause a crash
- Fixed a bug where changing worlds would show a black screen until pausing
- Fixed bug where dropping an item could not be rebound to mouse buttons
- Fixed a regessing bug where the last transparent block in a chunk would still be visible after removal
- Space keybind is no longer blank when set
- More internal work on mobs

## Pre-Alpha 0.1.33
- Small hotfix to fix crashing when opening a crate
- Various translation fixes

## Pre-Alpha 0.1.32
- Added the "Dynamic Sky" lighting option
- Added mouse keybinds for placing / breaking blocks
- Slight inventory improvements
- Max stack size increased to 1000, displayed as 1K
- Breaking blocks adds it back to your inventory
- Significant batch renderer optimizations
- Improved the internal block entity API for modders
- Mac vertex format is now the same as on PC
- Various translation additions
- Added health bar
 
## Pre-Alpha 0.1.31d
Unknown. MacOS test version

## Pre-Alpha 0.1.31c
Unknown. MacOS test version

## Pre-Alpha 0.1.31b
Unknown. MacOS test version

## Pre-Alpha 0.1.31
- Fixed placed blocks above y=256 not saving
- Fixed huge lag spike when quitting to main menu
- Fixed item duplication bug
- Fixed a crash with the batch renderer
- Various translation improvements

## Pre-Alpha 0.1.30
- Hotfix to prevent worlds regenerating terrain and reverting placed blocks

## Pre-Alpha 0.1.29
- Added wooden crate
- Added gravel
- Added limestone
- Added gabbro stone
- You can now build at any height above y=0
- Inventory and hotbar are now saved
- Items are now limited, to a maximum stack size of 999x
- Significant memory and meshing optimisations
- Fixed frustum culling issues
- Introduced the 'naive' renderer, which is slower but potentially more stable for laptops
- You can now switch between the default 'batched' and the new 'naive' renderer in the settings
- Added block entity logic, with saving and loading
- Region file version has been bumped from 0 to 1
- Various translation fixes

## Pre-Alpha 0.1.28
- Added asphalt block
- Added Welsh, Serbian (also I forgot to mention Romanian from a previous update)
- Fixed wall running
- Fixed glitch-hopping when crawling near slabs
- Fixed glitching to the side of vertical slabs
- Fixed being unable to climb stairs with a vertical slab above
- Fixed block state generators not loading from the mods folder correctly
- Exposed debug info as public to java mods

## Pre-Alpha 0.1.27
- Various movement fixes
- Player no longer phases through blocks when sprinting
- Player no longer glitches into the ground when falling
- Glass stairs are no longer ugly
- Added stairs for metal panels, aluminium panels, and packed lunar soil
- Added Serbian and other localisation fixes

## Pre-Alpha 0.1.26
- Fixed glass slabs missing from the last update

## Pre-Alpha 0.1.25
- Added stairs for seamless blocks
- Added block state generators, which can create variants of blocks at startup
- `generateSlabs` is **deprecated,** please replace it with `"stateGenerators": ["base:slabs_all"]` in your data mods!

## Pre-Alpha 0.1.24
- Fixed a severe memory leak with the debug menu
- Added missing font glyphs for Croatian
- Added Bulgarian, Czech, and another dialect of Norwegian
- Various localization fixes

## Pre-Alpha 0.1.23
- Added Turkish, Hungarian, Danish, Sicilian, Catalan, Swedish, Croatian, Italian
- Fixed various localization issues
- Pre-alpha text will now try to fit on screen the best it can
- If text on buttons are too long, text will wrap to try to fit as well as it can

## Pre-Alpha 0.1.22
- The game has been translated to multiple languages, including Spanish, German, French, Norwegian, Dutch, Polish, Portuguese, Russian, and Ukrainian (thank you everyone for your contributions!)
- Introducing block events `base:set_cuboid`, `base:set_sphere` and `base:set_spherical_segment`
  - These block events allow for setting blocks en masse, and running triggers for each block before and after setting
  - Examples can be found in `assets/block_events/examples` in the jar file

## Pre-Alpha 0.1.21
- Made walking speed faster
- Made sprinting speed slower
- Macs can render the world now
- Fixed bug where blocks would go missing on a palette clean

## Pre-Alpha 0.1.20

- Adjusted water shader slightly
- Adjusted player physics in water
- Player walks slower now
- Potential fix for inputs being ignored when creating a new world
- Bottom of nostalgic islands world type now converts from missing to basalt stone

## Pre-Alpha 0.1.19
- Added back references to myself to the game (the guy who wrote the previous changelog has been canned.)
- Nostalgic islands now generate with stone at the bottom layer instead of lava- uh, I mean cheese.
- Got rid of foolish blocks
- Fixed bug where entering the keybinds menu would stop all keypresses from working
- Fixed the player's position not loading properly

## Pre-Alpha 0.1.18 (April Fools Update)
- FinalForEach has been cancelled so all references to him in the game have been removed.
- Added nostalgic island world type
- Added a hunger and health system for a true survival experience
- You can now eat cheese to restore health
- Added can... but no can opener (find another way to open it!)
- Added "red" "stone"
- Added Foreshadowing block
- Added a block that really doesn't want to exist
- Re-unused boombox
- Unacknowledged moonman
- Reverted atlas size increase
- Reverted reversion of atlas size increase
- Fixed worlds unloading incorrectly
- Triggers are now per-zone rather than per-game

## Pre-Alpha 0.1.17b blue
- Testing version for the block catalog for MacOS

## Pre-Alpha 0.1.17b red
- Testing version for the block catalog for MacOS

## Pre-Alpha 0.1.17
- Fixed crash on world selection screen when world seed was not set

## Pre-Alpha 0.1.16
- Added world creation screen
- Can set world name, seed, and type
- Added flat world type
- Fixed random crash with the Batched renderer
- Major internal changes, separating the concept of worlds and zones to prepare for multiplayer

## Pre-Alpha 0.1.15
- Fixed crash when chunk's palette size exceeded 128
- Palette is automatically cleaned up when exceeding a soft limit of 128 or hard limit of 4096
- Major internal refactors to prepare for multiplayer

## Pre-Alpha 0.1.14b
Unknown

## Pre-Alpha 0.1.14
- Added tickDelay to base:run_trigger
- Added debug crash button for an easy way to copy specs
- Fixed texture buffer sharing the same binding as the diffuse texture
- Fixed bug where missing blockstate id would crash when no default params specified
- Fixed open save directory bug on windows not catching AWTError

## Pre-Alpha 0.1.13d
Unknown

## Pre-Alpha 0.1.13c
Unknown

## Pre-Alpha 0.1.13b
Unknown

## Pre-Alpha 0.1.13
- Texture atlas size + precision increase using texture buffers.
- Added Max FPS Slider
- Fixed non-qwerty keybinds saving incorrectly
- Reduced max FOV to 150
- Fixed player-jittering in pause menu
- Fixed bug where zeroed view direction would freeze game
- Meshes no longer add border for null blocks

## Pre-Alpha 0.1.12g
- Adjusted atlas size for testing

## Pre-Alpha 0.1.12f
- UVs sent to the UBO are now checked for duplicates before expanding

## Pre-Alpha 0.1.12e
- Unknown

## Pre-Alpha 0.1.12d
- Unknown

## Pre-Alpha 0.1.12c
- Unknown

## Pre-Alpha 0.1.12b
- The textures atlas has been increased to 1024x, increasing the limit to 4096 different block textures (in 16x format).

## Pre-Alpha 0.1.12
- Added run_trigger to relay custom triggers
- Unlocked FPS when not using VSync
- Updates now work on a fixed-timestep tick system
- Position in debug menu now uses two decimal places
- Fixed swimming physics that behaved differently with different FPS
- Fixed being able to place or break blocks while paused

## Pre-Alpha 0.1.11
- Reverted the atlas size change.
- Reverted the UV texture precision.

## Pre-Alpha 0.1.10
- Runtime texture atlas size increased from 256x to 1024x
- Increased UV texture precision for blocks from 7 bits to 32 bits per axis
- Moved some code into save library https://github.com/FinalForEach/Cosmic-Reach-Save-Library
- Pressing ESC in the keybinds menu no longer leaves if keybind button is active
- Fixed freeze when creating world if render distance is invalid

## Pre-Alpha 0.1.9b
- A test for the inventory and open save directory button.

## Pre-Alpha 0.1.9
- Fixed vertical slab placement when not placing on the ground
- Fixed worlds not unloading on going to main menu
- Fixed bug where open directory would go to the containing folder on windows

## Pre-Alpha 0.1.8
- Added aluminium panels
- Slabs can now be orientated depending on placement position
- Removed debug printing from explosions, reducing lag
- Reduced stuttering at larger render distances
- Fixed bug on windows where the open directory buttons wouldn't open
- Fixed bug where non-english characters would crash the game

## Pre-Alpha 0.1.7
- Added C4
- All lights can toggle on interact now
- Fixed bug where light slabs being toggled would turn into full blocks
- Introduced new block event trigger: onExplode
- Introduced new block event action: base:explode
- Introduced new block event action: base:set_block_state_params

## Pre-Alpha 0.1.5d
- Changes to mesh and shader code specifically for MacOS

## Pre-Alpha 0.1.6b
- Vsync is no longer activated by default. On/Off option should properly toggle Vsync now
- Partial MacOS Support

## Pre-Alpha 0.1.6
- Added mouse sensitivity, FOV, and render distance sliders
- More work done towards mac support + a warning message that macs are not yet supported
- Selecting a block now takes into account its shape, not just its position
- Introduced the catalogHidden field for block states, hiding them from the item catalog by default

## Pre-Alpha 0.1.5c
- Fixed invisible world
- Partial MacOS Support

## Pre-Alpha 0.1.5b
- Partial MacOS Support

## Pre-Alpha 0.1.5
- Reverted the atlas size change

## Pre-Alpha 0.1.4
- Increased the runtime texture atlas size for blocks
- Block selection is now a wireframe
- Debug screen now shows the block you are looking at
- Work done towards mac support
- Keybinds should support non-QWERTY keyboards
- Fixed bug where multiple keybind buttons could be triggered at once

## Pre-Alpha 0.1.3
- Introduced Block Events, Triggers and Actions
- Fixed a bug where one of the faces on the default cube was flipped

## Pre-Alpha 0.1.2
- Pressing screenshot will notify you the file name
- Removing mods no longer corrupts the world
- Added world selection screen
- Inventory no longer duplicates items across pages
- Improved the default mouse sensitivity for wide screen resolutions

## Pre-Alpha 0.1.1
- Fixed the last item in the item catalog being unable to be added to the hotbar

## Pre-Alpha 0.1.0
- Adds packed lunar soil
- The blocks.png is overwritten at runtime, all block textures are separate files

## Pre-Alpha 0.0.14
- Fixes the last item in the catalog being omitted

## Pre-Alpha 0.0.13
- Fixed the inventory buttons not closing
- Fixed the water shader ruining the UI when escaped

## Pre-Alpha 0.0.12
- Fixed inventory slot bugs (unsure)

## Pre-Alpha 0.0.11
- Skipped Version

## Pre-Alpha 0.0.10
- Inventory pages
- Light slabs

## Pre-Alpha 0.0.9
- Fixed the last-transparent-block bug

## Pre-Alpha 0.0.8
- Fixed the menu F1 bug
- Shaders can now use an #import preprocessor

## Pre-Alpha 0.0.7
- Fixed alt-tabbing ruining the player file

## Pre-Alpha 0.0.6
- Allows all assets to be loaded from the mods folder

## Pre-Alpha 0.0.5
- Fixed crouching on slabs

## Pre-Alpha 0.0.4
- Code cleanup
- Update chunk-water shader

## Pre-Alpha 0.0.3
- Adds more error catching/logging to code

## Pre-Alpha 0.0.2
- Fixed no block destruction cool-down while in the inventory
- Added basic mod support

## Pre-Alpha 0.0.1
- Game Release
