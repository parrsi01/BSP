# Making House Music Beats in FL Studio 20 — Full Tutorial

---

## 1. Project Setup

### BPM and Time Signature
- House music standard: **124–130 BPM**
  - Deep house: 122–124
  - Soulful house: 124–126
  - Tech house: 126–130
- Set in the toolbar tempo field or press **F10** → General → BPM
- Time signature: **4/4** (default, leave it)

### Audio Settings
- **F10 → Audio** tab
- Sample rate: **44100 Hz** (streaming standard) or 48000 Hz (if delivering to video)
- Buffer length: 256 samples for production; 512 if getting CPU crackle
- Output: your audio interface; disable "Allow background processing" to reduce latency

### Project Prep
- Save immediately: **Ctrl+S** → name format `BSP_[BeatName]_[BPM]_[Key]`
- Enable **time markers** in the Playlist for arrangement sections
- Set the **master pitch** to 0 unless you're transposing a loop set

**Keyboard shortcuts to learn now:**

| Action | Shortcut |
|--------|---------|
| Play/Stop | Space |
| Record | R |
| Open Mixer | F9 |
| Open Piano Roll | F7 (on selected pattern) |
| Open Browser | F8 |
| Zoom in Playlist | Ctrl+Scroll |
| Add pattern to Playlist | Middle-click drag |

---

## 2. 808 / Kick Drum Pattern (4-on-the-Floor)

