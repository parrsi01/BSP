# House Music Sound Design — Deep Dive

---

## Classic House Kick Drum: Layering a 909 with Sub Bass

The house kick is built, not just sampled. Even when starting with a 909 sample, layering is what gives it professional weight and presence.

### The Three-Layer Kick Stack

| Layer | Frequency Range | Role | Source |
|-------|----------------|------|--------|
| Sub layer | 20–80 Hz | Low-end weight, felt in clubs | Sine wave synth or 808 sub |
| Body layer | 80–200 Hz | The "thump" and punch | 909 kick sample |
| Click/attack | 2–8 kHz | Transient definition, audible on small speakers | Short click, wood block, or noise burst |

### Building the Sub Layer
Using a synth (Sytrus, ES2, Serum, or Vital):
1. Oscillator: pure **sine wave**
2. Pitch envelope: start at **180–250 Hz**, fall rapidly to **40–50 Hz** over 80ms
3. Amp envelope: fast attack (0ms), medium decay (100–150ms), sustain 0%
4. The pitch drop is what gives the 808 kick its character

### Processing the Body (909 Sample)
1. Load 909 kick WAV in a sampler
2. **High-pass filter:** cut below 50–60 Hz (the sub layer handles this range)
3. **Transient shaper:** increase attack presence; reduce sustain if it's too "boomy"
4. **Saturation:** subtle tape saturation to add harmonic content

### Click Layer
- A very short (30–50ms) transient sample or noise burst
- High-pass filter at 1.5 kHz — only the click energy remains
- Volume: 10–20% relative to body — subtle, but critical for small speaker definition

### Phase Alignment
All three layers must fire simultaneously. In your DAW:
- Zoom into the waveform (sample level)
- Ensure all three waveforms begin at the same point in time
- Watch for phase cancellation: if combined kick sounds thinner than individual layers, invert phase on one layer

---

## Deep House vs Tech House vs Afro House — Differences

| Element | Deep House | Tech House | Afro House |
|---------|-----------|-----------|-----------|
| BPM | 120–124 | 126–132 | 118–124 |
| Kick | Warm, soft attack, sub-heavy | Punchy, clicky, less sub | Organic, drum-like attack |
| Hi-hats | Swung, laid-back | Tight, mechanical, triplet patterns | Complex polyrhythm, shakers |
| Bass | Walking sub bass, melodic | Minimal, repetitive, driven | Melodic bass with swing |
| Chords | Lush 7th chords, jazz harmony | Minimal stabs, less chord-heavy | World-music harmony, pentatonic |
| FX | Warm reverb, subtle delay | Dry, distorted, industrial | Percussive, ethnic instruments |
| Vocal | Full vocal hooks, gospel influence | Short chops, minimally processed | Chants, polyrhythmic vocals |
| Reference artists | Larry Heard, Kerri Chandler | Chris Lake, Fisher, James Hype | Black Coffee, Enoo Napa, Themba |

---

## Vocal Sample Processing

### Step 1: Clean the Source
- **High-pass filter** at 80–100 Hz to remove room rumble
- **De-ess** if there are harsh sibilants (use stock de-esser at 6–9 kHz)
- **Noise gate** to eliminate breath noise between phrases

### Step 2: Chop
- Slice at transients (word boundaries, syllable hits)
- Select the most musical fragments: vowel sounds, breaths, exclamations ("yeah", "oh", "hey")
- Keep chops short: 1/8th to 1/4 bar for stabs; longer (1–2 bars) for hooks

