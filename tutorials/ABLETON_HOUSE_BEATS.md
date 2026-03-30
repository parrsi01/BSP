# Making House Music Beats in Ableton Live — Full Tutorial

---

## 1. Project Setup and Preferences

### Audio Preferences
- **Ableton → Preferences → Audio** (Mac: Cmd+, / Win: Ctrl+,)
- Driver: ASIO (Windows) or Core Audio (Mac)
- Sample rate: **44100 Hz** (44.1 kHz) for music delivery; 48000 Hz if working with video
- Buffer size: **256 samples** for production; drop to 128 for low-latency recording; raise to 512 if CPU spikes
- Check "Input Config" and "Output Config" to enable your interface channels

### Project Template
- Set BPM: **126 BPM** (good starting point; range 124–130 for house)
- Set time signature: **4/4**
- Save as a template: **File → Save As Default Set** so every new project starts configured

### Recommended File Structure
Inside Ableton's User Library, create folders:
```
User Library/
├── Beats/
│   ├── Drum Racks/
│   ├── MIDI Clips/
│   └── Templates/
├── Samples/
│   └── House/
└── Presets/
```

---

## 2. Session View vs Arrangement View — When to Use Each

| View | Shortcut | Use For |
|------|---------|---------|
| Session View | Tab | Sketching ideas, jamming, testing loops, live performance |
| Arrangement View | Tab (toggle) | Full song arrangement, automation, stem export |

### Recommended House Workflow
1. **Start in Session View:** Build loops (drum rack, bass, chords) and jam them together
2. Once your groove feels right, **record into Arrangement View** (global record: F9 in Arrangement + play clips in Session)
3. Refine structure, add automation, and finalize in Arrangement View

---

## 3. Drum Rack Setup for House

### Creating the Drum Rack
1. **Cmd/Ctrl+Shift+B** → Instruments → Drum Rack → drag to a MIDI track
2. Or drag any sample directly to a Drum Rack pad

### House Drum Rack Layout (Standard Mapping)

| Pad | MIDI Note | Element | Sample Type |
|-----|----------|---------|------------|
| C1 | 36 | Kick | 909/808 kick WAV |
| D1 | 38 | Snare/Clap | 909 clap or snare |
| F#1 | 42 | Closed HH | Metallic closed HH |
| A#1 | 46 | Open HH | Open hat |
| C#1 | 37 | Rimshot/Ghost | Low-velocity ghost |
| D#1 | 39 | Hand clap | Layered with snare |
| A1 | 45 | Percussion 1 | Shaker or conga |
| B1 | 47 | Percussion 2 | Cowbell or rim |

### Layering in the Drum Rack
- Each pad has a **chain** — you can stack multiple samples on one pad
- Click the pad → expand chain view → drag a second sample
- Use the **chain volume** to blend layers
- For kick layering: pad 1 = sub kick (sine-ish), pad 1 chain 2 = 909 body, pad 1 chain 3 = click/snap

### Macro Controls
- Drum Rack has 8 macro knobs — map kick volume, hi-hat pitch, and swing amount here for quick tweaks during a session

---

## 4. MIDI Programming House Patterns

### Drawing in Clips (Arrangement View)
- Double-click an empty clip slot → opens MIDI editor
- Draw mode: **B** key or pencil icon
- Select mode: **Ctrl/Cmd** to switch

### 4-on-the-Floor Kick Pattern
In a 1-bar MIDI clip at 1/16 resolution:
- Draw kick notes at positions: **1.1.1, 1.2.1, 1.3.1, 1.4.1**

### Hi-Hat Pattern (classic 8th note house)
- Closed HH: every **1/8th note** (positions 1.1.1, 1.1.3, 1.2.1, 1.2.3, etc.)
- Open HH: on the **off-beat 1/8th** (positions 1.1.3 and 1.3.3 for emphasis)

### Clap/Snare Pattern
- Clap on beats **2 and 4** (positions 1.2.1 and 1.4.1)

### Ghost Notes
- Draw low-velocity hits (velocity 30–60) around the main snare
- Velocity editor: click the triangle at the bottom of the MIDI clip to show velocity bars
- Drag individual velocity bars down for ghost hits

