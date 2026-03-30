# Mixing and Mastering Guide for House Beats

---

## Gain Staging Workflow

Proper gain staging prevents noise floor buildup and distortion before any processing happens.

### Target Levels Before Processing

| Stage | Target Level |
|-------|-------------|
| Individual instrument outputs | -18 to -12 dBFS (peaks) |
| Bus/group outputs | -10 to -6 dBFS |
| Pre-master bus | -6 to -3 dBFS |
| Master output (before limiter) | -6 dBFS |

### How to Gain Stage
1. Start with all faders at 0 dB
2. Play your loudest section (the drop)
3. Set each instrument's **output gain** (before the fader) so peaks hit -18 dBFS
4. Use fader to blend the mix — now you have headroom for dynamics processing
5. The master fader should never clip before mastering

**Rule:** Never compensate for gain staging with a compressor or limiter early in the chain.

---

## EQ Cheat Sheet for House Elements

### Kick Drum

| Band | Frequency | Action | Reason |
|------|-----------|--------|--------|
| HPF | 20–30 Hz | Cut | Inaudible sub-rumble wasting headroom |
| Sub | 60–80 Hz | Boost (+2–4 dB) | Weight and felt low-end |
| Mud | 200–400 Hz | Cut (-3 to -6 dB) | Clean up muddiness |
| Snap | 3–6 kHz | Boost (+2–3 dB) | Transient click for small speakers |

### Bass (Sub / Walking)

| Band | Frequency | Action | Reason |
|------|-----------|--------|--------|
| HPF | 30–40 Hz | Cut | Sub rumble |
| Fundamental | 80–120 Hz | Boost (+1–3 dB) | Core bass tone |
| Mud | 250–400 Hz | Cut (-4 to -8 dB) | Remove mud competing with kick body |
| Presence | 1–2 kHz | Boost (+2 dB) | Bass audible on laptop speakers |

### Hi-Hats

| Band | Frequency | Action | Reason |
|------|-----------|--------|--------|
| HPF | 600–1000 Hz | Cut | Remove low-mid rumble |
| Air | 10–16 kHz | Boost (+1–2 dB) | Shimmer and presence |
| Harshness | 6–8 kHz | Cut if needed | Reduce ear fatigue |

### Clap / Snare

