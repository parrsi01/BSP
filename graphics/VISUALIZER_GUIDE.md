# Music Visualizer Creation Guide

---

## Platform Size and Format Requirements

| Platform | Dimensions | Aspect Ratio | Frame Rate | Format |
|----------|-----------|-------------|-----------|--------|
| YouTube | 1920 x 1080 px | 16:9 | 30 fps | MP4 (H.264) |
| TikTok | 1080 x 1920 px | 9:16 | 30 fps | MP4 |
| Instagram Reels | 1080 x 1920 px | 9:16 | 30 fps | MP4 |
| Instagram Feed | 1080 x 1080 px | 1:1 | 30 fps | MP4 |
| YouTube Shorts | 1080 x 1920 px | 9:16 | 30 fps | MP4 |
| SoundCloud (static) | 800 x 800 px | 1:1 | N/A | JPEG/PNG |

---

## Free Visualizer Tools

### Renderforest — [renderforest.com](https://www.renderforest.com)
- Free tier available (watermarked)
- Reactive audio visualizer templates — upload your MP3, it animates to the music
- Good template variety: waveform, spectrum, circular
- Paid ($10–$20/month) removes watermark

### Kapwing — [kapwing.com](https://www.kapwing.com)
- Free tier (watermark on free)
- Add waveform animation to any video
- Good for quickly adding a waveform bar to a beat video
- Also useful for resizing/reformatting between platforms