---

## 5. Bass Creation with Wavetable or Analog

### Using Wavetable for House Bass
1. Insert **Wavetable** instrument on a MIDI track
2. **Oscillator 1:** Sine or Triangle wave
3. **Filter:** Set to Low-Pass, Cutoff ~700 Hz, Resonance ~20%
4. **Envelope:** Fast attack (0–1ms), sustain ~80%, release 200–400ms
5. For deeper sub: reduce the filter cutoff and boost the Osc level

**House bass in Wavetable — specific settings:**
- OSC 1 Position: 0 (pure sine)
- Filter: LA Multi 12dB, Cutoff 500 Hz
- Amp Envelope: A=0, D=200ms, S=70%, R=300ms
- Add **Redux** device for subtle saturation/bit crush on the bass channel

### Using Analog for Walking Bass
1. Insert **Analog** instrument
2. OSC1: Saw wave (for more harmonic content)
3. Filter 1: Low-pass, Cutoff ~800 Hz
4. Use Glide (in the Analog settings) for smooth pitch slides between notes

### MIDI for Bass
- Draw root notes in piano roll following your chord progression
- For walking bass: add passing notes (half-step or whole-step) between roots
- 8th-note rhythm is standard; try syncopated patterns (notes slightly before the beat) for groove

---

## 6. Using Simpler / Sampler for Vocal Chops

### Loading a Vocal in Simpler
1. Drag a vocal WAV to a MIDI track → Simpler loads automatically
2. In Simpler, set **Mode to Classic**
3. Use **Start** and **End** markers to isolate a section
4. Map to a key in your MIDI clip to play the chop at different pitches

### Chopping with Simpler (multiple chops)
1. Set Simpler to **Slice mode** (mode selector top-right)
2. Adjust the **sensitivity** slider — Simpler auto-slices on transients
3. Each slice maps to a pad — trigger them from MIDI

### For Multiple Independent Chops: Use Sampler
1. Drag vocal to **Sampler** instrument
2. In the **Zones** tab, create multiple zones per key with different start/end points
3. Now each MIDI note plays a different chop

### Pitch Shifting Without Artifacts
- In Simpler: go to the **Warp** tab → **Complex Pro** mode
- Adjust **Formants** knob to avoid chipmunk effect when transposing up

---

## 7. Chord Stabs and Pads with Wavetable

### Pad Sound in Wavetable
1. Load Wavetable → OSC1: Morphing to a "Vocal" or "Pad" wavetable
2. Set the **Position** macro to 30–50% into the table for a lush, evolving sound
3. Filter: 12dB LP, Cutoff ~2 kHz, slight resonance
4. Amp Envelope: slow attack (200–500ms), long release (1–2 sec)
5. Reverb: use a **Reverb** device after Wavetable; Size 80%, Dry/Wet 40%

### House Chord Stab
1. Shorter attack (10–30ms) for a "stab" feel
2. Short decay, no sustain — like a stabbed chord
3. Add a small amount of **chorus** or **ensemble** for width

### Voicing Chords for House
Use **upper structure voicings** — spread notes across 2 octaves:
- Minor 7: root, flat-7, flat-3, 5th (example Am7: A2, G3, C4, E4)
- Major 7: root, major-7, 3rd, 5th

Draw the chord once in MIDI, then copy blocks — house music repeats extensively.

---

## 8. Groove and Swing Settings

### Applying Groove
- Select a MIDI clip or audio clip → **Clip Properties** panel → **Groove** dropdown
- Recommended grooves: **MPC Swing 16** or **Akai MPC 16 Swing** templates
- **Swing amount:** 5–20% for house (controlled by the Global Groove knob in the transport bar)

### Per-Clip Groove
- Right-click a clip → **Groove** → select a template
- Each clip can have a different groove amount — use this to make drums feel slightly more human than pads

### Nudging Individual Notes
- In the MIDI editor, select a note and nudge with arrow keys
- Shift+arrow for larger nudges
- Nudge hi-hats and percussion slightly behind the grid (+5 to +10ms) for a "laid back" house feel

---

## 9. Sidechain Compression (Glue Compressor Technique)

