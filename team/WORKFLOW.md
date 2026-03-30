# Team of 4 Workflow Guide

---

## Role Division

| Role | Primary Responsibilities | Secondary |
|------|------------------------|----------|
| **Beat Maker A** (FL Studio 20) | Beat production, arrangement, sound design | Mixing review |
| **Beat Maker B** (Ableton Live) | Beat production, live performance prep, loop creation | Sound design R&D |
| **Beat Maker C** (Logic Pro X) | Beat production, mixing, mastering | Cross-DAW stems bouncing |
| **Marketing Lead / Designer** | Social media, cover art, BeatStars uploads, licensing, email | Beat copy writing |

### Responsibilities Overlap — Who Does What When

| Task | Owner | Support |
|------|-------|---------|
| New beat production | Beat Maker (respective) | — |
| Initial mix | Producer who made the beat | — |
| Final mix review | Beat Maker C (Logic) | Beat Maker A or B |
| Mastering | Beat Maker C | BandLab/LANDR for overflow |
| Cover art | Marketing Lead | Generator AI tools |
| BeatStars upload | Marketing Lead | Producer provides tags + metadata |
| Social media posts | Marketing Lead | All team provides clips |
| Artist outreach | Marketing Lead | All team reviews DM scripts |
| License agreements | Marketing Lead | Review with full team quarterly |

---

## Daily Production Targets

### Per Producer per Week

| Producer | Beats per Week | Notes |
|---------|---------------|-------|
| Beat Maker A | 2–3 new beats | 1 fully arranged, 1-2 sketches |
| Beat Maker B | 2–3 new beats | At least 1 DJ-ready (5+ min) |
| Beat Maker C | 1–2 beats + 2 mixes | Mixes for team's finished beats |
| Marketing Lead | 0–1 beat | Production not primary focus |

**Monthly target for the collective:** 20–30 beats produced, 10–15 finalized and uploaded.

### Quality Gate: A beat is "finished" when:
- [ ] Fully arranged (intro/drop/breakdown/outro)
- [ ] Mixed and A/B'd against reference track
- [ ] Mastered to -8 LUFS or -14 LUFS depending on release target
- [ ] Stems exported (if exclusive tier offered)
- [ ] Cover art created (1000x1000px)
- [ ] BeatStars metadata: title, BPM, key, genre tags, description
- [ ] Tagged MP3 version exported

---

## Beat Quality Checklist Before Upload

Every beat must pass this checklist before the Marketing Lead uploads it:

### Technical
- [ ] No clicks, pops, or digital artifacts
- [ ] Mix checked in mono (no phase cancellation)
- [ ] Checked on laptop speakers (not just studio monitors)
- [ ] LUFS measured and confirmed (-8 to -10 for BeatStars, -14 for streaming)
- [ ] True peak below -0.3 dBTP
- [ ] Stems are clean and labeled correctly

### Creative
- [ ] 4-on-the-floor kick pattern is solid
- [ ] Sidechain compression working properly
- [ ] Arrangement has clear intro, drop, breakdown, drop 2, outro
- [ ] DJ-friendly: at least 8 bars of clean drums at intro and outro
- [ ] Reviewed against a reference track in the same subgenre

### Delivery
- [ ] WAV master exported (24-bit, 44.1kHz)
- [ ] Tagged MP3 with beat tag at 0:30 intervals
- [ ] Stems ZIP (kick, bass, chords, lead, fx, full mix)
- [ ] Naming convention followed: `BSP_BeatName_BPM_Key_v1.wav`

---

## Shared Folder Structure

Use Google Drive or Dropbox. Never put audio files in the GitHub repo.

```
BSP Team Drive/
├── 00_ACTIVE_PROJECTS/
│   ├── BeatMakerA/
│   │   ├── Beat_Warm_Nights_126_Am/
│   │   │   ├── BSP_WarmNights_126_Am_MASTER.wav
│   │   │   ├── BSP_WarmNights_126_Am_TAGGED.mp3
│   │   │   ├── Stems/
│   │   │   └── ProjectFile_FL.zip
│   └── BeatMakerB/
│   └── BeatMakerC/
├── 01_READY_TO_UPLOAD/
│   └── [beats that passed QC, awaiting upload]
├── 02_UPLOADED/
│   └── [uploaded beats, organized by month]
├── 03_SAMPLES_LOOPS/
│   ├── Drums/
│   ├── Bass/
│   ├── Chords/
│   └── FX/
├── 04_GRAPHICS/
│   ├── Cover_Art/
│   ├── Visualizers/
│   └── Templates/
├── 05_MARKETING/
│   ├── Social_Clips/
│   ├── Email_Templates/
│   └── Analytics/
└── 06_CONTRACTS_LICENSES/
    ├── License_Templates/
    └── Executed_Licenses/
```

