# Beat Quality Checklist — Before Every Upload

A thorough pre-upload quality control process for BSP. Run this checklist for every beat before it touches a storefront, streaming platform, or artist inbox. No beat leaves the session without passing all six sections.

---

## Overview

| Section | Focus | Stage |
|---------|-------|-------|
| 1. Production Check | Arrangement, structure, catchiness | In session |
| 2. Mix Check | Balance, separation, frequency clarity | Post-mix |
| 3. Master Check | Loudness, dynamic feel, playback translation | Post-master |
| 4. File Export | File format, naming, stems | Pre-upload |
| 5. Metadata | Tags, descriptions, cover art | Platform setup |
| 6. Marketing Prep | Content, captions, scheduling | Launch day |

---

## Section 1: Production Check

Run this while still in your DAW, before mixing begins.

- [ ] **BPM is locked and consistent throughout** — no unintentional tempo drift; verify in DAW tempo ruler; quantize any live-played elements that need it
- [ ] **Key is identified and noted** — document in file name and internal notes; all melodic elements harmonically consistent
- [ ] **No unintentional clipping in any channel** — check every channel strip; red clip indicators cleared; gain stage properly set before any processing
- [ ] **Kick and bass are not fighting** — low-end frequency separation achieved via sidechain compression (kick ducking bass ~6dB at 60–120Hz) or EQ notching (high-pass bass around kick's fundamental, or vice versa)
- [ ] **Main hook/melody is memorable and appears within first 16 bars** — artists on BeatStars make purchase decisions in the first 30 seconds; the best element must hit early
- [ ] **Arrangement has clear structure:**
  - [ ] Intro (4–8 bars, builds anticipation, no full drop)
  - [ ] Verse section (stripped back, space for rap or vocal)
  - [ ] Pre-chorus / build (energy increase)
  - [ ] Hook / chorus (full arrangement, all elements)
  - [ ] Breakdown / bridge (stripped or contrasting)
  - [ ] Outro (gradual reduction or hard cut)
- [ ] **Beat length minimum 3:30 for sync/licensing uses** — 2:30 minimum for BeatStars/SoundCloud previews
- [ ] **Repetition is intentional, not lazy** — every section should feel purposeful; "copy-paste" arrangement should have at least one evolving element (filter sweep, percussion add/remove, etc.)
- [ ] **Vocal space exists** — the arrangement does not stack frequencies in the 500Hz–3kHz range so densely that a vocal cannot sit without being buried

---

## Section 2: Mix Check

Run after the mix is complete, before mastering.

### Gain Staging
- [ ] No channel peaking above **-6dBFS pre-fader** before processing (headroom for mix bus processing)
- [ ] Mix bus (stereo output) peaking no higher than **-3dBFS** before limiter

### Low End
- [ ] **Mono check completed** — collapse stereo to mono (in your DAW or via a mono utility plugin); kick and bass should still be audible and defined; no cancellation
- [ ] **Kick and bass have distinct frequency roles** — kick punches in 60–100Hz range; bass occupies 100–250Hz range; sub frequencies not competing
- [ ] **High-pass filter applied** to all non-bass elements — synths, pads, leads should have HP filter removing unnecessary low-frequency mud (typically 80–200Hz cut depending on source)

### High End
- [ ] **No harsh high frequencies** — test on cheap earbuds (AirPods, standard 3.5mm); any sibilance, harsh hat, or sharp synth attack that fatigues the ear must be addressed with a de-esser or shelf cut above 10kHz
- [ ] Checked on: studio monitors + headphones + laptop speakers + phone speakers (all four)

### Reference Comparison
- [ ] **A/B reference track comparison done** — import a reference track from your genre at approximately the same perceived loudness; flip between reference and your beat 5+ times; note: overall loudness, low-end weight, stereo width, hi-hat presence, vocal space

### Stereo Field
- [ ] **No phase issues** — mono fold test (see above); use a phase correlation meter (green = in phase; avoid red)
- [ ] **Stereo width is intentional** — center: kick, snare, bass, lead vocal; sides: pads, background FX, wide synths; nothing critical should be only in one ear

### Vocal Space
- [ ] **500Hz–2kHz range has room for a vocalist** — if your primary melody occupies this range, it should have a notch or be lower in the mix to allow a lead vocal to cut through without competing
- [ ] Test by playing the mix and singing (or humming) along — if your voice disappears, the mix is too dense in the vocal range

---

## Section 3: Master Check

Run after mastering is applied (final limiter stage).

### Loudness Targets

| Destination | Integrated LUFS | True Peak Max |
|-------------|----------------|---------------|
| Spotify / Apple Music | **-14 LUFS** | -1.0 dBTP |
| BeatStars store preview | **-8 LUFS** (punchy, competitive) | -0.5 dBTP |
| YouTube | **-14 LUFS** | -1.0 dBTP |
| SoundCloud | **-14 LUFS** | -1.0 dBTP |
| Radio / broadcast | -23 LUFS | -3.0 dBTP |

- [ ] **Integrated loudness measured** — use a LUFS meter (free options: Youlean Loudness Meter, ToneBoostr LM-Correct; paid: iZotope Insight)
- [ ] **True peak checked** — inter-sample peaks addressed; no values above target
- [ ] **No pumping or distortion from limiter** — if limiter is working harder than 3–4dB of gain reduction peak, your mix is too loud going into it; pull back the mix bus level instead

### Translation Testing
- [ ] Sounds good on **studio monitors** — spatial, balanced, defined
- [ ] Sounds good on **headphones** — check for harsh frequencies and stereo imbalance
- [ ] Sounds good on **laptop speakers** — does the beat lose all low end and feel empty? If so, mid-frequency presence needs work
- [ ] Sounds good on **phone speakers** — the most critical test for streaming audiences; if your beat sounds weak here, the mix needs more presence in 1–5kHz and tighter low end

---

## Section 4: File Export

### Files to Export Per Beat

| File | Format | Specs | Purpose |
|------|--------|-------|---------|
| Tagged MP3 (with beat tag watermark) | MP3 | 320kbps, ID3 tags filled | SoundCloud preview, free download |
| Clean WAV (untagged) | WAV | 44.1kHz, 24-bit | Lease delivery |
| All stems (for unlimited/exclusive) | WAV per stem group | 44.1kHz, 24-bit | Unlimited lease and exclusive delivery |

### Stem Groups to Export

| Stem Name | What It Includes |
|-----------|-----------------|
| Drums | Kick, snare, hi-hats, percs, claps — all routed to one stem |
| Bass | Bass synth, 808, sub — all bass elements |
| Melody | Lead melody instrument(s) |
| Chords / Harmony | Pads, chord stabs, harmonic elements |
| FX / Atmosphere | Risers, downlifters, reverb tails, atmospheric textures |
| Extras (if applicable) | Any element not fitting above categories |

**Export method:** Mute all other tracks, solo one group, export full-length WAV. Ensure all stems are the same length (even if silent at the start/end — no trimming). This ensures perfect sync when stacked in a DAW.

### Beat Tagging

Every tagged preview file must include:
- Vocal tag from all 4 producers or a group tag (e.g., "BSP" said audibly)
- Frequency: every 8–16 bars (not just beginning and end)
- Tag must be in the center of the stereo field (mono compatible)
- Tag should not mask the primary melody — it should announce, not dominate

### File Naming Convention

```
BSP_[BeatName]_[BPM]BPM_[Key]_[Version].wav
```

Examples:
```
BSP_CityLights_140BPM_FMin_tagged.mp3
BSP_CityLights_140BPM_FMin_clean.wav
BSP_CityLights_140BPM_FMin_stems_drums.wav
BSP_CityLights_140BPM_FMin_stems_bass.wav
BSP_CityLights_140BPM_FMin_stems_melody.wav
BSP_CityLights_140BPM_FMin_stems_chords.wav
BSP_CityLights_140BPM_FMin_stems_fx.wav
```

**No spaces in file names** — use underscores. Spaces cause problems in some DAWs and server environments.

- [ ] Tagged MP3 exported and named correctly
- [ ] Clean WAV exported and named correctly
- [ ] Stems exported (if applicable) and named correctly
- [ ] Files moved to correct folder in project file system

---

## Section 5: Metadata

### BeatStars / Airbit Listing
- [ ] **Title format:** `[Genre keyword] + [Beat Name] + [BPM] + [Key]`
  - Example: "Afrohouse Beat — City Lights 140 BPM F Minor"
- [ ] **5 relevant tags selected** — be specific: "afrohouse 2025", "deep house instrumental", "140bpm beat", "F minor", "BSP"
- [ ] **Description written** — include: genre, mood, BPM, key, license pricing, buy link, collab info
- [ ] **License prices set** — all tiers (basic, premium, unlimited, exclusive) with correct file delivery assigned
- [ ] **Buy link is active and correct** — test it
- [ ] **Beat added to correct playlist** on BeatStars/SoundCloud (genre playlist, new releases playlist)

### Cover Art
- [ ] **Dimensions: 3000x3000px minimum** (square format)
- [ ] **No pixelation, blur, or compression artifacts** — export from source at full resolution
- [ ] **Beat title is readable at thumbnail size** (check at 150x150px in browser)
- [ ] **Branding consistent** — BSP logo or brand element visible
- [ ] **File format:** JPG (max 5MB) or PNG for transparency support

### SoundCloud-Specific
- [ ] **Uploaded to SoundCloud** with tagged MP3
- [ ] **Description includes** buy link to BeatStars listing
- [ ] **Buy link button set** in SoundCloud track settings (direct link to BeatStars)
- [ ] **Genre and tags** filled in SoundCloud settings
- [ ] **Added to relevant SoundCloud playlists**

### Distribution Metadata (if distributing)
- [ ] Composer credits listed for all contributors
- [ ] Genre correctly selected
- [ ] Release date set (minimum 7 days out; 3–4 weeks if pitching to Spotify editorial)
- [ ] PRO registration submitted before release date
- [ ] Refer to full checklist in `resources/DISTRIBUTION_GUIDE.md`

---

## Section 6: Marketing Prep

Do not upload and hope — every release needs a brief but real marketing push.

- [ ] **Beat clip recorded (30–60 seconds)** — record a screen or camera clip of your DAW playing the beat for Reels and TikTok; or record a phone video of you in the studio with the beat playing
- [ ] **Waveform video created** — use Wavve.co, Headliner, or Canva's audio visualizer to make an animated waveform video for static platforms (Instagram feed, Twitter/X)
- [ ] **Caption written for Instagram** — include: beat name, BPM, key, "Link in bio" call to action, relevant hashtags (8–12, mix of niche and broad)
- [ ] **Caption written for TikTok** — shorter, hook-first, 3–5 hashtags
- [ ] **Posting time scheduled** — based on when your audience is most active (Instagram Insights; TikTok Analytics); general benchmark: Tue–Thu, 6–9pm local time in target market
- [ ] **Team member assigned** — who is posting, who is monitoring comments for the first 2 hours post-upload

### Hashtag Strategy (Instagram)

| Category | Example Tags | Count |
|----------|-------------|-------|
| Niche / genre | #afrohouse #trapbeats #rnbinstrumental | 3–4 |
| BPM / key specific | #140bpm #fminor | 1–2 |
| Producer community | #beatmaker #producers #hiphopbeats | 2–3 |
| Location (if relevant) | #ukproducers #londonbeats | 1–2 |
| Brand | #BSP #buysomebeats (your tag) | 1 |

**Avoid:** Using the exact same hashtag set every post — rotate them to avoid the algorithm treating your account as repetitive.

---

## Final Sign-Off

Before publishing:

```
Producer who made the beat: _______________
Date completed: _______________
Mix engineer (if different): _______________
Master engineer (if different): _______________

Section 1 - Production:     PASS / FAIL
Section 2 - Mix:            PASS / FAIL
Section 3 - Master:         PASS / FAIL
Section 4 - File Export:    PASS / FAIL
Section 5 - Metadata:       PASS / FAIL
Section 6 - Marketing Prep: PASS / FAIL

All sections pass: [ ] YES — cleared for upload
```

Any FAIL on Sections 1–4 = beat goes back to production. No exceptions.
Sections 5–6 can be completed day of upload, but must be done before going live.
