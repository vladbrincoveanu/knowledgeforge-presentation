# KnowledgeForge — grilled GTM & strategy (one page)

Output of two grills: Cialdini (influence/mechanics) + Munger (business/strategy). This is the
shared understanding the deck + email are built to serve.

## Strategy (Munger lens)

- **Wedge vs moat.** The repo→map is the **wedge** — commoditizable (LLM + tree-sitter), and that's
  fine; it's the free-sample hook. **Don't defend it.** The **moat** is the per-customer
  **data-gravity flywheel**: more connectors + data → more accurate → better context for agents *and*
  humans → more use → more data. Autocatalysis: nothing below critical mass, self-sustaining above it.
- **Scope = circle of competence.** **Win CODE first** — "the operating picture of your code," AST-grounded,
  defensible. Expand only **code-adjacent** (PRs, incidents, runbooks, tickets) *after* it's a moat.
  Do **not** jump to "all company knowledge" (Glean / Notion / Palantir red ocean, no edge).
- **Moat type = per-customer**, not cross-customer. A cross-customer data network would contradict the
  slide-11 promise (*your data stays yours, on-prem, GDPR*). Per-customer switching cost + product depth
  is honest and consistent.
- **Sell value, not lock-in.** Switching cost is *your* advantage but the buyer's *fear* ("what's our
  exit?"). Pitch the compounding value ("more useful every week as it learns your systems").
- **Vision split.** Knowledge-fabric grand vision → fundraise / warm conversations only. Cold pitch stays
  on the one clear thing: the code map.

## Go-to-market (Cialdini lens)

- **Target — both markets, sequenced.** Phase 1: **startups (Series A–C, 50–300 eng, polyglot, AI-codegen)**
  — they act cold → give logos/proof. Phase 2: **enterprise** with that proof (champion-led, audit/cockpit
  angle, longer nurture). Never one email to both.
- **Buyer / incentive.** **Head of Platform / Eng / Security-owner** — whoever *answers for the system*.
  Personal stake: never be the one caught flat-footed in a CVE, audit, or incident; onboarding that drags.
- **Offer — (c) public-repo-map FIRST.** Map their public repo, send the graph back — **zero trust wall,
  reciprocity given before any ask.** Private-repo + 20-min call = the **upsell**, not the opener.
- **Delivery — hybrid by tier.** Shortlist (~30–50 you truly want): real map as a **live link** in email 1.
  Volume: teaser (their-stack OSS map) + offer on reply. **Link, not attachment.**
- **List / channel.** **GitHub-native** (active ICP public repos → maintainer = lead + map source +
  personalization). **LinkedIn + email**, same "I mapped your repo" hook. Cold sends off a burner domain
  past ~30/day; GDPR opt-out line always.

## Guardrails (Munger: margin of safety + disconfirmation)

- **Reliability is the operational killer.** Never send an **unreviewed** auto-map to a target — one ugly
  map = mere-association blowup. Prove the pipeline on **10 real target repos**, pin the capable LLM model,
  **hand-QA every shortlist map**, kill-before-send. Scale volume only after auto-quality is boring.
- **Pre-committed kill-gate (honor it):** *30 QA'd shortlist maps sent → if <5 replies and <2 calls, the
  wedge/pitch is wrong. Stop, don't scale, re-examine.* Hunt the disproving evidence first (Darwin).

## Influence coverage (Cialdini audit)

Contrast ✅ · reciprocation ✅ (free map = standout) · commitment ✅ · liking ✅ · authority ✅ (ISO 42010 +
certs + admit-a-weakness) · scarcity ✅. **Social proof = the one structural gap** — closes the day you have
2–3 real named logos. Never fabricate.

## Artifacts

- `slides.md` — 11-slide deck (operating-picture concept, ISO 42010 credential, security slide, Palantir
  essence unnamed, full Cialdini stack).
- `OUTREACH-EMAIL.md` — cold email v2 (offer-(c)-first).
- `DECK-RATIONALE.md` — persuasion rationale + honesty log.

## Open / next

- Product reliability **boring** before scaling (offer-(c) depends on it).
- First 2–3 **named logos** → unlocks enterprise Phase 2 + closes the social-proof gap.
- Fresh **PDF export** before first send (the Documents copy is stale).
