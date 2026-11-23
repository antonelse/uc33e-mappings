# Evolution UC33e: mapping procedure and reference

This file is the general reference for the UC33e. The per-device mappings live in their own folders (see the README index).

## Mapping process

For each parameter, perform two operations on the UC33e: **Assignment** and **Storage**.

### 1. Assignment
- Move the desired knob, fader or button to focus on it.
- Press **ASSIGN** and set the CC value with the keypad.
- Press **CHANNEL** and set the MIDI channel.

### 2. Storage
- Press **STORE** and choose the preset number (for example 20 for P20).

**Important:** wait until the screen stops blinking before going on.

## Memory dump and restore

Use [SysEx Librarian](https://www.snoize.com/SysExLibrarian/) with a MIDI2USB cable for I/O. You can also send MIDI over USB with **MIDI OUT FROM USB** (press SELECT + ASSIGN together).

### Dump
- Connect the MIDI2USB to the UC33e OUTPUT MIDI port.
- In SysEx Librarian, select the correct input source and press *Record Many*.
- On the UC33e press MEM.DUMP (DATA MSB + STORE). The screen shows *SYS* while transmitting.

### Restore
- Connect the MIDI2USB to the UC33e INPUT MIDI port.
- In SysEx Librarian, select the correct output source, choose the SysEx file and press *Play*.
- The screen shows *SYS* while receiving.

### Load a preset
- Press RECALL and enter the preset number.

The complete dump of the controller is `complete_dump_UC33e.syx` in the repository root.

## Shortcuts
- **Reset UC33e:** power on while holding + and -.
- **Lock UC33e:** press CTR MUTE (PROGRAM + DATA LSB).
- **Send snapshots:** press SNAPSHOT (+ and -).
- **MIDI out via USB:** press SELECT + ASSIGN together.

## Tips
- **Channel assignment:** press CHANNEL and move each control in turn. Use + and - to change the value on screen.
- **CC assignment:** press ASSIGN and move each knob in turn, entering the CC number on the keypad as you go.
- **Check:** move the controls while watching the screen to confirm CC and channel values.
