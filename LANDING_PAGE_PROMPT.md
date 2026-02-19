# Landing Page Generator Spec — Hafiz Pro (Prompt Pack)

Use this document as a **single source of truth** to generate a modern, responsive landing page for a Quran memorization app inspired by **Hafiz Pro**.

This is intended to be pasted into another AI / project to produce a similar high-quality landing page.

---

## 1) Product Summary (what the app is)

**Product name:** Hafiz Pro

**One-liner:** Master the Quran, one Ayah at a time.

**Purpose:**
Hafiz Pro is a Flutter application designed to help Muslims test and improve their Quran memorization skills through interactive, audio-based testing.

**Core features to highlight on the landing page:**
- Test memorization using **multiple modes**:
  - **Test by Surah**
  - **Test by Juz**
  - Random testing across the Quran
- **Audio playback** with multiple reciters
- **Playback controls** (play/pause/seek/speed)
- **Background playback**
- **Loop modes** for repetition
- **Progress tracking** / continue from last read
- **Modern UI** with Arabic typography
- **Responsive design** (mobile + desktop)
- Settings for reciter/autoplay/preferences

**Target user:** Muslims memorizing Quran (Hifz), students, and anyone improving recitation and recall.

**Tone / vibe:**
- Modern, calm, premium
- Spiritual but not overly ornate
- Confident, minimal, and respectful
- Quranic feel: gentle, luminous, serene

---

## 2) Landing Page Goal

Create a landing page that:
- Communicates the value proposition quickly
- Feels **modern and app-like** (premium UI)
- Has a **subtle Islamic/Quranic aesthetic**
- Is **fully responsive**
- Works as a **standalone HTML file** (no build tools required)

Important: If the project is a Flutter web app, **do NOT replace `web/index.html`** (it boots Flutter). Prefer creating a separate file like `web/landing.html`.

---

## 3) Required Sections (structure)

### A) Top Navigation
- Brand (logo + name)
- Links: Features, How it works, Why
- CTA buttons:
  - Primary: “Open App” / “Launch Hafiz Pro”
  - Secondary: “Get Started” / “See Features”

### B) Hero Section
- Headline (modern, large):
  - Example: “A calm, modern way to memorize the Quran.”
- Short description (2–3 lines)
- Arabic ayah/phrase for spiritual feel (rendered with Arabic font)
  - Keep it respectful and minimal
- CTA row
- Small meta badges (Web + Mobile, Verse-by-verse audio, Distraction-free)

### C) Features Section
- 3–6 feature cards
- Each card: icon + title + short description

### D) How It Works
- Step-based explanation (3–4 steps)
- Keep copy short

### E) Why / Trust Section
- One or two Quranic quotes (Arabic + English translation)
- Additional reassuring copy: calm, consistency, gentle repetition

### F) Footer
- Copyright
- Quick links

---

## 4) Design Requirements

### Visual Style
- Dark, premium background with subtle gradients and soft glows
- Glassmorphism-style cards (semi-transparent, blurred if possible)
- Rounded corners (14–20px)
- Subtle borders (white at ~8–15% opacity)
- Soft shadows (not harsh)

### Islamic/Quranic Feel (without clichés)
- Arabic typography for quotes (e.g., Amiri)
- Gentle green/teal accents (emerald/teal)
- Optional gold accent sparingly
- Avoid heavy geometric patterns; keep it subtle if used

### Typography
- Latin: `Inter` (or similar modern sans)
- Arabic: `Amiri` (or similar serif Arabic font)

### Responsiveness
- Mobile-first safe
- Navigation collapses/hides on small screens
- Hero becomes single-column under ~940px
- Cards stack nicely

### Accessibility
- Good contrast
- Real text (no text baked into images)
- Semantic HTML

---

## 5) Technical Constraints

Generate a **single HTML file** with:
- Inline CSS (preferred) OR a linked CSS file (optional)
- No heavy frameworks required
- Optional: Google Fonts CDN
- Use relative asset paths where possible

If icons exist, assume:
- `web/icons/icon-192.png`
- `web/icons/icon-512.png`

Use them for:
- Favicon
- Apple touch icon
- Branding image in the navbar

---

## 6) Content Guidelines (copy suggestions)

### Headline options
- “Master the Quran, one Ayah at a time.”
- “A calm, modern way to memorize the Quran.”
- “Focused practice for lasting memorization.”

### Microcopy keywords
- calm
- consistent
- focused
- gentle repetition
- distraction-free
- recitation
- recall

Avoid:
- Overpromising
- Overly salesy tone

---

## 7) Deliverables

The AI should output:
- `landing.html` (or similar)
- Uses the product name “Hafiz Pro”
- Includes all sections above
- Is visually modern and responsive

Optional nice-to-have:
- Subtle decorative background pattern using CSS
- Small animated hover effects (buttons/cards)

---

## 8) Example “Open App” Link Strategy

If Flutter app lives at the same root:
- “Open App” can link to `./`

If you prefer landing at `/` and Flutter app at `/app/`:
- “Open App” should link to `./app/`

(Adjust based on hosting.)