| Band | Frequency | Action | Reason |
|------|-----------|--------|--------|
| HPF | 80–120 Hz | Cut | Remove low-end (kick's territory) |
| Body | 200–400 Hz | Boost or cut to taste | Snare body |
| Crack | 2–4 kHz | Boost (+2–4 dB) | Attack and snap |
| Air | 8–12 kHz | Boost (+1–2 dB) | Brightness |

### Pads / Chords

| Band | Frequency | Action | Reason |
|------|-----------|--------|--------|
| HPF | 150–300 Hz | Cut | Leave low-end to bass and kick |
| Mud | 300–600 Hz | Cut (-2 to -4 dB) | Clarity in the mix |
| Presence | 2–4 kHz | Boost slightly | Cut through the mix |
| Air | 10–16 kHz | Boost (+1–2 dB) | Sparkle and width |

### Lead Melody

| Band | Frequency | Action | Reason |
|------|-----------|--------|--------|
| HPF | 250–400 Hz | Cut | Remove low-mid buildup |
| Presence | 2–5 kHz | Boost (+2–4 dB) | Lead sits above other elements |
| Air | 10–14 kHz | Boost if needed | Brightness |

---

## Compression Settings Per Element

### Kick Drum
- **Ratio:** 4:1 to 6:1
- **Attack:** 5–15ms (slow enough to let transient through)
- **Release:** 80–150ms (match kick decay)
- **GR (Gain Reduction):** 3–6 dB
- **Purpose:** Tighten the tail, add punch consistency

### Bass
- **Ratio:** 3:1 to 5:1
- **Attack:** 10–30ms (slightly slow — preserve note attack)
- **Release:** 100–200ms
- **GR:** 4–8 dB
- **Purpose:** Control dynamics for a consistent, polished bass

### Clap / Snare
- **Ratio:** 4:1 to 8:1
- **Attack:** 0.5–3ms (fast — catch the transient)
- **Release:** 50–100ms
- **GR:** 4–8 dB

### Pads
- **Ratio:** 2:1 to 4:1
- **Attack:** 50–100ms (slow — let pad attack breathe)
- **Release:** 300–600ms
- **GR:** 1–4 dB
- **Purpose:** Light glue, control peaks

### Drum Bus (the whole drum mix)
- **Ratio:** 2:1
- **Attack:** 30ms
- **Release:** Auto
- **GR:** 2–4 dB
- **Purpose:** Glue the kit together, make it sound like one unit

---

## Sidechain Compression — The House Music Pump Effect

This is the defining characteristic of house music. The bass (and often pads) ducks every time the kick hits.

### What It Does
The kick drum signal is used as a "trigger" that tells the compressor on the bass channel to reduce its volume. The result: the bass dips in volume on each kick hit, then rises back up. This creates the pumping, breathing feel.

### Method 1: Dedicated Compressor with Sidechain Input

**Ableton:**
1. Insert **Compressor** on the bass track
2. Expand the compressor → enable **Sidechain** → set Input to the kick track
3. Threshold: -20 dB, Ratio: 8:1, Attack: 0.5ms, Release: 200ms

**FL Studio:**
1. Insert **Fruity Peak Controller** on the kick's Mixer track
2. Link it to the Volume knob of the bass Mixer track
3. Set base = 50%, volume = 100%, attack/release to taste

**Logic Pro:**
1. Create a side-chain from the kick to a compressor on the bass track
2. In the compressor plugin, set the **Side Chain** drop-down to the kick's track

### Method 2: LFO-Based Volume Pump (Predictable and Tight)
When your kick is always on the beat (4-on-the-floor), you can simulate sidechain with an LFO:
- Synced LFO → volume modulation, 1/4 note rate, sawtooth (falling) shape
- This creates a perfectly consistent pump regardless of kick volume variations
- Use this on pads; it gives a very electronic, machine-like pump sound

### Sidechain Settings for Different Effects

| Effect | Threshold | Ratio | Attack | Release |
|--------|-----------|-------|--------|---------|
| Subtle groove | -15 dB | 3:1 | 5ms | 300ms |
| Classic house pump | -20 dB | 6:1 | 0.5ms | 200ms |
| Hard pumping | -25 dB | 10:1 | 0.1ms | 150ms |
| DJ tool (aggressive) | -30 dB | 20:1 | 0.1ms | 100ms |

---

## Stereo Width: What to Keep Mono vs Wide

### Keep Mono (0–200 Hz)
Everything below 200 Hz should be **mono**. This ensures:
- Compatibility with mono club systems
- No phase cancellation when summed to mono
- Bass translation across all playback systems

**How to mono the low end:** Use a **Multiband Mid-Side EQ** or a plugin like **ISOL8** (free) or **Brainworx bx_solo** to check low-end mono.

### Width Guide by Element

| Element | Mono/Stereo | Notes |
|---------|------------|-------|
| Kick | Mono | Always |
| Bass | Mono | Full spectrum mono |
| Clap (main hit) | Mono or narrow | Wide clap reverb is OK |
| Pads/Chords | Wide | Use stereo widener on mid-high content |
| Lead | Slightly wide | Don't over-widen or it'll lose focus |
| Reverb returns | Wide | This is where width should live |
| Hi-hats | Slightly offset | Pan L and R hi-hats ±10–20% |

### Checking Mono Compatibility
In your DAW, use a **mono toggle** on the master:
- If bass drops out → there's phase cancellation, check bass tracks
- If mix sounds significantly worse in mono → pads/leads are over-widened

---

## Reverb and Delay Sends

### Recommended Send Bus Setup

| Bus | Type | Settings | What to Send |
|-----|------|---------|-------------|
| Short Room | Reverb (0.5–0.8s) | Small room preset | Drums (snare, clap) |
| Plate | Reverb (1–2s) | Plate preset | Vocals, leads |
| Large Hall | Reverb (3–5s) | Hall preset | Pads, atmospheric elements |
| Delay | 1/8 or 1/4 note sync | 20–30% feedback | Leads, vocals, FX |

### Rules
- Always **high-pass** your reverb return at 150–250 Hz to prevent low-end mud
- Always **high-pass** the delay return at 300 Hz for clarity
- Keep drum reverb subtle in house music — tight and punchy, not washy

---

## Loudness Targets

| Platform | Integrated LUFS | True Peak Max | Notes |
|----------|----------------|-------------|-------|
| Spotify | -14 LUFS | -1 dBTP | Normalizes louder tracks down |
| Apple Music | -16 LUFS | -1 dBTP | More conservative normalization |
| YouTube | -14 LUFS | -1 dBTP | Volume normalized |
| Tidal | -14 LUFS | -1 dBTP | |
| BeatStars (MP3 preview) | -8 to -10 LUFS | -0.3 dBTP | Competitive loudness for beat store |
| Beatport / DJ use | -8 to -10 LUFS | -0.3 dBTP | DJs want loud, hot masters |
| Stems (WAV delivery) | -14 to -18 LUFS | -1 dBTP | Leave headroom for artist's mix |

**For house music producers:** Master your beat at **-8 to -10 LUFS** for BeatStars/DJ use. This is louder than streaming targets but expected in the beat store context.

---

## Mastering Chain

```
Mix Bus
  1. EQ (Broad, transparent) — shape overall tone
  2. Multiband Compressor — control frequency dynamics
  3. Stereo Widener (mid-side) — subtle width enhancement
  4. Limiter — ceiling at -0.3 dBTP
  5. Clipper (optional) — soft clip before limiter for loudness
  6. LUFS Meter — verify target loudness
```

### Step-by-Step

**1. EQ (Parametric — FabFilter Pro-Q3 or stock)**
- Gentle high-shelf boost: +1–1.5 dB at 10 kHz (air)
- Gentle low-shelf boost: +1 dB at 60 Hz (weight)
- Cut any resonant buildup (sweep and cut)
- Cut below 25 Hz (infrasonic content)

**2. Multiband Compressor (Ozone, Maximus, or free: TDR Molot)**
- Low band (20–200 Hz): Ratio 2:1, gentle compression
- Mid band (200–3 kHz): Ratio 1.5:1, minimal — protect midrange dynamics
- High band (3 kHz+): Ratio 2:1, tame harshness

**3. Limiter**
- Ceiling: **-0.3 dBTP** (inter-sample peak protection)
- Threshold: lower until reaching your LUFS target
- Recommended: **Limiter No6** (free), **Youlean Loudness Meter** (free), or FabFilter Pro-L2

**4. Clipper (Optional, for very loud house masters)**
- Place **before** the limiter
- Soft clip 1–2 dB — converts peaks to distortion before limiting
- Reduces limiter pumping artifacts for cleaner loudness

---

## Reference Track Matching

1. Import a reference track you admire (same subgenre) into your DAW
2. Match its **RMS/LUFS** level to your mix using a gain plugin
3. Rapidly A/B switch between your mix and the reference
4. Trust your ears, not your eyes — match tonal balance, width, and punch

**Free tool:** [REFERENCE plugin by Mastering The Mix](https://www.masteringthemix.com/products/reference) — loads a reference track and shows how your mix compares.

---

## Plugin Recommendations

### Free Mixing/Mastering Plugins

| Plugin | Type | Best For |
|--------|------|---------|
| TDR Nova | Dynamic EQ | Transparent EQ, sidechain |
| Limiter No6 | Limiter | Mastering limiter |
| Youlean Loudness Meter | Metering | LUFS measurement |
| SPAN (Voxengo) | Spectrum Analyzer | Visual frequency reference |
| MeldaProduction MFreeFXBundle | Various | Full suite of free processors |
| Valhalla SuperMVB | Reverb | Studio-quality free reverb |
| OTT (Xfer) | Multiband Comp | Upward compression, density |

### Paid (Worth It)

| Plugin | Type | Why |
|--------|------|-----|
| FabFilter Pro-Q3 | EQ | Best EQ on the market; dynamic EQ |
| FabFilter Pro-C2 | Compressor | Versatile, transparent |
| FabFilter Pro-L2 | Limiter | True peak, ISP, clean limiting |
| Valhalla Room | Reverb | Industry-standard algorithmic reverb |
| iZotope Ozone | Mastering Suite | All-in-one mastering with AI assist |
| Waves SSL Buss Compressor | Bus Comp | Classic SSL glue |

---

## Common House Music Mixing Mistakes

| Mistake | Fix |
|---------|-----|
| Too much reverb on kick | Keep kick dry; only light room reverb at most |
| Muddy low-end | HPF every non-bass element above 150–200 Hz; keep bass mono |
| Harsh hi-hats | Cut 6–8 kHz; high-shelf at 10 kHz instead of boosting 8 kHz |
| Weak sidechain | Increase ratio and lower threshold; check release time (match kick decay) |
| Thin-sounding mix | Check gain staging; pads may need more low-mid presence |
| Over-compressed mix | Mix at lower volumes; revisit compressor ratios (use 2:1–4:1, not 10:1) |
| No mono low-end | Use M/S EQ to keep bass mono; check on a single speaker |
| Clipping the master | Gain stage earlier in the chain; give 6 dB headroom before mastering |
| No reference | Always A/B against a professional track in the same subgenre |
