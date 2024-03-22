# CosmicArchive
An Archive Of Every Cosmic Reach Version

<img src="/image.png"></img>

# Changelog

## 0.1.12
- Added run_trigger to relay custom triggers
- Unlocked FPS when not using VSync
- Updates now work on a fixed-timestep tick system
- Position in debug menu now uses two decimal places
- Fixed swimming physics that behaved differently with different FPS
- Fixed being able to place or break blocks while paused

## 0.1.11
- Reverted the atlas size change.
- Reverted the UV texture precision.

## 0.1.10
- Runtime texture atlas size increased from 256x to 1024x
- Increased UV texture precision for blocks from 7 bits to 32 bits per axis
- Moved some code into save library https://github.com/FinalForEach/Cosmic-Reach-Save-Library
- Pressing ESC in the keybinds menu no longer leaves if keybind button is active
- Fixed freeze when creating world if render distance is invalid

## 0.1.9b
- A test for the inventory and open save directory button.

## 0.1.9
- Windows only: Fixed bug where open directory would go to the containing folder.
- Fixed worlds not unloading on going to main menu.
- Fixed vertical slab placement when not placing on the ground.

## 0.1.8
- Added aluminium panels
- Slabs can now be orientated depending on placement position
- Removed debug printing from explosions, reducing lag
- Reduced stuttering at larger render distances
- Fixed bug on windows where the open directory buttons wouldn't open (Testers wanted!)
- Fixed bug where non-english characters would crash the game

## 0.1.7
- Added C4
- All lights can toggle on interact now
- Fixed bug where light slabs being toggled would turn into full blocks
- Introduced new block event trigger: onExplode
- Introduced new block event action: base:explode
- Introduced new block event action: base:set_block_state_params

## 0.1.5d
- Changes to mesh and shader code specifically for MacOS

## 0.1.6b
- Vsync is no longer activated by default. On/Off option should properly toggle Vsync now
- Partial MacOS Support

## 0.1.6
- Added mouse sensitivity, FOV, and render distance sliders
- More work done towards mac support + a warning message that macs are not yet supported
- Selecting a block now takes into account its shape, not just its position
- Introduced the catalogHidden field for block states, hiding them from the item catalog by default

## 0.1.5c
- Fixed invisible world
- Partial MacOS Support

## 0.1.5b
- Partial MacOS Support

## 0.1.5
- Reverted the atlas size change

## 0.1.4
- Increased the runtime texture atlas size for blocks
- Block selection is now a wireframe
- Debug screen now shows the block you are looking at
- Work done towards mac support
- Keybinds should support non-QWERTY keyboards
- Fixed bug where multiple keybind buttons could be triggered at once

## 0.1.3
- Introduced Block Events, Triggers and Actions
- Fixed a bug where one of the faces on the default cube was flipped

## 0.1.2
- Pressing screenshot will notify you the file name
- Removing mods no longer corrupts the world
- Added world selection screen
- Inventory no longer duplicates items across pages
- Improved the default mouse sensitivity for wide screen resolutions

## 0.1.1
- Fixed the last item in the item catalog being unable to be added to the hotbar

## 0.1.0
- Adds packed lunar soil
- The blocks.png is overwritten at runtime, all block textures are separate files

## 0.0.14
- Fixes the last item in the catalog being omitted

## 0.0.13
- Fixed the inventory buttons not closing
- Fixed the water shader ruining the UI when escaped

## 0.0.12
- Fixed inventory slot bugs (unsure)

## 0.0.11
- Skipped Version

## 0.0.10
- Inventory pages
- Light slabs

## 0.0.9
- Fixed the last-transparent-block bug

## 0.0.8
- Fixed the menu F1 bug
- Shaders can now use an #import preprocessor

## 0.0.7
- Fixed alt-tabbing ruining the player file

## 0.0.6
- Allows all assets to be loaded from the mods folder

## 0.0.5
- Fixed crouching on slabs

## 0.0.4
- Code cleanup
- Update chunk-water shader

## 0.0.3
- Adds more error catching/logging to code

## 0.0.2
- Fixed no block destruction cool-down while in the inventory
- Added basic mod support

## 0.0.1
- Game Release