### Canva Video — [canva.com](https://www.canva.com)
- Free tier includes basic video editing
- Animated elements, text animations, transitions
- Good for TikTok/Reels content with beat clips
- Not reactive audio (waveform doesn't move to the music) — use for styled beat promo videos

### Veed.io — [veed.io](https://www.veed.io)
- Free tier (with watermark)
- Waveform visualizer + text + subtitles
- Good for quick Instagram/TikTok beat clips
- Subtitle generation for vocal-heavy beats

---

## Paid / Professional Tools

### After Effects (Adobe) — industry standard for visualizers
- Part of Adobe Creative Cloud ($54.99/month full suite)
- Full creative control; complex reactive animations
- Steep learning curve — see step-by-step below

### Motion Array — [motionarray.com](https://motionarray.com)
- After Effects and Premiere Pro templates
- $29.99/month for full library access
- Search: "music visualizer", "audio spectrum", "waveform"
- Download template → replace audio → render → done

### Envato Elements — [elements.envato.com](https://elements.envato.com)
- $16.50/month for unlimited template downloads
- Large library of After Effects visualizer templates
- Filter for audio spectrum or music visualizer templates

---

## AI-Powered Visualizer Tools

### Vizzy — [vizzy.io](https://vizzy.io)
- AI-powered audio-reactive visualizer creation
- Drag in your audio → AI generates a reactive visual
- More creative than template-based tools

### Motionbox — [motionbox.io](https://motionbox.io)
- AI video creation including audio visualizers
- Good for quick, polished results without manual design

### Veed.io AI
- Veed's AI features can auto-generate video content from audio
- Useful for quick social media versions

---

## Creating a Reactive Waveform Visualizer in After Effects

Step-by-step guide for creating a professional audio-reactive visualizer:

### Setup
1. Open After Effects → **New Composition**
2. Settings: 1920x1080, 30fps, duration 4 minutes (or length of beat)
3. Import your audio: **File → Import → File** → select WAV/MP3

### Background Layer
1. Create a **New Solid** (Cmd/Ctrl+Y): black or dark color (#0A0A0A)
2. This is your background

### Add the Audio Spectrum Effect
1. Create another **New Solid** — this will be the spectrum
2. Go to **Effect → Generate → Audio Spectrum**
3. In Effect Controls:
   - **Audio Layer:** select your imported audio file
   - **Start Point:** set to left edge of composition (e.g., 100, 540)
   - **End Point:** set to right edge (e.g., 1820, 540)
   - **Frequency Bands:** 128 (more bands = smoother, more detailed spectrum)
   - **Maximum Height:** 200–400 (adjust to taste)
   - **Thickness:** 2–4
   - **Inside Color / Outside Color:** set to your brand color

### Add Your Cover Art
1. Import your 1000x1000px cover art
2. Scale to 300x300px in the composition
3. Position: lower left or center
4. Add a **Drop Shadow** effect for depth

### Add Beat Title and Producer Name
1. **Text Tool** (T key) → click in composition → type beat title
2. Font: your brand font (install first in your OS)
3. Position: near cover art or centered above it
4. Add subtle **Fade In** animation (keyframe opacity 0 at 0:00 → 100 at 0:30)

### Add Watermark/Tag Text
1. Add text: "BSP Beats" or your producer name
2. Opacity: 30–50% (subtle watermark)
3. Position: corner of the frame

### Export
1. **File → Export → Add to Adobe Media Encoder Queue**
2. Format: **H.264** (MP4)
3. Preset: **YouTube 1080p HD** (for YouTube) or **Match Source High Bitrate**
4. Output file name: `BSP_BeatName_Visualizer_1080p.mp4`
5. Render

---

## Free After Effects Templates for House Music

Search these sources for free AE visualizer templates:

| Source | URL | What to Search |
|--------|-----|---------------|
| Mixkit | [mixkit.co](https://mixkit.co) | "music visualizer", "audio spectrum" |
| Videezy | [videezy.com](https://videezy.com) | "music visualizer after effects" |
| Motion Array Free | [motionarray.com/free](https://motionarray.com/free) | "visualizer" |
| Envato Tuts | [tutsplus.com](https://tutsplus.com) | After Effects visualizer tutorials |

---

## Adding Album Art + Title + Watermark (Without After Effects)

### Using Canva (Easiest Method)
1. Open Canva → create a **1920x1080** design
2. Add a **dark gradient background** or solid color
3. Add your cover art image (center or left side)
4. Add text: Beat name, BPM, producer tag
5. Download as MP4 (Canva lets you animate text elements)
6. Use Kapwing or Veed.io to **add the waveform animation** on top

### Layering in Capcut (Free, Mobile/Desktop)
1. Import your background video/animation
2. Overlay text layers for beat title and producer name
3. Add Kapwing-generated waveform video as a picture-in-picture layer
4. Export at 1080p

---

## Exporting: H.264 for YouTube and Social

### After Effects → Media Encoder Settings

| Platform | Resolution | Codec | Bitrate | Audio |
|----------|-----------|-------|---------|-------|
| YouTube | 1920x1080 | H.264 | 8–10 Mbps | 320 kbps AAC |
| TikTok/Reels | 1080x1920 | H.264 | 4–6 Mbps | 320 kbps AAC |
| Instagram Feed | 1080x1080 | H.264 | 4–6 Mbps | 320 kbps AAC |

**Important:** YouTube compresses uploaded video further — upload at the highest quality you can to minimize generation loss.

---

## Free Stock Video Sources for Visualizer Backgrounds

| Source | URL | License |
|--------|-----|---------|
| Pexels | [pexels.com/videos](https://www.pexels.com/videos) | Free, commercial use OK |
| Pixabay | [pixabay.com/videos](https://pixabay.com/videos) | Free, commercial use OK |
| Coverr | [coverr.co](https://coverr.co) | Free, commercial use OK |
| Mixkit | [mixkit.co](https://mixkit.co) | Free (varies per asset) |
| Life of Vids | [lifeofvids.com](https://www.lifeofvids.com) | Free |

### Best Search Terms for House Music Backgrounds

| Mood | Search Terms |
|------|-------------|
| Club/night | "nightclub lights", "laser lights", "dance floor", "crowd" |
| Minimal/abstract | "abstract loop", "geometric animation", "particles", "neon" |
| Organic/deep | "smoke", "fog", "water reflection", "bokeh lights" |
| Afro house | "sunset Africa", "earth tones abstract", "desert dunes" |
| Cosmic/melodic | "space", "nebula", "starfield", "universe" |

### Licensing Note
Even free stock video has licensing terms — always verify "commercial use" is permitted before uploading to YouTube monetized content.
