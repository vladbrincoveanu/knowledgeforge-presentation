# KnowledgeForge — Cold-Approach Deck Rationale

The deck (`slides.md`, 11 slides, tahta `boardroom`) is engineered to **earn a 20-minute call** — not to close, not to explain everything. Three thinkers shape it. The persuasion is *invisible to the audience* (it lives in slide structure + speaker-note comments), because technical buyers reject visible tactics.

## The three lenses

**Charlie Munger — inversion, simplicity, lollapalooza.**
- *Inversion:* what kills a cold deck? Talking about us, overload, no hook, no proof, a big ask. So: their world first (cover, gap), one idea per slide, one catch, real proof, a tiny ask.
- *Simplicity:* every slide carries a single idea; the "how it works" is 4 steps, no deep dive.
- *Lollapalooza:* the **same architecture model** pays off in several directions at once — engineers, AI agents, executives, audit/security, cost. Multiple congruent forces → the buyer tips. Made explicit on the bridge slide, not just in a comment.

**Robert Cialdini — the six weapons** (one per job, never named on-screen):
- Liking (cover, gap) · Loss-aversion/Scarcity (stats, offer) · Authority (ISO/IEC/IEEE 42010 conformance, solution demo, mechanism) · Social proof (proof slide + standard grounding) · Reciprocity (free map) · Commitment/Consistency (one small repo).

**Mohnish Pabrai — cloning + Dhandho.**
- *Cloning (the frame, not a slide):* don't invent terminology, adopt a proven one. The output is framed as an **architecture description conforming to ISO/IEC/IEEE 42010:2022** — the international standard for describing the architecture of software, systems, and enterprises — instead of internal jargon (the old "C4" label). Cloning established credibility is zero-invention-risk. (Palantir's org-wide ontology / digital twin is a fair *verbal* analogy for the ambition — humans and AI reasoning over one model — but never a claim of affiliation, and no longer a slide.)
- *Dhandho / "heads I win, tails I don't lose much" (close):* frame the buyer's decision as an asymmetric bet — tiny downside (one repo, minutes, free, data stays theirs), big upside (a live map of the whole estate). They're confusing **risk** (none) with **uncertainty** (is it good? — see for yourself).

## Palantir's marketing essence — channeled, not named

The deck steals Palantir's go-to-market *soul* without naming them (naming a polarizing, enterprise/defense brand in a cold email reads as overreach and invites "you're not Palantir"):
- **Own a concept.** Palantir owns capital-O "Ontology". KnowledgeForge owns **"the operating picture of your software"** — what it *does* — repeated at the three anchor points (cover, solution, close). ISO/IEC/IEEE 42010 is the *credential* (what it formally is); "operating picture" is the *concept* (what it gives you).
- **Gravitas over features, measured.** Raise the stakes and own the concept, but keep the sharp, concrete voice — confident, not grandiose (credible in an inbox).
- **The disruption contrast, unnamed.** Palantir proved the digital-twin model at nation-scale over 18-month, eight-figure deployments. The solution-slide caption lands it without the name: *"What took institutions years and eight figures now builds itself from your source, in minutes."* That is the Pabrai clone-and-strip-the-cost move stated as consequence.
- **Show, don't tell.** Lead with the real product proven cold (slide 4, merged demo+proof); the visual is the argument.

## Why ISO/IEC/IEEE 42010 is the spine (not decoration)

The standard's core structure — **one architecture description → many views → each view serves one stakeholder's concerns** — is *exactly* the deck's promise: one model, read by leadership, engineers, and AI agents. So the standard names what the deck already claims, and lends international authority.

The standard's central tenet — *no single diagram serves every stakeholder* — is turned into the **differentiator**: hand-drawn diagrams give you one view (insufficient by the standard); KnowledgeForge generates the whole description and projects a view per stakeholder. That is the bridge slide's argument.

## Slide-by-slide intent (11 slides)

