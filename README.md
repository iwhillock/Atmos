by [Ian Whillock](ianwhillock.com)

Atmos is a Max for Live Device that allows the playback of sound files independent of the Ableton transport. 

---
### USE CASES
Atmos was built to play introduction, changeover, or exit material when clocking is still needed at an indeterminate time within the same Live Set. A Live Set can be played as normal, and when the transport is stopped, a soundfile can be automatically triggered. It can also be used creatively, adding the ability of flexible timing to compositions, while staying within the Live ecosystem. 

----
### COMPATIBILITY 
- Works only with MacOS. Tested with Apple Silicon, MacOS 15.6.1, November 2025.
### INSTALLATION
- Simply download the device and add it to where your Max4Live devices are stored

----
### NAMING
- Each Atmos device in a Live Set can be given a unique name. 
- This is to help organize multiple instances of the device, and also for external control.
### LOADING A FILE
- **before loading a file, the Live Set must be saved.**
- a file can be loaded by clicking the "LOAD" button, or by dragging and dropping a file onto the path name.
- all files within the live set used in the Atmos devices are stored in a Menu, and can be accessed with the green arrow. 
### PLAYBACK
- Fade in and fade out times: fade occurs when the soundfile is turned on or off. 
	- when a file is fading out, clicking the main button once more stops the file instantly.
	- hitting the "reset" button stops playback of all Atmos instances instantly.
- MIDI trigger on/off: each device can be triggered on or off with a midi note. 
- Oneshot: plays the sound file once from start to end
- Loop: loops a single sound file at the start and end of the soundfile.
- Crossfade: triggers, loops, and crossfades multiple instances of the soundfile for a smoother looping effect.

----
### OSC
- The name given to the device also functions as the OSC address.
- All Atmos devices are linked to port 666. 
##### MESSAGES
- /atmos/(name): turns the device on or off (changes state)
- /atmos/on/(name): starts the soundfile playback
- /atmos/off/(name): stops the soundfile playback
- /atmos/reset: stops all Atmos devices in the Live Set.

---
### FILE STRUCTURE
- Atmos automatically adds all files to a new folder "[project-folder]/Atmos", and searched for with a relative path. This means all files stay connected to your Ableton Project through the standard Ableton folder structure. 

