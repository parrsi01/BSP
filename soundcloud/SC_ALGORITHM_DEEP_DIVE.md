# SoundCloud Algorithm — Complete Deep Dive

## 1. How the Feed Works

SoundCloud's main feed (the "Stream") shows content in this priority order:

| Source | Feed Weight | Notes |
|--------|-------------|-------|
| Uploads from followed accounts | Highest | Appears immediately on upload |
| Reposts from followed accounts | High | Appears as "[Name] reposted" |
| Suggested tracks (algo-driven) | Medium | Based on listening history |
| Promoted tracks | Paid | Blended in with organic content |

The feed is not purely chronological. SoundCloud applies a relevance score that factors in:
- Your listening history (genre affinity)
- How engaged you've been with a specific account before
- Whether the account uploaded recently (recency bias)
- Engagement velocity on the specific track (see section 8)

**Practical implication:** Tracks from accounts you interact with regularly appear higher. This is why comment reciprocity matters — it trains followers' feeds to surface your content preferentially.

---

## 2. Discover Weekly Equivalent — Suggested Tracks & Stations

SoundCloud's equivalent of Spotify's Discover Weekly is delivered via:

- **"Suggested Tracks"** — appears after a track ends if autoplay is on; algorithm selects based on genre similarity, engagement overlap, and listener history
- **"Stations"** — infinite radio mode starting from a seed track or artist; SC's curation combines editorial picks and algorithmic selections
- **"Weekly Picks" playlists** — algorithmically generated for Go+ subscribers based on listening history

**How to get into Suggested Tracks:**
1. High engagement rate on your track (likes + reposts relative to plays)
2. Accurate genre tagging — SC's similarity engine is genre-anchored
3. Your track appearing in playlists alongside already-popular tracks in the genre
4. Being reposted by accounts that the target listener already follows

The algorithm learns genre proximity from co-occurrence in playlists and repost patterns. If multiple curators who post deep house also repost your track, SC starts classifying your account as a deep house authority.

---

## 3. Search Ranking Factors

SoundCloud search is not pure text-match. The ranking formula weights these factors:

| Factor | Weight | Notes |
|--------|--------|-------|
| Title keyword match | Very High | Exact match outperforms partial |
| Tag match | High | All 5 tags are indexed; exact tag = strong signal |
| Description keywords | Medium | SC indexes first ~1000 chars of description |
| Play count | High | More plays = higher authority ranking |
| Engagement rate (likes/plays) | High | Engagement rate beats raw play count |
| Recency | Medium | Recent uploads get a temporary boost for ~72 hours |
| Account authority | Medium | Older accounts with consistent upload history rank higher |
| Profile completeness | Low | Complete profiles get marginal boost |

**Search field priority order:** Title > Tags > Username > Display Name > Description > Playlist names

**Exact match is critical.** If someone searches "afro house type beat", a track titled "Afro House Type Beat 'Lagos'" ranks above "Afro House Instrumental" even with fewer plays.

---

## 4. The Repost Amplification Loop

Reposts are the most powerful organic distribution mechanism on SoundCloud.

**How the loop compounds:**

```
You upload → 1,000 followers see it
Producer A (2,000 followers) reposts → 2,000 new potential listeners
Producer B (1,500 followers) reposts → 1,500 more
Producer C (3,000 followers) reposts → 3,000 more
Total reach: 7,500 without spending anything
```

**Key mechanics:**
- Each repost is a full feed insertion for every follower of the reposter
- Reposts create a second "freshness" signal — even a 2-week-old track gets fresh algorithm treatment when reposted
- Cascading reposts (A reposts, their follower B also reposts) multiply reach exponentially
- SoundCloud shows the full repost chain: "Producer B reposted from Producer A" — social proof visible to the end listener

**Repost timing matters:** A repost within 2–6 hours of original upload captures the maximum engagement velocity window (see section 8). A repost 3 days later gets full feed insertion but misses the velocity spike.

---

## 5. Trending Charts — How to Climb Them

SoundCloud operates genre-specific charts with two tiers:

**"New & Hot"** — Tracks gaining rapid engagement relative to their age
**"Top"** — All-time or period leaders by raw play/engagement volume

**Chart ranking factors:**
- Plays per hour (velocity, not total)
- Likes per play ratio
- Reposts in the last 24 hours
- New followers gained via the track
- Time since upload (newer tracks compete in "New & Hot" more easily)

