# Making House Music Beats in Logic Pro X — Full Tutorial

For the team member working on Mac. Logic Pro X includes a large suite of professional instruments and effects that are ideal for house music production.

---

## 1. Project Template Setup

### Creating a House Music Template
1. **File → New from Template** or **File → New** and configure manually
2. Set BPM: click the tempo field in the LCD display → type your BPM (**126** is a good house starting point; range 124–130)
3. Time signature: **4/4** (default)
4. Sample rate: **File → Project Settings → Audio** → set to **44.1 kHz**
5. Buffer size: **Logic Pro → Preferences → Audio** → I/O Buffer Size: **256 samples** for production

### Template Track Layout
Set up these tracks once and save as a template (**File → Save As Template**):

| Track | Type | Purpose |
|-------|------|---------|
| Drums | Drummer or Software Instrument (Drum Machine Designer) | Main drum pattern |
| Kick Sub | Software Instrument | Sub-bass layered with kick |
| Bass | Software Instrument (ES2/Alchemy) | House bassline |
| Chords | Software Instrument | Pad/chord stabs |
| Lead | Software Instrument | Melody |
| Vocal Chops | Sampler | Vocal sample playback |
| FX | Audio/Software | Risers, sweeps |
| Drum Bus | Aux | Drum mix bus |
| Master | Output | Final output |

**Save the template:** File → Save As Template → "BSP House Template"

---

## 2. Drummer Track for House Patterns

The Drummer track uses Logic's AI drummer and is a fast way to get a realistic house groove.

### Setting Up Drummer
1. **Track → New Track → Drummer**
2. In the **Drummer Editor** (appears at the bottom), click the drummer name → browse genres
3. Select **"Electronic"** genre → choose a drummer style (Kyle and Tyrell work well for house)

### Customizing for 4-on-the-Floor House
1. In the Drummer Editor:
   - **Kick:** Drag the pattern selector toward "Simple" (steady 4-on-the-floor)
   - **Snare:** Set to beats 2 and 4
   - **Hi-hats:** Set to 1/8 notes with some variation
2. **Swing/Groove:** Adjust the **Swing** slider 10–20% to the right
3. **Complexity:** Keep complexity low-medium for classic house groove

### Converting to MIDI (for Full Control)
- Right-click the Drummer region → **Convert to MIDI Region**
- Now you can edit every note in the Piano Roll editor
- Add ghost notes (low velocity hits) between main beats

### Using Drum Machine Designer (DMD)
For complete sample control, use **Drum Machine Designer** instead:
1. **Track → New Software Instrument Track** → instrument selector → **Drum Machine Designer**
2. Drag your 909/808 samples onto the pads
3. Each pad routes to its own channel strip for individual EQ/compression
4. Open the Piano Roll to program patterns manually

---

## 3. ES2 / Alchemy for House Synths

### ES2 — Classic House Stabs and Bass
The ES2 is Logic's built-in analog-style synth, great for vintage house sounds.

**House bass preset setup (ES2):**
1. Insert **ES2** on a Software Instrument track
2. OSC1: **Sine** wave, level 100%, tune 0
3. OSC2: **Square** wave, level 40%, tune +12 semitones (one octave up)
4. **Filter:** Low-Pass (LP), Cutoff **600 Hz**, Resonance **15%**
5. **Amp Envelope:** Attack 0ms, Decay 200ms, Sustain 70%, Release 300ms
6. **Filter Envelope:** Slight positive amount, fast attack/decay for subtle filter pluck

**House chord stab with ES2:**
1. OSC1: **Saw** wave, level 100%
2. OSC2: **Saw** wave + 5 cents (unison detune)
3. OSC3: **Saw** wave - 5 cents
4. Filter: LP, Cutoff 3 kHz, Resonance 10%
5. Amp Envelope: fast attack, short decay, sustain 0% (stab shape)

### Alchemy — Lush House Pads
Alchemy is Logic's premium synth, excellent for evolving pads.

**Deep house pad:**
1. Start from **Init preset** → set source A to **Additive** mode
2. In Additive panel, use sine + low harmonics only
3. **ENV1 (amplitude):** Attack 500ms, Decay 1s, Sustain 80%, Release 2s
4. Add **Modulation:** LFO → Cutoff (subtle, slow rate ~0.1 Hz) for animation
5. Enable **Wide** button for stereo spread
6. Apply Logic's **ChromaVerb** (see Step 4) via a Send for reverb tail

---

## 4. Space Designer for Reverb

Space Designer is Logic's convolution reverb — one of the best included with any DAW.