| # | Slide | Job |
|---|-------|-----|
| 1 | "Nobody can draw your architecture. Your code already did." | The hook — inversion + curiosity. |
| 2 | Business & engineering stopped speaking one language | Name the core wound (the bridge thesis). |
| 3 | 2026 reality — 30% / 3mo / 0 / 60% | Loss aversion, then the turn (1 good stat). |
| 4 | The solution, proven cold — merged demo+proof (chips + screenshot + 42010 caption) | Authority by demonstration + social proof in one beat; the demo IS the proof (Munger fewer-bigger). The moment that earns the call. |
| 5 | One graph, one language, every stakeholder's view (exec / eng / AI) | The bridge — spined on ISO/IEC/IEEE 42010: one description, three views, three stakeholders. |
| 6 | Curated context for agents (vs raw repo) | Dev self-interest; tokens are the *side effect*, not the headline. |
| 7 | Exec cockpit — who's building what, risk, KPIs, connectors on the architecture map | Executive self-interest (other half of the lollapalooza). |
| 8 | What it's worth (compare) | ROI against budget lines they own. |
| 9 | How it works (4 steps) | Authority by simplicity. |
| 10 | Enterprise-grade security (ISO 27001 / SOC 2 Type II, deploy-anywhere, GDPR/EU) | Objection-handling before the ask — clears the "can we trust them with our code?" trust wall for both the repo offer and enterprise procurement. |
| 11 | "Heads you win, tails you lose nothing" → book the call | Dhandho asymmetry + reciprocity + commitment + scarcity, now with **liking** (founder-empathy: "we couldn't answer these about our own systems either") + **authority** (Cialdini admit-a-small-weakness: "we're early… if you run more than a handful of services, this is for you"). |

**Cialdini audit (vs the book's 7 levers), 2026-07-01:** 5/7 strong, honesty-clean. Contrast, reciprocation (free map = the standout), commitment, authority (ISO 42010 + slide-11 certs), scarcity — all covered. **Social proof is the one real gap** (pre-launch, no logos); do the honest max (founding-cohort framing) and add real named logos/quotes as startups convert — gate enterprise (Phase 2) on 2–3. Never fabricate (the book's meta-lesson).

## Honesty / before you send

- **Slide 3:** `30%` — cited (Science 2026, 30M commits: ~1/3 of new US code AI-assisted; corroborated 26.9%, 4.2M-dev study). The viral `41%` is debunked (Copilot-only extrapolation), do not revert. `60%` — inside Microsoft GraphRAG's published 26–97% fewer-tokens range; swap in own measured bench when ready. `0` is rhetorical.
- **Slide 4:** "conforming to ISO/IEC/IEEE 42010" must stay defensible — the model maps to the standard's stakeholder/view structure; do not overclaim formal certification.
- **Slide 5:** the credibility rests on the standard, not on authoring it. Keep "built on / grounded in the standard", never "we wrote the standard".
- **Slide 5 / 7:** agent-context claims are roadmap-framed (directional).
- **Slide 7:** panels, connectors, custom KPIs are partly roadmap ("we could start with") — confirm what is live before presenting.
- **Slide 10:** ISO 27001 / SOC 2 Type II / EU-hosting / on-prem stated as fact per founder confirmation (real/live). If any lapses, reword to "in progress / built to controls" — false certs fail enterprise due diligence and break the deck's honesty rule.
- **Slide 4 (merged):** ensure the screenshot IS a genuine cold run (or swap in the real Mastodon run + node/edge counts + wall-clock) so every proof chip is literally true of the image.
- **Slide 11:** the founding-customer scarcity must be **true** (Cialdini: false scarcity, once caught, destroys trust).

## Build

`cd KnowledgeForge && pnpm dev` (or `npx slidev build`). `npx tahta-lint slides.md` must stay clean. Logo: `public/logo-light.png` (white wordmark + teal mark, for the dark theme). Architecture image: `public/graph-architecture.png`.
