🎵 The Mystic Octave (Tyrian Piano)

A zero-dependency, browser-based virtual piano inspired by the dark fantasy aesthetic of Guild Wars 2. It features dynamic key remapping, magical synthesized instruments, and a fully custom native .sf2 (Soundfont) parser built entirely in vanilla JavaScript.

[Insert a screenshot of the app here]
(Tip: Take a screenshot of the piano, save it as screenshot.png in your repo, and replace this line with ![Mystic Octave Screenshot](screenshot.png))

✨ Features

Native Soundfont Support: Upload any .sf2 file directly into the browser. The app parses the binary RIFF chunks, reconstructs the instrument presets, calculates volume envelopes (ADSR), and repitches raw PCM audio on the fly—all without a single external library.

Magical Synthesizers: Don't have a Soundfont? Play immediately using 4 built-in procedural Web Audio API synthesizers: Lute, Brass, Flute, and Crystal.

Dynamic Keybinding: Easily remap any piano key or octave control to any button on your keyboard.

Guild Wars 2 Aesthetic: Immersive UI with tarnished gold, dark parchment, and fiery reactive keys.

Performance Features:

Extend Notes (Sustain pedal simulation)

Octave shifting with optional constraints (Low/Mid/High)

Polyphonic playback with velocity and envelope management.

Tomes of Melodies: Built-in links to community-sourced tabs/sheet music for easy playing.

🚀 Live Demo

(Note: If you enable GitHub pages, put your link here!)
Play the Mystic Octave Here

🎮 How to Play

Getting Started

Because the entire application is bundled into a single file, there is no installation or build step required!

Clone the repository or download virtual_piano.html.

Double-click virtual_piano.html to open it in any modern web browser.

Start typing!

Default Controls

Keys 1-8 or Numpad 1-8: Play the C Major Scale (C, D, E, F, G, A, B, C)

Q / E: Shift the Octave down or up.

Don't like the defaults? Click Edit Binds: OFF to toggle remapping mode, click the key you want to change, and press your desired keyboard button!

🛠️ Technical Details

This project acts as a powerful demonstration of the browser's native capabilities:

Single-File Architecture: All HTML, CSS (via Tailwind CDN), and JavaScript logic is contained within one file for ultimate portability.

Web Audio API: Generates procedural sound waves, filters, and gain envelopes from scratch.

Binary Data Parsing: The JavaScript utilizes DataView and ArrayBuffer to manually traverse the complex binary RIFF structure of Soundfont files, interpreting generator zones, instrument bags, and raw audio slices natively.

📝 License

This project is open-source and available for anyone to use, modify, and learn from.

(Disclaimer: This project is fan-made and not affiliated with ArenaNet or Guild Wars 2.)