---

## Version Control for Beats

### File Naming Convention
```
BSP_[BeatName]_[BPM]_[Key]_[Version].[ext]
```

**Examples:**
```
BSP_WarmNights_126_Am_v1.wav        ← First draft
BSP_WarmNights_126_Am_v2.wav        ← After feedback revision
BSP_WarmNights_126_Am_MASTER.wav    ← Final master
BSP_WarmNights_126_Am_TAGGED.mp3    ← Tagged preview
BSP_WarmNights_126_Am_STEM_Kick.wav ← Stem file
```

### Version Notes
Keep a simple `NOTES_[BeatName].txt` in the beat folder:
```
v1 — Initial arrangement, 2024-01-15
v2 — Adjusted bassline, added perc layer, 2024-01-17 (feedback from C)
v3 — Re-mastered after mix note about kick, 2024-01-18
MASTER — Approved by team, uploaded BeatStars 2024-01-19
```

---

## Feedback Loop

### How to Review Each Other's Beats

1. **Reviewer listens on 3 setups:** Studio monitors, headphones, and phone/laptop speaker
2. **Reference check:** Pull up a similar professional track and A/B compare
3. **Leave comments in the notes file** — not verbal (written is trackable)

### Feedback Categories
Use consistent language in feedback:

| Category | Example Comment |
|----------|----------------|
| Technical | "Kick is too loud vs mix, -2dB" |
| Creative | "Breakdown feels too short — extend by 8 bars" |
| Genre accuracy | "This feels more nu-disco than tech house" |
| Mix | "Pads are too wide — check mono" |
| Arrangement | "Intro is only 8 bars — DJs need 32" |

### Veto Rule
If 2 out of 4 team members flag the same issue, it **must be fixed** before upload. One person's subjective taste doesn't block a release, but shared concerns do.

---

## Revenue Split Agreement Template

Formalize the revenue split in a written document all 4 members sign. Revisit annually.

**Default split (suggested):**

| Scenario | Recommended Split |
|----------|-----------------|
| Solo beat (one producer) | Producer: 70% / Team marketing fund: 30% |
| Collaborative beat (2 producers) | Producer A: 35% / Producer B: 35% / Team fund: 30% |
| Beat with featured design (producer + marketing) | Producer: 55% / Designer: 15% / Team fund: 30% |
| Team fund usage | Reinvest in samples, plugins, ads |

**Important:** Revenue splits are between the team. Copyright ownership remains with the producing member(s) unless separately agreed in writing.

---

## Communication: Discord Server Setup

### Recommended Server Structure

| Channel | Purpose |
|---------|---------|
| `#general` | General chat |
| `#beat-drops` | Post new beats for team listening |
| `#feedback` | Written beat feedback threads |
| `#marketing` | Coordination on social posts, uploads |
| `#analytics` | Share weekly stats from BeatStars/social |
| `#samples-sharing` | Share found loops, samples, links |
| `#revenue` | Monthly revenue reports (private) |
| `#resources` | Plugin deals, free sample packs |

### Voice Channels
- `Studio` — drop in for casual production sessions together
- `Weekly Sync` — reserved for weekly meeting

### Notification Rules
- `@here` only for urgent releases or issues
- Pin important messages (beat naming decisions, pricing changes)

---

## Weekly Team Meeting Agenda Template

**Day:** Every Monday, 7pm [your timezone]
**Duration:** 45 minutes max
**Platform:** Discord voice

```
AGENDA — BSP Weekly Sync [Date]

1. Last Week Review (10 min)
   - Beats produced: [number]
   - Beats uploaded: [number]
   - Revenue: [total]
   - Top-performing content: [platform + post]

2. Current Projects Update (10 min)
   - [Producer A]: Working on _____, ETA _____
   - [Producer B]: Working on _____, ETA _____
   - [Producer C]: Working on _____, mixing _____
   - [Marketing]: Campaigns running, scheduled posts

3. Feedback Queue (10 min)
   - Beats waiting for review: [names]
   - Quick listen and verdict: pass / needs changes

4. This Week Goals (10 min)
   - Production: X beats to finish
   - Marketing: X posts to schedule, X beats to upload
   - One shared goal: _______________

5. Any Issues / Decisions (5 min)
   - Pricing changes?
   - New samples to buy?
   - License agreement updates?

ACTION ITEMS: [name] will [task] by [date]
```
