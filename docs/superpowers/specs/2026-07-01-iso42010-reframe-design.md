---
title: KnowledgeForge deck — ISO 42010 reframe + mental-model deepening
date: 2026-07-01
status: approved
ui_scope: true
graph_scope: false
test_scope: false
---

# KnowledgeForge deck v2 — ISO/IEC/IEEE 42010 reframe + mental-model deepening

## Source of the change
- Iulia (reviewer): drop "C4" branding; anchor on **ISO/IEC/IEEE 42010:2022** with a link;
  keep the "what's worth to you" slide (her favourite) intact.
- Vlad: think deeper — apply Munger mental models, Pabrai's application of them, and Cialdini's
  influence / cold-approach principles.

## Big idea (approved: "spine + weapon")
ISO/IEC/IEEE 42010 is not a word-swap. Its structure — **one architecture description → many views →
each view serves one stakeholder's concerns** — is *literally* the deck's existing promise
("one graph, three readers: leadership / engineers / AI agents"). So 42010 names what the deck
already claims and lends it international authority.

Tension Iulia flagged ("the standard says no single diagram suffices") becomes a **differentiator**:
- Hand-drawn diagrams / competitors = one diagram → insufficient *per the standard*.
- KnowledgeForge = one live model → per-stakeholder views → *conforms to* 42010.

## Mental-model deepening (surgical, not a rewrite)
- **Munger** — sharpen the *lollapalooza* (one artifact, three stakeholders, aligned incentives →
  nonlinear value) from a hidden comment into on-slide framing.
- **Pabrai** — dropping internal jargon ("C4") for an established international standard *is* Dhandho:
  clone proven credibility, zero invention risk. Close already nails the asymmetric bet — leave it.
- **Cialdini** — (1) Authority ↑ via 42010 citation + link; (2) fill the social-proof gap honestly with
  a credibility line grounded in the team's study of the standard (NOT "we authored ISO"); (3) keep
  reciprocity / scarcity / commitment in the close as-is.

## Approved decisions (via AskUserQuestion, 2026-07-01)
1. 42010 depth: **Spine + weapon** (weave into bridge slide + differentiator; no restructure).
2. Social proof: **Yes** — add an honest credibility line grounded in 42010 study (not fabricated logos).
3. Asset: **Rename** `graph-c4.png` → `graph-architecture.png` (public/ + assets/ + src ref).

## Grill-me guardrails (baked in)
- Credibility phrasing must NOT imply authoring ISO 42010. Use "grounded in / built on the
  international standard" — humble, defensible against Iulia's real thesis work.
- Do NOT overstuff the bridge slide: `feature` layout has no body slot; 42010 framing rides in
  `kicker` / `title` / feature `desc` only.
- Rename is atomic: move both image copies + update the single `src` ref; verify no other live ref.
- Keep 11 slides (Pabrai "few bets"). No net-new slide.

## Change list (modules)

### Module: Solution slide (s4, `default` + Figure)
- **Responsibility:** Establish authority — the product output IS a standards-conforming architecture description.
- **Interface:** `title` (keep punch), body line, `Figure` caption (carries 42010 conformance + "always current" + the "never hand-drawn" differentiator), `src` → `/graph-architecture.png`.
- **Dependencies:** renamed image asset present in `public/`.
- **Size target:** 1 slide.

### Module: Bridge slide (s5, `feature`)
- **Responsibility:** Embody 42010's core — three stakeholders, three views, one model — as the deck's spine.
- **Interface:** `kicker` = the standard's central tenet as a hook ("why one diagram is never enough"); `title` keeps "one language" emotional bridge; three `features` = the three stakeholder views (leadership / engineers / agents) in 42010 vocabulary (stakeholder → concern → view).
- **Dependencies:** none.
- **Size target:** 1 slide, exactly 3 features.

### Module: How-it-works step (s9, `steps`)
- **Responsibility:** Describe the build output in standard terms.
- **Interface:** step 2 `desc` → "an architecture description (ISO/IEC/IEEE 42010): ecosystem, services, internals as views".
- **Size target:** 1 line.

### Module: Close slide (s11, `end`)
- **Responsibility:** Authority + the asymmetric-bet ask, unchanged in structure.
- **Interface:** `subtitle` gets one short honest credibility clause (grounded in the standard); keep reciprocity/scarcity/commitment + contacts.
- **Size target:** 1 slide.

### Module: DECK-RATIONALE.md (project doc)
- **Responsibility:** Keep the design record consistent with the shipped framing.
- **Interface:** replace "C4 graph" / "C4 map" mentions with the architecture-description / 42010 framing.
- **Size target:** 2 edits.

### Module: Asset rename
- **Responsibility:** Purge "C4" from the repo incl. non-visible asset name.
- **Interface:** `git mv public/graph-c4.png public/graph-architecture.png`; same for `assets/`; update `slides.md` `src`.
- **Dependencies:** rebuild `dist/` after.

## Out of scope
- `graphify-out/*` (auto-generated; regenerates on next graphify build).
- "What's worth to you" slide content (Iulia's favourite — untouched).
- Any deck restructure or new slides.

## Verification
- `pnpm`/`npx slidev build` clean, 11 slides.
- Playwright screenshot s4, s5, s9, s11 at boardroom viewport; confirm 42010 link renders + clickable,
  image loads under new name, no "C4" visible, "what's worth" slide unchanged.
- `grep -rin '\bc4\b'` over non-generated files returns only intentional/historical notes.
