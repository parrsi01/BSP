# AI Agents and Tools for BSP

A guide to using AI tools across every production role in the team.

---

## Cover Art and Visual Design

### Claude + Midjourney Workflow

The most powerful AI art pipeline for house music cover art.

**Step 1 — Use Claude to write the Midjourney prompt:**

Tell Claude what you need:
```
Write me a Midjourney prompt for a deep house album cover.
The vibe should be: late night, warm amber, minimal, a hint
of smoke and jazz. No text in the image. Square format.
```

Claude will return an optimized, detailed Midjourney prompt with specific parameters.

**Step 2 — Run in Midjourney:**
Paste the prompt into Discord → `#imagine` channel → add `--ar 1:1 --v 6`

**Step 3 — Upscale and export:**
Press U1–U4 to upscale your preferred result → download → bring into Canva or Photoshop → add text overlay.

**Prompt engineering principles for house music:**
- Describe the **mood** before the visual content ("late night, melancholy, underground")
- Specify what you **don't** want ("no text", "no people", "no clichés")
- Mention lighting explicitly ("ambient LED lighting", "golden hour", "club strobes")
- Add art direction terms: "minimal", "editorial", "cinematic", "lo-fi grain"

---

### Adobe Firefly Integration — [firefly.adobe.com](https://firefly.adobe.com)

Use for: extending images, background replacement, generating textures.

- **Generative Fill** (in Photoshop): Select an area → describe what to put there → AI fills it in context
- **Text to Image:** Comparable to Midjourney for quick concept art; safer for commercial use (Adobe trains on licensed content)
- **Generative Expand:** Extend a 1:1 image to 16:9 for YouTube thumbnails without cropping

---

### DALL-E 3 via ChatGPT — [chatgpt.com](https://chatgpt.com)

Use for: rapid concept thumbnails, style exploration, reference generation.

Requires ChatGPT Plus ($20/month).

**Quick prompt format for beat art:**
```
Create album cover art for a tech house beat. Dark, industrial aesthetic.
Electric blue neon against black concrete. Abstract, no text. Square image.
```

DALL-E 3 is more literal than Midjourney — describe the image composition directly.

---

## Music Production AI

### AIVA — [aiva.ai](https://www.aiva.ai)
AI music composition. Use for: **creative inspiration and sketching chord progressions** — not for final releases.

- Input a style, mood, and duration → AIVA generates a full composition
- Export MIDI → import into your DAW → disassemble and use individual elements as inspiration
- Free tier available; paid plans from $11/month

**BSP use case:** Generate a MIDI chord progression in "deep house" style → import to FL Studio/Ableton → adapt the chords to your own arrangement.

---

### Suno AI — [suno.com](https://suno.com)
Text-to-music generation. Use for: **reference ideas and A/B comparisons** only.

- Type a prompt: "Deep house track, jazzy chord stabs, female vocal, 124 BPM" → generates a full song
- Useful for hearing what an AI thinks sounds like your target — helps clarify direction
- **Do not release AI-generated music as your own work**

---

### Soundraw — [soundraw.io](https://soundraw.io)
Royalty-free AI music generation. Use for: **background music for marketing videos**, not beat content.

- Generate royalty-free background music for YouTube beat showcases or social content
- Paid subscription allows commercial use

---

### BandLab AI Mastering — [bandlab.com](https://www.bandlab.com)
Free AI mastering. Use for: **quick masters of demos** when you don't have time for a full manual master.

- Upload WAV → AI analyzes and applies a mastering chain → download
- Results are decent for demos; not as refined as a manual Ozone/FabFilter master
- **Free** — no subscription required

---

### LANDR AI Mastering — [landr.com](https://www.landr.com)
Paid AI mastering. Use for: **release-ready masters at scale** when the full manual pipeline is overkill.

- Subscription from $7.99/month
- Better results than BandLab; genre-aware mastering
- Good for mastering back-catalog or lower-priority releases quickly

---

## Marketing and Copy

Claude is the best tool for all text-based marketing tasks.

### What Claude Can Write for BSP

| Task | Prompt to Claude |
|------|----------------|
| Beat description (BeatStars) | See prompt templates below |
| Instagram caption | See prompt templates below |
| TikTok caption | See prompt templates below |
| Email newsletter | See prompt templates below |
| License agreement | "Write a non-exclusive beat license agreement covering [details]" |
| Artist outreach DM | "Write a cold DM to an emerging house vocalist, offering a free beat. Tone: direct, not salesy" |
| Bio for BeatStars | "Write a 200-word BeatStars bio for BSP, a collective of 4 house music producers specializing in deep, tech, and afro house" |
| Beat title ideas | "Give me 10 beat title ideas for a dark tech house track at 128 BPM in A minor" |

---

## 10 Ready-to-Use Claude Prompt Templates

Copy, customize, and use these directly.

### 1 — Beat Description (BeatStars)
```
Write a 100-word BeatStars beat description for:
- Genre: Deep House
- BPM: 124
- Key: A minor
- Mood: Late night, warm, melancholic
- Elements: jazz chord stabs, walking bass, 909 drums, female vocal samples
- Tone: Confident, slightly poetic, not overly commercial

Include BPM, key, and a closing CTA to purchase.
```

### 2 — Instagram Caption (Beat Drop)
```
Write an Instagram Reel caption for a new tech house beat drop.
- Producer name: BSP
- Beat name: "Concrete Dreams"
- BPM: 128, Key: D minor
- Vibe: Underground, dark, driving
- Max 3 lines + 20 hashtags focused on house music producers and artists
- CTA: link in bio to BeatStars
```

