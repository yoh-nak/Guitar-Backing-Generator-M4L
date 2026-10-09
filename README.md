# Guitar Backing Generator for Max for Live

**Guitar Backing Generator** is a free Max for Live MIDI device for Ableton Live that turns incoming MIDI chords into guitar-style backing patterns, arpeggios, and hybrid performances.

It is designed to work with a wide range of MIDI guitar instruments and other GM-compatible instruments without relying on a particular sample library or proprietary articulation keyswitches.

This repository includes **v1.0** and **v2.0**. **v2.0 is recommended** for new projects.

## What's New in v2.0

- **623 global presets** across **12 families** and **81 genre categories**
- Three-level **FAMILY → GENRE → PRESET** browser
- One-click preset selection that updates the performance parameters together
- Backing, arpeggio, and hybrid performance modes
- Expressive strumming, picking, voicing, bass movement, damping, and chord release
- Rhythm, swing, velocity accents, variation, and humanization controls
- Recorded MIDI display with **VEL / CC / BEND / AT / ALL** views
- **RECORD / STOP**, **WRITE CLIP**, **NEW TAKE**, and **APPEND TAKE**
- **EXPORT MIDI** with MIDI notes and available CC, Pitch Bend, and Aftertouch events
- Improved recording timeline behavior and optimized internal processing

## Supported Styles

Presets cover a broad selection of styles, including pop, J-pop, rock, metal, punk, acoustic, folk, country, blues, funk, soul, R&B, jazz, Latin, reggae, ska, electronic, ambient, cinematic, classical, flamenco, and more.

Different presets combine rhythm patterns, voicing, picking, strumming, dynamics, and note-length settings. They are editable starting points rather than separate instrument engines.

## Getting Started

1. Download [`Guitar_Backing_Generator_v2.0.amxd`](Guitar_Backing_Generator_v2.0.amxd).
2. In Ableton Live, place the device on a **MIDI track before a MIDI instrument**.
3. Choose the input source and the **BACKING**, **ARPEGGIO**, or **HYBRID** mode.
4. Select a **FAMILY**, **GENRE**, and **PRESET** to load the corresponding settings.
5. Play or route MIDI chords into the device, then adjust individual parameters if needed.
6. Use **RECORD / STOP** to capture the performance.
7. Use **WRITE CLIP** to create a note-based Live clip, or **EXPORT MIDI** to preserve additional MIDI controller events.

## Performance Parameters

Depending on the chosen mode and preset, controls include:

- **Strum Range:** Restricts the simulated string/register range.
- **Stroke Dynamics:** Changes the relative emphasis of strokes and notes.
- **Mute / Damp:** Controls short, muted, or sustained note lengths.
- **Voicing:** Adjusts the chord-note arrangement.
- **Bass Movement:** Varies low-note movement within the accompaniment.
- **Variation:** Introduces changes across bars.
- **Picking Style:** Selects different picking or brushing behaviors.
- **Chord Release:** Adjusts note cutoffs around chord changes.
- **Groove / Swing / Accent / Humanize:** Shapes rhythmic feel and dynamics.

The musical result depends on the input chords and the receiving instrument. MIDI note patterns can approximate guitar performance, but they do not reproduce every physical guitar technique automatically.

## Important: WRITE CLIP vs. EXPORT MIDI

**WRITE CLIP does not preserve CC, Pitch Bend, or Aftertouch in the Live clip.**

| Operation | MIDI Notes | CC | Pitch Bend | Aftertouch (AT) |
| --- | :---: | :---: | :---: | :---: |
| **WRITE CLIP** | Yes | **No** | **No** | **No** |
| **EXPORT MIDI** | Yes | **Yes*** | **Yes*** | **Yes*** |

\* When those events have been recorded or generated.

**To retain CC, Pitch Bend, or Aftertouch, you must use EXPORT MIDI and then import the exported MIDI file into Ableton Live.** Using WRITE CLIP alone will lose those controller events.

Some instruments do not respond to Aftertouch or may use different Pitch Bend ranges and CC mappings. Check the settings of your receiving instrument.

## General MIDI Compatibility

The device primarily uses standard MIDI notes, note velocities, timing, note lengths, and common controller messages. Its basic accompaniment functions do not require proprietary guitar keyswitches.

**GM compatibility does not guarantee identical articulations or controller response across all guitar instruments.** In particular, pitch bend range and Aftertouch behavior depend on the instrument.

## Versions and Downloads

| Version | Description |
| --- | --- |
| **[v2.0](Guitar_Backing_Generator_v2.0.amxd)** | Recommended: expanded global presets, improved expressive controls, MIDI export, recording display, and performance optimizations |
| **[v1.0](Guitar_Backing_Generator_v1.0.amxd)** | Original version, retained for reference and compatibility with older projects |

## Feedback and Contributions

If you find a preset, style, or playing technique that could be improved, please send feedback. Suggestions for more natural guitar phrasing and new genre-specific arrangements are especially welcome.

You may inspect the device's internal implementation, modify its code or presets, and share your own modified versions **for free**.

## Use and Redistribution

- **Free use** is permitted.
- **Modification** of the device and its presets is permitted.
- **Free redistribution** of the original or modified device is permitted.
- **Selling the original or modified device, or charging for its download or distribution, is not permitted.**
- Please retain this notice when redistributing a modified version. Attribution to the original project is appreciated.

These are the project's stated sharing conditions. See a separate `LICENSE` file if one is added later for formal licensing terms.

## Author

Created by [yoh-nak](https://github.com/yoh-nak) for the Max for Live community.

This is an independent project and is not affiliated with Ableton.
