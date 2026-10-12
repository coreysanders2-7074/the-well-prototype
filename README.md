# The Well — Clickable Prototype

**What it is:** a working prototype of the #1 idea from *THE WELL — 100 Anonymous
First-Contact App Ideas* ("THE WELL — Flagship"): one screen, no signup, no name.
A visitor types their deepest need and receives a personal prayer plus one
scripture matched to their words.

**How to view:** open `index.html` in any browser (desktop or phone). Single file,
no build step, no network needed. Mobile-first (max 430px), dark mode.

**Three themes:** `index.html` is the original (deep navy + gold).
`index-vermilion.html` is the alternate theme — Vermilion `#FA4616` (accent),
Off-White `#F1F1F1` (text), Charcoal `#151515` (base). `index-kensington.html`
follows the Kensington brand guide (§1.4–1.5): Near Black `#1B1A1A` base,
Kensington Orange `#FD5200` accent, Alto `#CFC8C8` muted. Same app in all
three — only palette and fonts differ.

**Fonts (Kensington theme):** Montserrat (Google Fonts) stands in for Museo Sans
— Museo Sans is licensed, not freely available, so the real font needs a copy
from the Communications Department. Noto Serif loads real from Google Fonts and
is used for long-form copy (verse, prayer) per §1.4.2. Outbound (accent font) is
not applied — no licensed file on hand. Note: the Google Fonts CDN means the
Kensington theme makes a font-loading network request; the other two themes
are fully offline.

**How it works (all client-side — the privacy story is real):**
- 3 screens: the ask → the answer (verse + prayer) → pray-it-forward.
- 16 keyword themes (anxiety, grief, loneliness, shame, weariness, healing,
  provision, direction, anger, relationships, addiction, hopelessness, weakness,
  gratitude, crisis, + default) map to a verse (NIV) and a ~60-word prayer.
- Crisis keywords surface a 988 call/text card first. Nothing is stored anywhere
  — no localStorage, no network calls. The "privacy promise" on screen is
  literally true.
- "Pray it forward" ties in idea #3 (Someone Prayed For You) as the loop mechanic.

**Verse/prayer source notes:** all verse texts are NIV, quoted from memory of the
standard text; two are lightly trimmed with ellipsis (Deut 31:6, 1 Cor 10:13).
Before any public ship, spot-check the 16 verses against BibleGateway.

**If Corey wants it built for real, the honest next steps:**
1. Backend: anonymous prayer submission queue + a human/pastoral review layer
   before any "someone prayed for you" notification goes out.
2. Moderation: crisis-language escalation protocol beyond the 988 card.
3. Verse matching: upgrade keywords → embedding similarity over a tagged verse bank.
4. Decide the home: standalone PWA vs. a tab inside a Twlv2 app vs. a link-in-bio
   landing page (cheapest first test: link in bio on @twlv2church).

Built 2026-10-11 as a research-stage prototype. Not a shipped product.

---

## Top 10 prototypes (+ bonus)

Working single-file HTML prototypes of ideas #2–#11 from *THE WELL — 100
Anonymous First-Contact App Ideas*, built 2026-10-11 for Corey's morning review.
Open `apps/index.html` for the launcher (grid of all 10 + bonus), or open any
app folder's `index.html` directly. Same discipline as the flagship: single file,
mobile-first, zero localStorage, zero network calls (except the font-loading
note below), anonymous-first, every button functional.

All apps use the **full Kensington theme** (colors + fonts): Near Black `#1B1A1A`
base, Kensington Orange `#FD5200` accent, `#F5F2EB` text, `#CFC8C8` muted;
Montserrat for UI/headings, Noto Serif for long-form copy — per the Kensington
brand guide (§1.4–1.5, saved at `workspace/user/brand/kensington-brand-guide.md`).
Crisis cards keep their alert-red styling. Note: the Google Fonts CDN means these
apps make a font-loading network request (display only — no user data is sent);
with no network they degrade gracefully to system fallbacks. Museo Sans itself
is licensed, not free — Montserrat is the stand-in.

| # | App | Folder | What it does |
|---|-----|--------|--------------|
| 1 | The Well — Flagship | `index.html` (root) | Type your deepest need → verse + prayer, keyword-matched |
| 2 | 3AM Well | `apps/02-3am-well/` | Guided breathing (4-6, ~60s) → slow chat → verse till morning |
| 3 | Someone Prayed For You | `apps/03-prayed-for-you/` | Simulated prayer notification → pick situation → pray it forward |
| 4 | The Unsent Prayer | `apps/04-unsent-prayer/` | The unsayable prayer → heard → hold 7 days or let go |
| 5 | 7 Days at the Well | `apps/05-7-days/` | 7-night map → nightly question → 60s guided prayer → verse |
| 6 | Prayer Language Quiz | `apps/06-prayer-language/` | 8 questions → Warrior/Whisperer/Journaler/Walker/Weeper result card |
| 7 | Panic to Peace | `apps/07-panic-to-peace/` | "I'm panicking" → 90s breathing pacer + truths → closing prayer; 988 always visible |
| 8 | The Forgiveness Letter | `apps/08-forgiveness-letter/` | Guided letter → release / seal 30 days / burn rituals |
| 9 | Money Peace | `apps/09-money-peace/` | Money stress → prayer + one practical weekly step + verse; no prosperity gospel |
| 10 | The Doubt Room | `apps/10-doubt-room/` | 6 forbidden questions → honest, non-preachy answers + stillness timer |
| + | Detroit Community Resource Hub (bonus) | `apps/11-detroit-resources/` | "What's happening right now?" intake → top-3 urgency-ranked verified resources across 10 need categories; 22 verified listings |

**Resource-listing honesty (app #11):** every listing was verified (name, phone, service) against its official site or a current directory listing via web search on 2026-10-11 — unverified candidates were cut. **Full re-verification against official sites is required before any public launch.** Hours marked "call to confirm" unless verified from the official site.
