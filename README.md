# MIDI ↔ Hex Converter + Behringer Wing Mapping

*[Lire en français](readme-fr.md)*

🔗 **Live page:** https://bawaaaaah.github.io/midi-hex-converter-wing/

Local tool (single HTML page) to:

- Convert a MIDI command (CC, Program Change, Note On/Off, etc.) into hexadecimal code
- Convert a hex code into a readable MIDI description
- Browse the **full MIDI mapping of the Behringer Wing** (Faders, Mutes, DCA, Custom Controls, Scenes / Show Control, FX…)

## Usage

Just open `index.html` in any modern browser.
No installation, no internet connection required.

### Converter tab
- Combobox for the message type
- MIDI channel 1-16
- Dynamic fields depending on the type
- Clean hex code generation
- Reverse analysis (hex → MIDI) with special detection of Wing commands (CH7/CH8/CH9)

### Wing Mapping tab
Full table:
- CH1 Faders / CH2 Mutes / CH3 Pan
- CH4 DCA Faders / CH5 Mute Groups
- CH6 Custom Controls
- CH7 Scene Change (index)
- CH8 Scene Tag (#1–#128)
- CH9 Show Control (GO / PREV / NEXT)
- FX Parameters

## Sources
Wing MIDI documentation (Patrick-Gilles Maillot / Behringer World Wiki)

---
Built to make MIDI control of the Behringer Wing easier (scenes, snapshots, custom controls…).
