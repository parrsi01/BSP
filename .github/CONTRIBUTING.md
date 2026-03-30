# Contributing Guide — BSP Repository

For the 4-person BSP team. This repo is documentation and resources only — no audio files live here.

---

## Getting Started

### Clone the Repo
```bash
git clone https://github.com/your-org/bsp.git
cd bsp
```

### Prerequisites
- Git installed: [git-scm.com](https://git-scm.com)
- A markdown editor (VS Code recommended — install the "Markdown Preview Enhanced" extension)
- Access to the BSP team Google Drive for audio assets

---

## Folder Structure Rules

```
bsp/
├── README.md            ← Overview only; update when adding new files
├── AGENTS.md            ← AI tools documentation
├── loops/               ← Sample and loop source information
├── tutorials/           ← DAW-specific production tutorials
├── production/          ← Sound design, mixing, arrangement
├── marketing/           ← Selling, licensing, social media
├── team/                ← Internal workflow, checklists
├── graphics/            ← Visual design guides
├── resources/           ← Theory, plugins, outreach
└── .github/             ← Repo configuration and this file
```

### Rules
1. **No binary files in this repo.** Audio files, images, and videos belong in Google Drive. If you want to reference an asset, link to Google Drive.
2. **Documentation goes in the folder that matches its category.** When in doubt: create a new section in an existing file before creating a new file.
3. **README.md must be updated** whenever a new file is added (add it to the Table of Contents).

---

## File Naming Conventions

### Documentation Files
- All caps, underscores, `.md` extension
- Descriptive of content: `SOUND_DESIGN_HOUSE.md` not `notes.md`
- Pattern: `TOPIC_CATEGORY.md` or `TOOL_TOPIC.md`

### Audio Files (in Google Drive — NOT in repo)
```
BSP_[BeatName]_[BPM]_[Key]_[Version].[ext]
```
- BeatName: CamelCase, no spaces
- BPM: numeric (e.g., 126)
- Key: Note + minor/major shorthand (Am, Cmaj, Fm)
- Version: v1, v2, MASTER, TAGGED

**Examples:**
```
BSP_WarmNights_126_Am_v1.wav
BSP_WarmNights_126_Am_MASTER.wav
BSP_WarmNights_126_Am_TAGGED.mp3
BSP_WarmNights_126_Am_STEM_Kick.wav
```

---

## How to Add a New Tutorial

1. **Create a branch:**
   ```bash
   git checkout -b feature/logic-advanced-tutorial
   ```

2. **Create the file** in the appropriate folder:
   ```
   tutorials/LOGIC_ADVANCED_PRODUCTION.md
   ```

3. **Use the standard template structure:**
   ```markdown
   # Tutorial Title

   Brief introduction paragraph.

   ---

   ## 1. Section One

   Content here.

   ---

   ## 2. Section Two

   Content here.
   ```

4. **Update README.md** — add the new file to the Table of Contents under the correct section

5. **Commit:**
   ```bash
   git add tutorials/LOGIC_ADVANCED_PRODUCTION.md README.md
   git commit -m "docs: add Logic Pro advanced production tutorial"
   ```

6. **Open a Pull Request** against `main`

---

## How to Add a New Beat to the Shared Catalog

Beats do not go in the GitHub repo. The process:

1. Produce and finalize the beat (follow quality checklist in `team/WORKFLOW.md`)
2. Export all required files (MASTER.wav, TAGGED.mp3, Stems ZIP)
3. Upload to the **BSP Team Drive** → `00_ACTIVE_PROJECTS/[YourName]/[BeatFolder]/`
4. Move to `01_READY_TO_UPLOAD/` once it passes QC
5. Marketing Lead uploads to BeatStars/Airbit with metadata
6. Marketing Lead moves to `02_UPLOADED/` with a date note
7. Optionally: update a beat catalog spreadsheet in `05_MARKETING/`

---

## Commit Message Format

Follow the **Conventional Commits** format:

```
type: short description (under 72 characters)

Optional: longer explanation if needed.
```

### Types

| Type | Use For |
|------|---------|
| `docs` | Adding or updating documentation |
| `fix` | Correcting an error in existing docs |
| `feat` | New content, new file |
| `refactor` | Restructuring content without changing meaning |
| `chore` | Maintenance (updating links, formatting) |

### Examples
```
docs: add Ableton sidechain compression section
fix: correct BPM range for afro house in theory guide
feat: add artist outreach DM templates
chore: update all BeatStars links to current URLs
refactor: split MARKETING into separate files
```

---

## Branch Naming

| Pattern | Use |
|---------|-----|
| `feature/topic-name` | New content or new file |
| `fix/topic-name` | Correction to existing content |
| `update/topic-name` | Major update to existing content |
| `chore/topic-name` | Maintenance tasks |

**Examples:**
```
feature/email-marketing-guide
fix/fl-studio-bpm-range
update/pricing-strategy-2025
chore/broken-links-check
```

---

## No Large Binary Files in Repo

This is enforced by `.gitignore`. The following file types are blocked from the repo:

```
*.wav
*.mp3
*.aiff
*.flac
*.mp4
*.mov
*.avi
*.psd
*.ai
*.eps
*.zip
*.dmg
*.exe
```

If you need to share a binary asset with the team, **upload it to Google Drive** and paste the share link in the relevant markdown file or in the #resources Discord channel.

---

## Weekly Sync Branch Merges

Every Sunday:
1. All team members merge their active branches to `main` or open PRs for review
2. The person designated for weekly sync (rotate weekly) reviews and merges any open PRs
3. `main` should always reflect the current, agreed-upon state of the documentation

### Before Merging to Main
- [ ] No broken links (check any URLs you added)
- [ ] Correct markdown syntax (preview in VS Code or GitHub)
- [ ] No audio/binary files accidentally staged
- [ ] Commit message follows format above
- [ ] README.md updated if new file was added

---

## Markdown Style Guide

To keep all files consistent:

- **Headings:** H1 for title only, H2 for major sections, H3 for subsections
- **Tables:** Use for anything with 3+ rows of structured data
- **Code blocks:** Use for commands, file paths, naming conventions
- **Bullets:** Use for unordered lists; avoid in places where a table would be cleaner
- **Bold:** For emphasis on critical information only — not decorative
- **Links:** Always format as `[Display Text](url)` — never raw URLs in body text

---

## Questions and Conflicts

For questions about this guide: post in `#general` in the team Discord.

For content conflicts (two people wrote different advice): bring to the weekly meeting — don't just overwrite.
