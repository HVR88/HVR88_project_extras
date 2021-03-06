The downstream BC fork's repo is private at the moment. Request access or wait until it's made public again. Windows binaries of the cores are available as Release 1.0 in the base HVR88/vice-libretro repo for now:
* https://github.com/HVR88/vice-libretro/releases/
# VICE Libretro - Border Cropping (BC) Edition - Pixelpiper 2020

This project fork adds options to fit/fill any monitor of any aspect ratio, size or resolution, with perfectly scaled, non-distorted emulator screens at each platform’s correct aspect ratio - the resulting output will closely match the proportions/dimensions originally seen on a CRT/TV.

Output and features will work with all displays/monitors: 16:9, 16:10, 5:4, 4:3, LCDs, CRTs, etc. at any desktop resolution - including portrait-rotated modes/displays.

## Features ##
* Quick Zoom/Border Cropping presets
  * Small, Medium and Full border cropping - both width & height
  * Fit to Narrow & Fit to Wide (screens) - width or height
  * Custom cropping - displays additional options below
  
* Separate Width & Height cropping options for C64, C128, Vic-20 and C16/Plus4 cores
  * Preset-based with 3 crop settings for Width & 4 for Height, including complete border removal
  * Supports PAL & NTSC for every platform with appropriately-selected cropping presets for both Width and Height
  * No buggy side-effects of the Display Border Off option

* Manual Height Cropping Option for C64 and C128 cores - make the output perfectly fit any game
  * Independent Top and Bottom Cropping settings from 0 to 60 pixels (NTSC cropping restricted to match PAL range)
  * With support for over-cropping beyond the border to work with widest-possible range of games/titles

* Three new 4:3 normalized Pixel Aspect Correction options
  * Tweak to make NTSC/PAL fill similar/same amount of space (crop safe)
  * Ratios based on fitting full Vice region-specific resolutions to 4:3 CRT

* Virtual Keyboard scaling
  * Adapts to cropped height as necessary
  
* Hot Key to toggle (ON/OFF) the currently set Quick Zoom / Cropping preset

* Hot Key to cycle through the Quick Zoom / Border Cropping presets

* Hot Key to cycle through the presets for Width Cropping

* Hot Key to cycle through the presets for Height Cropping - includes Manual Crop setting

* Reorganized & relabeled Core Options for quicker access and ease of use

## Screenshot of Core Options ##

![Screenshot](https://github.com/HVR88/HVR88_project_extras/blob/master/VICE%20Libretro%20BC%20Edition-small.png)


Requirements: **Retroarch settings: Video settings -> Scaling -> Aspect Ratio: Core Provided + Integer Scaling: OFF**

***
The new options have been adopted by the emulation community and a large collection of games have been profiled to provide the optimal crop values to work on any display in the *C64 Dreams Curated Collection:* https://forums.launchbox-app.com/topic/49324-c64-dreams-massive-curated-c64-collection

**What others have said**

*”now 100% of the cropping is handled in the core itself, [RetroArch] video settings are untouched. This is a godsend because now it should “just work” for everyone. Equally important is that now that I can adjust these crops by single pixels, they’re more exact than the previous pre-defined zoom levels.”*

*”I’ll be honest, I wish every core had this option. I would use it. At the very least Beetle PSX and Beetle Saturn could really use it.Thank you for doing this! It resolves probably the single biggest issue with this project, so that’s a major boon.”*