### Loading a Kick
1. Open **Beat+Bassline** (right-click Playlist → Add one, or press **Shift+Ctrl+B**)
2. Right-click the first channel → **Insert** → browse to your kick sample (or use FL's built-in `Kick`)
3. Alternatively drag from the Browser (F8) directly into Beat+Bassline

### 4-on-the-Floor Pattern
In a 16-step Beat+Bassline at 1/4 resolution:
- Hit steps: **1, 5, 9, 13** (every beat)
- This is the defining pulse of house music — never skip it

### Kick Layering Technique
Use 2–3 kick layers for depth:
1. **Sub kick** (20–80 Hz): long transient, felt more than heard — use a 808 sine or Kick plugin set low
2. **Body kick** (80–200 Hz): the punch — classic 909 sample works here
3. **Click/attack** (2–5 kHz): transient snap — a short wood or click sample

**Layer tips:**
- Phase-align layers — zoom into waveform view and nudge so peaks align
- Cut low end (<40 Hz) off body kick, leave it on sub kick
- Side-chain all three layers to the same group in the Mixer

**FL Studio plugins for kick design:**
- **Kick** (native) — great for designing 808-style sub kicks
- **DirectWave** — load your 909 samples here
- **Sytrus** — can synthesize very clean kick transients

---

## 3. Hi-Hat Programming

### Basic Hi-Hat Pattern
In Beat+Bassline, add a closed hi-hat channel:

| Step | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 | 14 | 15 | 16 |
|------|---|---|---|---|---|---|---|---|---|----|----|----|----|----|----|-----|
| Closed HH | X | | X | | X | | X | | X | | X | | X | | X | |
| Open HH | | | | X | | | | X | | | | X | | | | X |

### Ghost Notes
Right-click active steps → **Set velocity** → 50–70% for ghost hits. Add ghost notes on off-steps (2, 4, 6, 10, 14, etc.) for groove.

### Shuffle / Swing
- Click the **"Swing"** knob in the Beat+Bassline channel strip
- House typically uses **20–35% swing** — too much makes it sound like hip-hop
- Alternatively use the **Groove template** (right-click the pattern name)

### Open Hi-Hat Placement
Classic house: open HH on the **off-beats** (steps 5, 13 in 16-step at 1/2 resolution, or 3 and 7 of an 8-step)

**Pro tip:** Layer 2 hi-hat samples (e.g., a bright metallic and a darker one) and pan them slightly opposite (L10, R10) for width without phase issues.

---

## 4. Clap / Snare Placement

### Standard Placement
- Clap/snare hits on beats **2 and 4** — steps 5 and 13 in 16-step
- Layer a **room snare** (for body) + a **rimshot or clap** (for crack)

### Ghost Snares
Add low-velocity hits just before beat 3 (step 9) or scattered around the main hits. Velocity: 30–50%.

### Clap Layering
1. Dry 909 clap (main crack)
2. Reverb-drenched clap (pre-fader send to reverb return)
3. Optional: vinyl-noise snap sample for vintage texture

---

## 5. Bassline Creation

### Using 3xOsc for House Bass
1. Add a **3xOsc** instrument channel in the Beat+Bassline or as a separate pattern in Playlist
2. **OSC1:** Sine wave, center, unison 1
3. **OSC2:** Sine wave, +1 octave, volume 50%, slight detune (+3 cents)
4. In the **Channel settings (F3):** set **FUN** (envelope) — fast attack (0%), sustain 80%, release 200ms

**For a walking bass:** Open the Piano Roll (F7), draw notes following the root of your chord progression. 8th-note movement between roots creates that classic deep house walk.

### Using Sytrus for House Bass
1. Load **Sytrus** → go to **Envelope** tab
2. OP1: Sine wave, Volume 100%, Ratio 1.00
3. Set a fast attack and medium release in the amplitude envelope
4. Add subtle **distortion** (OP1 Distortion knob ~10%) for presence
5. Enable **Mod X** → filter envelope sweep for an acid-adjacent sound (tech house)

**Bass EQ in Mixer:**
- High-pass at 30 Hz (remove rumble)
- Boost around 80–100 Hz for weight
- Cut 200–400 Hz to clean up mud (especially if kick has energy here)
- Side-chain to kick (see Step 9)

---

## 6. Chord Progressions

House music leans on **minor 7th**, **major 7th**, and **suspended** chords.

### Common House Progressions

| Progression | Key feel | Example (Am) |
|------------|----------|-------------|
| i - VI - III - VII | Dark, driving | Am - F - C - G |
| i7 - iv7 | Deep, jazzy | Am7 - Dm7 |
| Imaj7 - IVmaj7 | Bright, soulful | Cmaj7 - Fmaj7 |
| i - VII - VI - VII | Anthemic | Am - G - F - G |
| i - bVII | Minimal, hypnotic | Am - G (loop) |

### Programming Chords in FL Studio
1. Add a pad instrument (e.g., **FL Keys**, **Sytrus**, or **ZGameEditor Visualizer**)
2. Open Piano Roll (F7)
3. Draw chords as **block chords** first, then offset individual notes by 10–30ms for a strummed/human feel
4. Use **Chord mode** in the Piano Roll toolbar (right-click notes to see chord options)

**Pro tip:** Use the **MIDI chord tool** (Piano Roll → Tools → Chord) to auto-generate chord voicings.

---

## 7. Lead Melody Tips

- House leads often sit in the **upper mid range** — play melodies in the C5–C7 range
- Keep it simple: 4–8 note phrases that repeat with subtle variation
- Common technique: **call and response** — play a 2-bar phrase, leave 2 bars of space
- Use **portamento** (pitch glide) on leads for a vocal/analog feel — set in Channel Settings (F3) under Porta
- Velocity variation: 70% notes on beats, 50–60% on off-beats, 90% on accented notes

---

## 8. Sample Chops (Vocal Samples)

### Chopping a Vocal in Edison
1. Load your vocal sample into **Edison** (drag sample to mixer insert → click Edison icon)
2. Press **E** in Edison → **Detect regions** (auto-detects transients)
3. Manually adjust region markers by dragging
4. Right-click each region → **Send to Piano Roll as sample**

### Chopping in the Sampler Channel
1. Drag vocal WAV to a **Sampler channel** in the Beat+Bassline
2. Open the Channel Settings (click channel name)
3. Use **Start/End** knobs to isolate a chop
4. Press notes in Piano Roll to play different start points

### Pitch-Shifting Chops
- In Sampler channel: **Pitch** knob shifts by semitones
- For melodic chops: map chops across keys and play a melody in Piano Roll
- Add **formant shifting** using **NewTone** plugin for natural pitch shifts without chipmunk effect

---

## 9. Mixing in the Mixer

### Routing
- Right-click each instrument channel → **Set mixer track** (or press Ctrl+L to auto-link)
- Create groups: Drums Bus, Bass Bus, Synths Bus, FX Bus → route to Master

### EQ (Parametric EQ 2)
**Quick house EQ cheat sheet:**

| Element | Cut | Boost |
|---------|-----|-------|
| Kick | <30 Hz, 200–400 Hz (if muddy) | 60–80 Hz (sub), 3–5 kHz (attack) |
| Bass | <40 Hz, 400–600 Hz | 80–120 Hz |
| Clap/Snare | <100 Hz | 2–4 kHz (crack), 8–12 kHz (air) |
| Hi-Hats | <800 Hz | 10–14 kHz (shimmer) |
| Pads/Chords | <200 Hz (wide cut) | Midrange presence if needed |
| Lead | <300 Hz | Presence 2–4 kHz |

### Compression (Fruity Peak Controller + Parametric)
For individual elements: **Fruity Peak Controller** as a sidechain trigger.

### Sidechain Compression (The Pump Effect)
1. Route your **kick** to Mixer Track 1
2. Route **bass** to Mixer Track 2
3. On the bass track, click the send knob from Track 1 → Track 2 (send = side-chain trigger)
4. Add **Fruity Peak Controller** on Track 1 as a peak control
5. Link Peak Controller output to the **volume knob of Track 2**
6. Set the Peak Controller: **Attack ~0ms, Release ~300–500ms, Base = 50%, Volume = 100%**

**Alternative (faster method):**
- On the bass track → add **Parametric EQ 2** or a volume automation clip
- Draw a volume dip automation that ducks on every kick hit (Ctrl+L in the Playlist → draw beats)

---

## 10. Arrangement

### House Music Structure

| Section | Length | Description |
|---------|--------|-------------|
| Intro | 16–32 bars | Drums only, minimal elements, DJ-friendly |
| Build | 8–16 bars | Add elements gradually; tension builds |
| Drop 1 | 32–64 bars | Full arrangement; main hook/bass |
| Breakdown | 16–32 bars | Strip back; often chord-only or vocal |
| Build 2 | 8–16 bars | Re-tension; filter sweep, cymbal roll |
| Drop 2 | 32–64 bars | Full energy returns, possibly with variation |
| Outro | 16–32 bars | Strip elements back; DJ-friendly exit |

### Building the Arrangement in Playlist
1. Use **Ctrl+M** to open the Playlist
2. Drag patterns from the left panel into time blocks
3. Use **color coding**: drums = red, bass = blue, synths = green, FX = yellow
4. Create **automation clips** (right-click knob → Create automation clip) for filter sweeps, volume builds

### DJ-Friendly Tips
- Intro and outro should be **drums-only or minimal** — at least 8 bars before any melody
- Total track length: **5–7 minutes** for DJ use; **3–4 minutes** for streaming
- Include a **loop point** at the main groove section (mark with time markers)

---

## 11. Mastering Basics in FL Studio

### Master Chain (on the Master Mixer Track)
1. **Parametric EQ 2** — gentle high-shelf boost (10 kHz, +1–2 dB); cut below 30 Hz
2. **Maximus** (multiband comp/limiter) — use the "Mastering" preset as a starting point; keep ceiling at -0.3 dB
3. **Fruity Peak Controller** — not needed at master; leave Maximus as final stage

### Loudness Targets

| Platform | LUFS Target | True Peak |
|----------|------------|----------|
| Spotify / Apple Music | -14 LUFS | -1 dBTP |
| YouTube | -14 LUFS | -1 dBTP |
| BeatStars (watermarked MP3) | -8 to -10 LUFS | -0.3 dBTP |
| Beatport / DJ use | -8 to -10 LUFS | -0.3 dBTP |

Use **Fruity Loudness Meter** on the Master to check LUFS.

---

## 12. Export Settings for Beat Selling

### Exporting the Main Beat (Tagged MP3)
- **File → Export → MP3**
- Bit rate: **320 kbps**
- Add your **beat tag/watermark** at the 30-second mark (route your tag audio as an automation event or bake it in before export)
- Filename: `BSP_BeatName_BPM_Key_TAGGED.mp3`

### Exporting WAV (High Quality / Lease)
- **File → Export → WAV**
- Bit depth: **24-bit**
- Sample rate: **44100 Hz**
- Filename: `BSP_BeatName_BPM_Key_MASTER.wav`

### Exporting Stems (Exclusive / Unlimited License)
1. Solo each bus group (Drums, Bass, Chords, Lead, FX)
2. Export WAV for each group
3. File naming: `BSP_BeatName_BPM_Key_STEM_Drums.wav`, etc.
4. Deliver stems in a ZIP with the license document

### Project Archive (for collaboration)
- **File → Export → Zipped loop package** — includes all samples the project references
- Always do this before handing a project to a teammate