The pumping sidechain effect is central to house music energy.

### Method 1: Glue Compressor Sidechain
1. Place your **kick** on Track 1
2. Place your **bass** (or pads) on Track 2
3. On Track 2, add a **Glue Compressor**
4. In the Glue Compressor, click **Sidechain** tab → enable **External Sidechain**
5. Set the **Audio From** dropdown to Track 1 (Kick)
6. Set: **Threshold -20dB, Ratio 4:1, Attack 0.01ms, Release 150–300ms**
7. The compressor now ducks every time the kick hits

### Method 2: Volume Automation
1. On the bass or pad track, **right-click the volume knob** → Create automation lane
2. Draw volume dips that align exactly with your kick hits
3. Faster and more precise; sounds less natural but very controllable

### Settings for the Classic House Pump

| Parameter | Value |
|-----------|-------|
| Threshold | -18 to -25 dB |
| Ratio | 4:1 to 8:1 |
| Attack | 0.1–1 ms |
| Release | 150–400 ms (match the kick decay) |
| Make-up gain | +2 to +4 dB |

---

## 10. Automation for DJ-Friendly Builds

### Creating a Filter Sweep Build
1. On your pad or full synth bus track, add **Auto Filter**
2. In Arrangement View, right-click the Auto Filter Frequency knob → **Show Automation**
3. Draw a rising line from ~200 Hz (at the start of the build) to ~8000 Hz (at the drop)
4. Use **curve handles** (drag midpoint of automation line) to make it exponential — more dramatic

### Cymbal Roll Build
1. Create a new audio or MIDI track with a cymbal loop
2. Automate the **volume** or a **reverb wet/dry** to increase into the drop
3. Classic: use a white noise sample with rising volume automation over 8 bars before the drop

### High-Pass Filter Build (stripping the track)
1. Put an **EQ Eight** on the Master (or a stem bus)
2. Enable band 1 (high-pass filter) in Automation view
3. Draw automation: start at ~300 Hz (cutting the low end during breakdown) → cut to 30 Hz (releasing at the drop)

---

## 11. Clip Launching for Live Performance

### Session View Setup
- Organize clips by **scene** (rows): Scene 1 = Intro, Scene 2 = Groove A, Scene 3 = Build, Scene 4 = Drop
- Each scene contains matching clip lengths (all 4 or 8 bars)
- Press **Enter/Return** on a scene to launch all clips simultaneously

### MIDI Mapping for Performance
- **Cmd/Ctrl+M** → MIDI Map mode
- Click a clip slot, then press a key on your controller → mapped
- Map the **Launch** button, **Stop All Clips**, and **Scene launchers** to your controller

### Quantization
- Set **Global Launch Quantization** (top of screen) to **4 Bars** so clips wait for the right bar to launch — prevents off-beat triggers during live sets

---

## 12. Stems Export and Delivery Formats

### Exporting Stems
1. **File → Export Audio/Video** (Cmd/Ctrl+Shift+R)
2. Render each bus separately: solo a track group → export → unsolo → next
3. Or use **Render track to new audio** for each bus

### Export Settings

| Setting | Value |
|---------|-------|
| File Type | WAV |
| Bit Depth | 24-bit |
| Sample Rate | 44100 Hz |
| Normalize | Off (preserve gain staging) |
| Create Analysis Files | Off (not needed for delivery) |

### Stem Naming Convention
```
BSP_BeatName_BPM_Key_STEM_Kick.wav
BSP_BeatName_BPM_Key_STEM_Bass.wav
BSP_BeatName_BPM_Key_STEM_Chords.wav
BSP_BeatName_BPM_Key_STEM_Lead.wav
BSP_BeatName_BPM_Key_STEM_Perc.wav
BSP_BeatName_BPM_Key_STEM_FX.wav
BSP_BeatName_BPM_Key_MASTER.wav
```

### Tagged MP3 for BeatStars/Airbit
1. Bounce the full beat with your tag as MP3: **Cmd/Ctrl+Shift+R** → MP3 320kbps
2. Insert your beat tag as an audio track that plays at the 30-second mark
3. Export: `BSP_BeatName_BPM_Key_TAGGED.mp3`