### 3 — TikTok Caption
```
Write a TikTok caption for a 30-second beat preview video.
Short, punchy, max 150 characters. Include: beat name, BPM, a hook
statement that makes an artist want to record on it. No hashtags in the
caption — just the hook text. Genre: Afro House.
```

### 4 — Email Subject Lines (generate 10)
```
Generate 10 email subject lines for a beat drop announcement.
Genre: Soulful house. Beat name: "Feels Like Home". The email
goes to a list of 500 artists who signed up for free beats.
Vary between curiosity-driven, direct, and FOMO-based approaches.
Keep each under 50 characters.
```

### 5 — Email Newsletter Body
```
Write a short email newsletter for BSP's weekly beat drop.
- Beat name: "Ocean Drive" | BPM: 126 | Key: C minor | Genre: Deep house
- Include: 3-sentence beat description, pricing (MP3 $29.99, WAV $49.99)
- CTA: BeatStars link
- Tone: Personal, producer-to-artist, not corporate
- Length: 150 words max
```

### 6 — Social Media Bio
```
Write an Instagram bio for BSP Beats. We are 4 house music producers
making deep, tech, and afro house beats. We sell on BeatStars.
Maximum 150 characters. Must include: genre, a call to action, and
indicate beats are for sale. No emojis unless absolutely necessary.
```

### 7 — Cold DM Script
```
Write a cold DM for Instagram to an emerging house vocalist with
~8,000 followers. We are BSP, a house music producer collective.
We want to offer them a free beat in exchange for tagging us if they
use it. Tone: genuine, not salesy, brief (under 50 words).
```

### 8 — Beat Bundle Description
```
Write a product description for a "5-Beat Deep House Bundle" priced at
$99. Each beat is individually priced at $29.99. Buyers save 33%.
The beats are: 124 BPM, A minor, lush pads, jazz chords, 909 drums.
100 words max. Include the savings calculation.
```

### 9 — Artist Licensing Pitch
```
Write a short pitch to an artist who has been using one of our
non-exclusive beats and is now growing (50K streams on Spotify).
We want to offer them an upgrade to exclusive rights at $399.
Pitch should create urgency (others could also buy it) without
being threatening. 3 sentences max.
```

### 10 — Beat Title Generator
```
Generate 15 beat title ideas for a house music producer collective.
Titles should feel:
- Urban and underground (not generic)
- Like they could be a track name, not just a description
- Open to interpretation
- 1-2 words preferred
Genre mix: deep house, tech house, afro house
```

---

## Workflow Automation

### Zapier — [zapier.com](https://zapier.com)

Free tier: 100 tasks/month. Use for connecting BeatStars, email, and spreadsheets.

**Automation 1 — New BeatStars Sale → Email Notification:**
```
Trigger: New order on BeatStars (via Webhook or Email trigger)
Action: Send email via Gmail "New sale: [Beat Name] — [Amount]"
```

**Automation 2 — BeatStars Sale → Log to Google Sheets:**
```
Trigger: New order on BeatStars
Action: Add row to Google Sheet with: Date, Beat Name, License Type, Amount, Buyer Email
```

**Automation 3 — New Email Subscriber → Send Welcome Email:**
```
Trigger: New subscriber in Mailchimp/ConvertKit
Action: Send Gmail with free beat download link
(For this, ConvertKit's built-in automation is easier — use Zapier only if cross-platform needed)
```

---

### Make (formerly Integromat) — [make.com](https://www.make.com)

More powerful than Zapier for complex workflows. Free tier: 1,000 operations/month.

**Instagram Post Scheduler Automation:**
```
Trigger: New row added to Google Sheets (content calendar)
Action: Post image + caption to Instagram Business Account
Schedule: Daily at 7pm
```

Note: Direct Instagram posting via API requires a Business or Creator account linked to a Facebook Page.

---

### Notion AI — [notion.com](https://www.notion.com)

Use for: **AI-powered beat catalog management and content creation**.

- Build a beat catalog database in Notion (title, BPM, key, genre, mood, BeatStars link, upload date)
- Use Notion AI to: generate descriptions from metadata, draft captions, summarize analytics notes
- Notion AI is included in Notion Plus ($8/month) and above

**Beat Catalog Template Fields:**
```
| Beat Name | BPM | Key | Genre | Mood | Upload Date | BeatStars URL | Revenue |
```

---

## Claude on iOS — On-the-Go Workflow

### Claude App Setup
Download the Claude app (iOS/Android) — free tier available, Pro ($20/month) for faster responses and more context.

### On-the-Go Beat Description Workflow
1. Record a 30-second voice note of yourself describing the beat's vibe (on phone)
2. Transcribe using iOS built-in transcription or Whisper AI
3. Paste into Claude app: "Clean this up into a 100-word BeatStars description: [transcription]"
4. Copy → paste directly into BeatStars on mobile

### Voice-to-Text → Claude → Social Caption
1. Use iOS dictation to voice-record a caption idea (messy, natural)
2. Paste into Claude: "Rewrite this as a clean Instagram caption for a house music beat drop: [raw text]"
3. Copy output → paste into Instagram or Buffer

### Quick Prompts as iOS Shortcuts
Use the **Shortcuts app** (iOS) to save frequently used Claude prompts:

1. Open Shortcuts → New Shortcut
2. Add action: **Text** → paste your template prompt with [PLACEHOLDER] tokens
3. Add action: **Copy to Clipboard**
4. Name the shortcut: "BSP Beat Description"
5. Add to Home Screen
6. Tap shortcut → edit the placeholder text → paste into Claude

**Recommended shortcuts to create:**
- "BSP Beat Description" — the full BeatStars description template
- "BSP Instagram Caption" — the Instagram Reel caption template
- "BSP Cold DM" — the artist outreach DM template
- "BSP Email Subject" — subject line generation prompt
