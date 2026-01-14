# LES CERCLES

**Les Cercles** is a web-based generative music sequencer that combines orbital mechanics with physics-based interactions. It creates evolving musical patterns using "planets" that trigger sounds as they cross "gates" in their orbit, alongside a "slingshot" physics engine for chaotic, collision-based textures.

## Features

### Orbital Sequencer
* **Polyrhythmic Logic:** Create up to 32 "planets," each with independent RPM (speed), velocity, and note assignments.
* **Dynamic Gates:** Adjust the number of trigger gates (1-32) on the orbit path.
* **Transposition:** Gates can be assigned individual pitch shifts (transpositions), allowing a single orbiting note to play complex melodic lines.
* **Global Controls:** Real-time adjustment of global speed, orbit direction (CW/CCW), and master transposition.

### Physics Engine (The Orb)
* **Slingshot Mechanic:** Drag and release from the center to launch "orbs" into the arena.
* **Collision Modes:**
    * **Circle:** Orbs trigger sound when hitting the outer boundary.
    * **Gates:** Orbs trigger sound when crossing gate lines.
    * **Notes:** Orbs trigger sound when colliding with orbiting planets.
* **Generative Chaos:** Enable orb-to-orb collisions to create evolving, non-repeating rhythmic textures.

### Audio & MIDI
* **Synth Engine:** Built-in polyphonic web audio synthesizer (Triangle wave with lowpass filtering).
* **Music Theory:** Lock your sequence to various scales (Chromatic, Major, Minor, Pentatonic, Dorian, Lydian, Whole Tone) or create a **Custom Scale**.
* **Web MIDI Support:** Route note data to external hardware synthesizers or DAWs via the "MIDI..." dropdown.

## Controls

### Top Bar
* **AUDIO:** Toggle the audio engine on/off.
* **SETTINGS:** Open global settings for Root Note, Scale, and JSON Save/Load.
* **MIDI:** Select a MIDI output device.
* **VOL:** Master volume control.

### Main Controls
* **PLAY/PAUSE:** Start or stop the sequencer.
* **UNDO:** Revert the last action (supports up to 20 steps).
* **CLEAR:** Reset the entire scene.
* **SYNC:** Synchronize the RPM of all planets to match the first planet.
* **EVEN:** Evenly space all planets along the orbital path.
* **ORB:** Toggle the Slingshot/Orb panel.

### Macro Controls
* **CCW/CW:** Toggle orbit direction (Switches UI between Light and Dark mode).
* **GATES:** Set the number of trigger lines (1-32).
* **TRANSPOSE:** Shift the pitch offset of all gates.
* **RND:** Randomize the transposition values of current gates.
* **SPEED:** Global playback speed multiplier (0.1x to 3.0x).

## Usage

1.  **Initialize:** Click the screen to start the AudioContext.
2.  **Add Planets:** Use the **+** button in the bottom planet list to add new notes.
3.  **Edit Planets:** Click a planet chip to adjust its specific Note, RPM, and Velocity.
4.  **Launch Orbs:** Toggle "ORB" mode, then drag from the center of the circle to slingshot projectiles.

## Installation

Les Cercles is a standalone web application with zero dependencies.

1.  Clone the repository.
2.  Open `index.html` in any modern web browser.

## License

Copyright (c) 2026 Jerome Potter.  
Released under the MIT License.