**How to climb New & Hot:**
1. Coordinate repost network to fire within the first 2 hours of upload
2. Immediately post to all social channels on upload (not the next day)
3. Send track to 5–10 artists/fans for a "listen and like" before it goes live
4. Genre accuracy is mandatory — SoundCloud places tracks in charts based on their genre setting, not just tags

**Genre chart reality:** Smaller genres (afro house, trap dancehall) have far less competition than "Hip-Hop" or "Electronic." A track that would rank #200 in Electronic might reach top 10 in Afro House. Always set the most specific genre available.

---

## 6. New & Hot vs Top — The Difference

| Chart | What It Shows | Best For |
|-------|--------------|----------|
| New & Hot | Fastest-rising tracks in last 7 days | New accounts, recent uploads |
| Top | Most played tracks, longer timeframe | Established accounts, proven tracks |
| Trending | Real-time momentum chart | Highest volatility, hardest to crack |

**Strategic use:**
- Target "New & Hot" aggressively with every new upload (coordinated repost launch)
- "Top" charts build passively as a track accumulates plays over months
- Being in "New & Hot" even briefly (a few hours in top 20) generates a significant permanent play spike because listeners browsing the chart find and play your track

---

## 7. The 30-Second Rule

**SoundCloud only counts a play after 30 seconds of listening.** This is the single most important fact for track structure.

**What this means for beat production:**
- Intros longer than 15 seconds will cause significant drop-off before the play counts
- The hook or main groove must hit by bar 4 (at 120 BPM, bar 4 = ~8 seconds)
- Fade-ins and long build-ups are algorithm killers
- The 30-second mark should ideally land at a peak moment (drop, chorus equivalent, hardest bar of the groove)

**Completion rate engineering:**
1. Full energy by 0:15
2. First breakdown at 0:45–1:00 (provides contrast, keeps attention)
3. Second peak at 1:30–2:00 (re-engages any passive listeners)
4. Outro can be long — listeners who make it past 2:30 almost always finish

**Completion rate benchmark:** Aim for 60%+ average completion on beats. Under 40% means your intro is losing people before the play even counts.

---

## 8. Engagement Velocity

SoundCloud's algorithm heavily weights **engagement per unit time**, not just cumulative totals.

**Velocity vs volume:**

| Scenario | Algorithm Response |
|----------|-------------------|
| 100 plays in hour 1 | Triggers "rising" signal, boosted in genre chart |
| 1,000 plays over 7 days | Treated as slow organic growth, minimal boost |
| 50 plays/day consistently | Read as healthy steady account, not chart-worthy |

**How to engineer a velocity spike:**
- Release all repost network partners simultaneously (within 1–2 hour window)
- Post to all social channels the moment the track goes live
- Send a "pre-launch" DM to your top 10 engaged followers asking them to listen immediately
- Pin a comment on the track before it goes public so the CTA is visible from minute zero

**The velocity decay curve:** The algorithm boost from a velocity spike lasts roughly 48–72 hours. After that, the track settles into normal organic distribution. This is why you need a new velocity event (repost from a big account, social post going viral) to revive an old track.

---

## 9. Dead Track Recovery

A "dead" track has under 200 plays and no engagement activity for 30+ days. Recovery options:

| Method | Effort | Expected Lift |
|--------|--------|--------------|
| Repost from your own account | 1 click | 10–20% of followers see it again |
| Update title (add year, tweak wording) | 5 min | Triggers re-indexing, appears in search again |
| Refresh all 5 tags | 5 min | Re-indexes in search, may appear in new autocomplete results |
| Add it to a new playlist | 2 min | Playlist listeners discover it |
| Pitch to a fresh curator | 30 min outreach | Potential 500–2K play spike |
| Embed on external site | 20 min | New traffic source, counts toward plays |
| Social post (waveform video) | 15 min | Drives external traffic back to dead track |

**Never delete a track with any plays** unless the audio quality is embarrassing. Even 50 plays is catalog history. Low-performing tracks can be moved to a "Vault" playlist where they accumulate slow organic plays without cluttering your main feed.

---

## 10. Account Age and Authority

SoundCloud's ranking algorithm treats account history as a trust signal.

**Older accounts with:**
- Consistent upload history (no 6-month gaps)
- Prior high-performing tracks
- Accumulated followers from organic activity

...rank higher in search and appear more in Suggested Tracks compared to new accounts with identical content.

**For new accounts:** The first 90 days are slower by design. The algorithm needs behavioral data to classify your genre, audience, and content quality. Expect search ranking to be suppressed for the first 30–60 uploads.

