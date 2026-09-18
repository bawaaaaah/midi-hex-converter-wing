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
- FX Parameters (CH9–16): Insert / Mix / Model / Param 1-32 (FX1-8) or 1-33 (FX9-16), **plus the full list of the ~62 FX1-16 effect models** (standard and premium effects) with their OSC parameters in CC order, sourced from the *Effects and Plugins' Parameters list* appendix of the WING protocol

## Sources
- [WING Remote Protocols](https://drive.google.com/file/d/1-iptgd2Uxw4qPEbmegG2Sqccf8AbRRfk/view) (Patrick-Gilles Maillot) — full OSC/MIDI/SYSEX protocol, including the Effects and Plugins' Parameters list appendix
- [WING Effects Guide](https://cdn-media.empowertribe.com/60af52fb37824ce891703cfaecf4d8d0/M_BE_0603-AEN_WING%20EFFECTS%20GUIDE%20DARK1_WW.pdf) (Behringer) — illustrated description of the effects and plugins

---
Built to make MIDI control of the Behringer Wing easier (scenes, snapshots, custom controls…).