### Setting Up a Reverb Send (the correct way)
1. Create an **Aux track** (Mix → Create New Auxiliary Channel Strip)
2. Insert **Space Designer** on the Aux
3. On each instrument track, use the **Send** knob (in the mixer) to send signal to the Aux
4. Set Space Designer Dry/Wet to **100% wet** — the dry signal comes from the source track

### Space Designer Settings for House

| Use | IR or Preset | Size | Pre-delay | Decay |
|-----|-------------|------|----------|-------|
| Snare room | "Medium Room" preset | 30–40% | 10–20ms | 0.5s |
| Pad ambience | "Large Hall" preset | 60% | 0ms | 2–4s |
| Vocal chop | "Plate" preset | 50% | 30ms | 1.5s |
| FX riser | "Dark Space" preset | 80% | 0ms | 3s+ |

**Pro tip for house:** Keep the **kick drum dry** (no reverb or very minimal). Reverb on kicks makes the low end muddy.

---

## 5. Flex Time and Flex Pitch for Samples

### Flex Time (Rhythmic Correction)
1. In the main Tracks area, click **Edit → Show Flex Pitch/Time** or press **Cmd+F**
2. Click the flex icon on an audio track → choose **Rhythmic** mode for drum loops, **Monophonic** for bass
3. Transient markers appear — drag them to snap to the grid or adjust timing

**Slicing a vocal sample:**
1. Enable **Slicing** flex mode on the vocal track
2. Flex markers auto-detect transients
3. Drag individual slices to rearrange in time → creates chop-style rearrangements

### Flex Pitch (Melodic Correction and Pitch Shifting)
1. Select an audio region → **Audio → Show in Track Editor** → click **Flex Pitch** button
2. Blue pitch blocks appear for each detected note
3. Drag blocks vertically to change pitch (semitone snapping by default)
4. **Fine tune:** double-click a block to see sub-semitone fine tune
5. **Vibrato and formants:** available per note in the editor

**For vocal chop pitch mapping:**
1. Take a one-syllable vocal sample
2. Use Flex Pitch to create 5–7 versions at different pitches
3. Bounce each pitch as audio → load into Sampler across different keys

---

## 6. Stem Export Workflow

### Preparing for Stem Export
Before exporting, ensure your project is finalized:
- All tracks have consistent gain staging
- Master channel has no peak limiting that affects individual stems
- All virtual instruments are bounced to audio (for faster export)

### Method 1: Solo and Bounce Per Track
1. Solo the track group (Drums, Bass, Chords, etc.)
2. **File → Bounce → Project or Section** (or Cmd+B)
3. Settings: WAV, 24-bit, 44100 Hz, **normalize: Off**
4. Repeat for each group

### Method 2: Export All Tracks (Logic Pro 10.7.5+)
1. **File → Export → All Tracks as Audio Files**
2. Logic exports every track or bus simultaneously
3. Set destination folder: `BSP/Stems/BeatName/`
4. Format: WAV 24-bit, 44100 Hz

### Stem Naming Convention
```
BSP_BeatName_BPM_Key_STEM_Drums.wav
BSP_BeatName_BPM_Key_STEM_Bass.wav
BSP_BeatName_BPM_Key_STEM_Chords.wav
BSP_BeatName_BPM_Key_STEM_Lead.wav
BSP_BeatName_BPM_Key_STEM_VocalChops.wav
BSP_BeatName_BPM_Key_STEM_FX.wav
BSP_BeatName_BPM_Key_MASTER.wav
BSP_BeatName_BPM_Key_TAGGED.mp3
```

### Tagged MP3 Export
1. Add your beat tag (audio clip) as a track that triggers at 30 seconds
2. **File → Bounce → Project or Section** → choose MP3 → 320 kbps
3. Filename: `BSP_BeatName_BPM_Key_TAGGED.mp3`

### Sending Project Files to the Team
- Logic project files (`.logicx`) are macOS-only — teammates on Windows cannot open them
- For cross-DAW collaboration: bounce all stems to WAV and share via Google Drive
- Always include a **MIDI export** of all patterns (File → Export → Export All MIDI Regions as MIDI File) for portability

---

## Quick Reference: Logic Pro Keyboard Shortcuts for House Production

| Action | Shortcut |
|--------|---------|
| Play/Stop | Space |
| Record | R |
| Open Piano Roll | P (with MIDI region selected) |
| Open Mixer | X |
| Open Smart Controls | B |
| Bounce (export) | Cmd+B |
| Create Drummer track | Cmd+Option+U (via menu) |
| Toggle Flex view | Cmd+F |
| Undo | Cmd+Z |
| Cycle region (loop) | U |
| Zoom to fit | Z |
| Merge regions | Cmd+J |
| Split at playhead | Cmd+T |
