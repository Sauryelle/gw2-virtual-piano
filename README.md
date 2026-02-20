# 🎵 Sarya's Play Thingy (Tyrian Piano)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Vanilla JS](https://img.shields.io/badge/Made%20with-Vanilla%20JS-f7df1e)

A zero-dependency, browser-based virtual piano inspired by the dark fantasy aesthetic of *Guild Wars 2*. It features dynamic key remapping, magical synthesized instruments, and a fully custom native **.sf2 (Soundfont) parser** built entirely in vanilla JavaScript.

---

## ✨ Features

* **Native Soundfont Support:** Upload any `.sf2` file directly into the browser. The app parses binary RIFF chunks, reconstructs instrument presets, calculates volume envelopes (ADSR), and repitches raw PCM audio on the fly—all without a single external library.
* **Magical Synthesizers:** Don't have a Soundfont? Play immediately using 4 built-in procedural Web Audio API synthesizers: *Lute, Brass, Flute, and Crystal*.
* **Dynamic Keybinding:** Easily remap any piano key or octave control to any button on your keyboard.
* **Tyrian Aesthetic:** Immersive UI with tarnished gold, dark parchment, and fiery reactive keys inspired by the Guild Wars 2 interface.
* **Performance Features:**
    * **Sustain Simulation:** Extend notes for a richer sound.
    * **Octave Shifting:** Constraints for Low, Mid, and High ranges.
    * **Polyphonic Playback:** Full velocity and envelope management.
* **Tomes of Melodies:** Built-in links to community-sourced tabs and sheet music.

## 🚀 Live Demo

**[➔ Play The Mystic Octave Here](https://sauryelle.github.io/gw2-virtual-piano/)**

---

## 🎮 How to Play

### Getting Started
Because the entire application is bundled into a single file, there is no installation or build step required!

1.  **Clone** the repository or download `virtual_piano.html`.
2.  **Double-click** `virtual_piano.html` to open it in any modern web browser.
3.  **Start typing!**

### Default Controls
* **Keys 1-8 / Numpad 1-8:** Play the C Major Scale (C, D, E, F, G, A, B, C)
* **Q / E:** Shift the Octave down or up.
* **Customization:** Click `Edit Binds: OFF` to toggle remapping mode, click the key you want to change, and press your desired keyboard button.

---

## 🛠️ Technical Details

This project is a demonstration of the browser's native power:

* **Single-File Architecture:** All HTML, CSS (via Tailwind CDN), and JavaScript logic is contained within one file for ultimate portability.
* **Web Audio API:** Generates procedural sound waves, filters, and gain envelopes from scratch.
* **Binary Data Parsing:** Utilizes `DataView` and `ArrayBuffer` to manually traverse the complex binary **RIFF structure** of Soundfont files, interpreting generator zones, instrument bags, and raw audio slices natively.

---

## 📝 License

This project is open-source and available for anyone to use, modify, and learn from.

**Disclaimer:** *This project is fan-made and not affiliated with ArenaNet or Guild Wars 2. All aesthetic inspirations belong to their respective owners.*
