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