### Step 3: Pitch Shifting
- Map chops across a MIDI keyboard — different notes play different pitches of the same chop
- Use **Formant preservation** (Ableton Complex Pro, Logic's Flex Pitch, or Melodyne) to avoid chipmunk effect
- Classic house vocal: transpose vocal sample up 3–5 semitones for a soulful, bright sound

### Step 4: Reverse Samples
- Take a vocal chop → reverse it → place it just before a beat hit
- Creates a "rising into" the beat effect — classic house production trick
- Also works with claps, pads, and snares

### Step 5: FX Processing Chain for Vocals
```
Source → EQ (clean) → Pitch Shift → Reverb Send → Delay Send → Saturation → Output
```
- **Reverb:** Plate or room reverb, pre-delay 20–30ms, decay 1–2s, wet 25–40%
- **Delay:** 1/8th note sync, feedback 20–30%, high-pass the delay return at 500 Hz

---

## Pad Sound Design: Lush Chords with Reverb Tails

### The Foundation Pad
Goal: warm, evolving chords that fill space without competing with the bass or kick.

**In Serum (or Vital):**
1. OSC A: **Analog BD8** or any analog-modeled table, Position 30%, Unison 4 voices, Detune 15 cents
2. OSC B: **Hollow** wavetable, opposite phase (+180°), level -6dB
3. **Filter:** Low-pass, Cutoff 2.5 kHz, Resonance 10%, slight envelope modulation (amount +10%)
4. **Envelope 1 (Amp):** Attack 400ms, Hold 0, Decay 2s, Sustain 70%, Release 3s
5. **LFO 1 → Cutoff:** Rate 0.08 Hz (very slow), Amount ±15% — subtle breathing animation

### Layering the Pad
Two synth layers create depth:
- Layer 1: Wavetable pad (as above), panned center
- Layer 2: Simple FM pad with sine oscillators, panned slightly left-right (±15%)

### Reverb for Pads
- Reverb type: **Hall** or **Large Room** (Space Designer, Valhalla Room, or FabFilter Pro-R)
- Pre-delay: **0ms** for pads (no gap — let the reverb bloom with the note)
- Decay: **3–6 seconds** — house pads breathe and sustain
- High-pass reverb return at 200 Hz (prevent mud building up in reverb tail)

---

## Bass Design: Deep Sub vs Walking Bass vs Acid Bass (303-style)

### Deep Sub Bass
Purpose: felt in the body, heard on subwoofers. Minimal harmonic content.
- **Oscillator:** Sine wave only (no overtones)
- **Filter:** Low-pass at 150 Hz — tight, controlled
- **Envelope:** Fast attack, medium-long release (400ms)
- **Processing:** Side-chain to kick, very subtle saturation only

### Walking Bass (Deep House)
Purpose: melodic movement between notes, creates groove and musicality.
- **Oscillator:** Sine + slight triangle (adds warmth without brightness)
- **Portamento:** 20–50ms glide time between notes
- **Pattern:** Root on beat 1, walk up/down on beats 3-and or 4-and
- **EQ:** Presence boost at 200–400 Hz so the walk is audible on standard speakers

### Acid Bass (303-Style, Tech House)
Purpose: hypnotic, resonant, driving line — a hallmark of tech house and early rave.
- **Oscillator:** Sawtooth wave (full harmonic content)
- **Filter:** Resonant low-pass, Resonance 60–80%
- **Envelope (filter):** High attack-decay modulation — this is the "acid" sound
- **Sequence:** Repetitive, often using the same note with accent and slide variations
- **Dedicated synth options:** TAL BassLine-101 (free), Monsta (by Xfer), or Serum in mono mode

---

## Percussion Layering for Groove

### The Percussion Stack (Beyond Kick/Clap/HH)

| Element | Sound | Rhythmic Placement |
|---------|-------|-------------------|
| Conga / bongo | Mid-range organic hit | Off-beats, syncopated |
| Shaker | White-noise rattle | 16th-note pattern, adds momentum |
| Cowbell | Mid-high metallic | On 3-and or 4-and |
| Rimshot | Dry crack | Ghost beats between snare hits |
| Tambourine | High, jangly | 8th-note emphasis |
| Wood block | Short, dry click | Syncopated positions |
| Clap layer | Reversed clap | Just before main clap hit |

### Groove Through Velocity
- Lead percussion: 90–100% velocity
- Supporting percussion: 60–75%
- Ghost/texture hits: 30–50%
- Velocity variation between identical hits: ±10% to humanize

### Polyrhythm in Afro House
- Layer a **3-against-4** conga pattern over the standard 4/4 drums
- Conga hits at: 1, 1.2.2, 1.3.3, 2.1.1, 2.2.2, 2.3.3 (every 3rd 16th note)
- This creates tension and forward momentum — the Afro house signature

---

## White Noise Sweeps and Risers

### Building a Noise Riser from Scratch
1. Create a white noise source (any synth noise oscillator, or a recorded noise WAV)
2. Apply a **high-pass filter** — automate the cutoff from 20 Hz → 16 kHz over 8 bars
3. Apply volume automation: start at -∞ dB, arrive at 0 dB on the last beat
4. Add subtle reverb (large hall, long decay) — lets it breathe and anticipate the drop
5. Optional: add a **pitch rise** (automate pitch of the noise +1 octave over 4 bars)

### Cymbal Roll Build
1. Take a cymbal or hi-hat loop
2. Increase the playback speed gradually (Flex time, pitch-independent) over 4–8 bars
3. Or: layer increasing numbers of hi-hat hits (from 1/4 → 1/8 → 1/16 → 1/32) in the last 2 bars
4. Add reverb wet amount automation: ramp from 20% to 80% wet going into the drop

### Common Riser Types

| Riser | Sound | Length | Placement |
|-------|-------|--------|-----------|
| Noise sweep | White noise HPF sweep | 4–8 bars | Before main drop |
| Cymbal roll | Accelerating hi-hat | 2–4 bars | Last section of build |
| Synth riser | Pitch-rising pad or sine | 2–4 bars | Layered with noise |
| Vocal rise | Pitched vocal chop scaling up | 1–2 bars | Dramatic effect |
| FX hit | Downward crash at drop | Instant | Drop point |

---

## FX Chain Order for House: Reverb → Delay → Saturation

### Why This Order Matters

**Reverb first:** the reverb gives natural space, as if the sound is in a room.
**Delay after reverb:** the delay echoes the already-reverbed signal — sounds natural and wide.
**Saturation last:** adds harmonics and "warmth" to the processed signal, gluing everything together.

### Full Insert Chain for a House Pad

```
Pad Source
  → EQ (remove low-end mud, shape high mids)
  → Chorus / Ensemble (width and animation)
  → Reverb (Room or Plate, 20–40% wet)
  → Delay (1/8 note sync, 15–25% wet)
  → Saturation (Tape mode, 5–15% drive)
  → EQ (final tone shaping, air boost at 12kHz)
  → Compressor (gentle glue, 2–3 dB GR)
```

### Send/Return vs Insert for Reverb and Delay
- **Send/Return** (preferred): one shared reverb and delay instance services multiple tracks — saves CPU and creates cohesion (all elements sound like they're in the same space)
- **Insert**: use on individual elements that need unique treatment (kick — no reverb; vocal chop — dedicated plate reverb)

---

## Reference Tracks for A/B Mixing

See [resources/REFERENCE_TRACKS.md](../resources/REFERENCE_TRACKS.md) for a full categorized list.

**Quick reference by use case:**

| What to Study | Track | Artist |
|--------------|-------|--------|
| Sub kick weight | "I Need Your Lovin'" | DJ Duke |
| Sidechain pump | "Show Me Love" | Robin S (club mix) |
| Pad depth | "Can You Feel It" | Mr. Fingers |
| Vocal chop technique | "Music Sounds Better With You" | Stardust |
| Tech house groove | "Cola" | CamelPhat & Elderbrook |
| Afro house percussion | "Superman" | Black Coffee |
