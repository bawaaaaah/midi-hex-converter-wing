# Convertisseur MIDI ↔ Hex + Mappage Behringer Wing

*[Read in English](README.md)*

🔗 **Page en ligne :** https://bawaaaaah.github.io/midi-hex-converter-wing/

Outil local (page HTML unique) pour :

- Convertir une commande MIDI (CC, Program Change, Note On/Off, etc.) en code hexadécimal
- Convertir un code hex en description MIDI lisible
- Consulter le **mappage MIDI complet de la Behringer Wing** (Faders, Mutes, DCA, Custom Controls, Scènes / Show Control, FX…)

## Utilisation

Ouvre simplement `index.html` dans n’importe quel navigateur moderne.  
Aucune installation, aucune connexion internet requise.

### Onglet Convertisseur
- Combobox pour le type de message
- Canal MIDI 1-16
- Champs dynamiques selon le type
- Génération du code hexa propre
- Analyse inverse (hex → MIDI) avec détection spéciale des commandes Wing (CH7/CH8/CH9)

### Onglet Mappage Wing
Tableau complet :
- CH1 Faders / CH2 Mutes / CH3 Pan
- CH4 DCA Faders / CH5 Mute Groups
- CH6 Custom Controls
- CH7 Scene Change (index)
- CH8 Scene Tag (#1–#128)
- CH9 Show Control (GO / PREV / NEXT)
- Paramètres FX (CH9–16) : Insert / Mix / Modèle / Param 1-32 (FX1-8) ou 1-33 (FX9-16), **plus la liste complète des ~62 modèles d'effets FX1-16** (effets standards et premium) avec leurs paramètres OSC dans l'ordre des CC, tirée de l'appendix *Effects and Plugins' Parameters list* du protocole WING

## Sources
- [WING Remote Protocols](https://drive.google.com/file/d/1-iptgd2Uxw4qPEbmegG2Sqccf8AbRRfk/view) (Patrick-Gilles Maillot) — protocole OSC/MIDI/SYSEX complet, dont l'appendix Effects and Plugins' Parameters list
- [WING Effects Guide](https://cdn-media.empowertribe.com/60af52fb37824ce891703cfaecf4d8d0/M_BE_0603-AEN_WING%20EFFECTS%20GUIDE%20DARK1_WW.pdf) (Behringer) — description illustrée des effets et plugins

---
Créé pour faciliter le contrôle MIDI de la Behringer Wing (scènes, snapshots, custom controls…).