**Authority-building actions:**
- Never delete tracks from your history (each track is a catalog data point)
- Maintain upload consistency — accounts that upload regularly rank better than bursty accounts
- Older reposts that gained traction contribute to your authority score permanently

---

## 11. Shadowban Signals

SoundCloud does not announce penalties, but certain behaviors reduce algorithmic reach:

| Behavior | Risk Level | Notes |
|----------|-----------|-------|
| Following/unfollowing at volume rapidly | High | Triggers bot detection; reduces feed reach |
| Mass liking sessions (100+ likes in minutes) | Medium | Can flag as automated behavior |
| Buying fake plays | Very High | SC detects traffic pattern anomalies; can suspend account |
| Uploading copyrighted material | Very High | DMCA claim = track removal; repeat = account suspension |
| Duplicate tracks (same audio twice) | Medium | SC deduplication may suppress both |
| Keyword stuffing in tags (20 similar tags) | Low | Tags limited to 5 anyway; description stuffing has low but real risk |

**Signs of reduced reach:** Significant drop in plays-per-upload with no change in posting behavior; followers stop seeing your reposts in their feeds; search ranking drops across multiple tracks simultaneously.

**Recovery:** Stop all suspicious behavior for 30 days. Resume normal activity. There is no official appeal process for soft penalties.

---

## 12. The "Related Tracks" Section

The related tracks panel (shown next to or below a playing track) is one of the highest-traffic discovery surfaces on SoundCloud. Listeners who finish a track often click something from this panel.

**How SoundCloud selects related tracks:**
- Genre and subgenre match
- Tag overlap (sharing 2+ tags with the playing track)
- Engagement rate of the related track (higher engagement = more likely to appear)
- Account authority of the related track's producer
- Whether the related track appears in playlists alongside the current track

**How to appear in related tracks of popular tracks:**
1. Tag your tracks identically to the popular track you want to appear next to
2. Get your track added to playlists that already contain that popular track
3. Build enough plays/engagement that your track's quality score is competitive with the popular track's neighborhood

---

## 13. Notification Triggers

Understanding what sends notifications lets you engineer engagement:

| Action | Notification Sent To |
|--------|---------------------|
| You upload a track | All your followers (feed + push notification if enabled) |
| You repost a track | All your followers (feed insertion, no separate push) |
| You like a track | Track owner only |
| Someone comments on your track | You |
| Someone reposts your track | You |
| Someone follows you | You |
| You add a track to a playlist | Playlist followers if public |

**Implication:** Uploads generate the strongest notification signal (push notifications). Reposts reach your followers in their feed but don't send a push. This means your upload day is your highest-notification day — schedule it when followers are most active (evenings, Friday).

---

## 14. Cross-Genre Discovery

SoundCloud's genre system uses a primary genre plus tags to place you in adjacent discovery feeds.

**Tactics for cross-genre reach:**
- Set primary genre to your exact subgenre (e.g., "Afro House") not just "Electronic"
- Use tags from adjacent genres: if you make afro house, include "afrobeats" and "melodic house" tags
- Create playlists that mix your genre with adjacent ones — playlist listeners who discover you through a mixed playlist expand your genre footprint
- Collab with producers in adjacent genres — their followers see your name in the track title

**Genre bridge tags for house/trap dancehall:**
- Afro House bridges to: Afrobeats, Deep House, Organic House
- Trap Dancehall bridges to: Dancehall, Trap, Reggaeton, Afrobeats

---

## 15. Metadata Refresh — Re-Indexing Bump

SoundCloud re-indexes a track's search ranking when its metadata is updated.

**The hack:** Edit an old track's title, tags, or description → SC re-indexes it within 24–48 hours → the track gets a brief "freshness" signal in search.

**What to change:**
- Add or update the year in the title (change "2024" to "2025")
- Add one new trending tag relevant to your genre
- Expand the description with 2–3 new keyword sentences
- These are cosmetic changes that do NOT require a re-upload

**Limit:** Do not refresh the same track more than once per 30 days. Frequent metadata cycling can trigger the duplicate/spam detection that suppresses tracks.

---

## Algorithm Summary Cheat Sheet

| Priority | Action | Frequency |
|----------|--------|-----------|
| 1 | Coordinated repost launch within 2h of upload | Every upload |
| 2 | Accurate genre + all 5 tags + keyword title | Every upload |
| 3 | Hook within first 15 seconds | Every track |
| 4 | Reciprocal comment engagement | Daily |
| 5 | Metadata refresh on underperforming old tracks | Monthly |
| 6 | Curator playlist placement | Weekly outreach |
| 7 | External embeds for traffic diversification | Weekly |
