# Convertisseur MIDI ↔ Hex + Mappage Behringer Wing

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
- Paramètres FX

## Sources
Documentation MIDI Wing (Patrick-Gilles Maillot / Behringer World Wiki)

---
Créé pour faciliter le contrôle MIDI de la Behringer Wing (scènes, snapshots, custom controls…).
