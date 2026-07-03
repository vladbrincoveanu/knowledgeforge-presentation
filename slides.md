---
theme: slidev-theme-tahta
title: Nobody can draw your architecture. Your code already did.
info: |
  KnowledgeForge, client pitch.
  A living map of your software, read by your engineers, your executives, and your AI agents.
themeConfig:
  variant: boardroom
  accent: "#F6AE31"
  lang: en
  logo: /logo-amber.svg
transition: slide-left
layout: cover
kicker: For the people who answer for the system
subtitle: The operating picture of your software, generated from the source, read the same way by your engineers, your executives, and your AI agents.
---

<!-- HOOK (Munger inversion + curiosity): open on a provocative truth about THEIR world, not our logo. Nobody can draw the whole architecture, but the code already encodes it. The job of this deck is to earn a 20-min call, not to explain everything. -->

---
layout: columns
kicker: The status quo
title: The business and the engineering floor <span class="accent2">stopped speaking the same language.</span>
columns:
  - title: "On the ground, your engineers…"
    items:
      - "Can't see what breaks downstream when they change a service"
      - "Onboard in months, nobody can point to the whole system"
      - "Rebuild what already exists on another team"
      - "Now inherit AI-written code no one ever mapped"
  - title: "In the boardroom, you can't answer…"
    items:
      - "What does our engineering org actually run?"
      - "Which systems does this security issue touch?"
      - "Where does sensitive data flow, for the audit?"
      - "What's business-critical, and who owns it?"
---

<!-- CIALDINI Liking + pain. The core wound = the broken connection between the business side and the engineering side. Show we feel it at BOTH altitudes. AI codegen widens the gap faster than anyone maps it. -->

---
layout: stats
kicker: The 2026 reality
title: Three costs compounding. <span class="accent2">One lever that pays.</span>
stats:
  - { value: 30, unit: "%", label: "of new code is AI-written, and no one mapped it", icon: "lucide:bot", tone: bad }
  - { value: 3, unit: mo, label: "to onboard an engineer into an unmapped codebase", icon: "lucide:user-plus", tone: bad }
  - { value: 0, label: "real-time view leadership has of what's actually shipping", icon: "lucide:eye-off", tone: bad }
  - { value: 60, unit: "%", label: "fewer tokens for sharper answers, curated context not the whole repo", icon: "lucide:trending-down", tone: good }
---

<!-- CIALDINI loss aversion (3 bad) → the turn (1 good) = self-interest hook into the rest.
SOURCES (verified 2026-07-01): 30% = peer-reviewed Science study (2026, 30M GitHub commits): ~1/3 of new US code AI-assisted by early 2025; corroborated by the 4.2M-developer empirical study (Nov 2025–Feb 2026): 26.9% AI-authored production code. Talk-track kicker if asked: Google self-reports 75% of new code AI-generated (Pichai, Apr 2026). Do NOT use the viral "41%", it's a Copilot-only extrapolation, debunked.
60% = inside Microsoft GraphRAG's published 26–97% fewer-tokens range (graph-curated vs raw context); the "~" stays until we swap in our own measured benchmark. 0 is rhetorical. -->

---
layout: diagram
kicker: The solution, proven cold
title: We turn your repos into your <span class="accent2">operating picture.</span>
---

<div class="proof-strip">
  <span>A multi-service codebase, never seen before</span>
  <span>Full model in <b>one pass</b></span>
  <span>Owners · tech stack · risk · compliance per node</span>
  <span><b>Ask any node</b> in plain language</span>
</div>

<Figure src="/graph-architecture.png" alt="KnowledgeForge architecture description" caption="The operating picture of your software, conforming to <a href='https://www.iso.org/standard/74393.html' target='_blank'>ISO/IEC/IEEE 42010</a>, the international standard. What took institutions years and eight figures now builds itself from your source, in minutes." />

<!-- SOLUTION + PROOF MERGED (was two app slides; demo IS the proof, Munger fewer-bigger, show-don't-tell once and devastatingly). CIALDINI authority by demonstration + social proof + Pabrai clone-a-proven-frame. Full-width Figure, no crop, no text-over-image. ISO/IEC/IEEE 42010 per Iulia grounds the output in the international standard. BEFORE SENDING: make sure the screenshot IS a genuine cold run (or swap in the real Mastodon run + node/edge counts + wall-clock time) so every chip is literally true of the image shown. -->

---
layout: feature
kicker: Why one diagram was never enough
title: One graph. One language. <span class="accent2">Every stakeholder's view.</span>
features:
  - { icon: "lucide:briefcase", title: Your leadership, desc: "the executive view, what we run, what's at risk, what this CVE touches, in plain business terms" }
  - { icon: "lucide:code", title: Your engineers, desc: "the engineering view, what breaks if I change this, down to the file and the dependency" }
  - { icon: "lucide:bot", title: Your AI agents, desc: "the machine view, curated context pulled straight from the model, sharper output, fewer tokens" }
---

<!-- THE BRIDGE = the core promise, now spined on the standard. One model, three views, three stakeholders, exactly what ISO/IEC/IEEE 42010 prescribes: no single diagram serves everyone, so you need one description projected into a view per stakeholder's concerns. That is the differentiator, hand-drawn diagrams give you one view; we generate the whole description. MUNGER lollapalooza: the same model pays off for business + engineering + agents at once. -->

---
layout: vs
kicker: For the developers
title: Your agents are only as good as <span class="accent2">the context you feed them.</span>
label: vs
left:
  title: Context from the raw repo
  items:
    - "Greps blindly, dumps whole files"
    - "Noisy and partial, often the wrong slice"
    - "Weak on cross-repo links and business meaning"
    - "More guessing, more hallucination"
    - "And it burns tokens doing it"
right:
  title: Context from your graph
  items:
    - "The exact subgraph for the task, code and business"
    - "Owners, dependencies, data flow, intent"
    - "Curated structure → sharper, grounded answers"
    - "Works on code AND business questions"
    - "Side effect: ~60% fewer tokens, more AI on the same plan"
---

<!-- CIALDINI authority (mechanism) + self-interest. LEAD with context QUALITY, graph-curated context beats raw context on code AND business questions. Token/cost saving is the SIDE EFFECT (cheaper AI, more usage per plan), never the headline. Roadmap framing; 60% = target/measured. -->

---
layout: panels
kicker: For the executive floor
title: Leadership gets a cockpit, <span class="accent2">not a status meeting.</span>
panels:
  - { icon: "lucide:users", title: "Who's building what", body: "activity and ownership per service, see where the effort actually goes" }
  - { icon: "lucide:shield-alert", title: "Where the risk is", body: "compliance, security, stale or abandoned services, flagged on the map" }
  - { icon: "lucide:gauge", title: "The KPIs you choose", body: "pin the metrics that matter to you, read straight off the architecture model" }
  - { icon: "lucide:plug", title: "Plugs into your stack", body: "connectors to the tools you already run, you steer what comes first" }
---

<!-- EXEC self-interest (the other half of the lollapalooza). The same architecture map that feeds engineers and agents also gives leadership a live overview: headcount, activity, risk, and their own KPIs. ROADMAP: panels / connectors / custom KPIs are "we could start with", frame as direction, confirm what's live before sending. -->

---
layout: compare
kicker: What it's worth to you
title: The same work, <span class="accent2">a fraction of the time.</span>
columns: [What you do today, Manual way, With KnowledgeForge, Δ]
rows:
  - { metric: Audit & compliance prep, before: weeks, after: about a day, delta: "~10× faster" }
  - { metric: Onboard a new engineer, before: months, after: days, delta: "" }
  - { metric: Architecture diagram, before: "hand-drawn, stale", after: "auto, always current", delta: "" }
  - { metric: "Blast radius of a new CVE", before: days of digging, after: one query, delta: "" }
  - { metric: AI agent context, before: raw repo dump, after: curated subgraph, delta: "sharper + ~60% fewer tokens" }
---

<!-- CIALDINI self-interest / ROI. Outcomes tied to budget lines they already own: audit, onboarding, security, and the AI bill. Directional, roadmap-framed where not yet measured. -->

---
layout: steps
kicker: How it works
title: Point it once. Then it <span class="accent2">runs itself.</span>
steps:
  - { title: Point it at your repos, desc: "GitHub URL or local folder, public or private, one repo or your whole estate", icon: "lucide:git-branch" }
  - { title: It builds the graph, desc: "parses the source into a standards-based architecture description, with owner and risk on every node", icon: "lucide:workflow" }
  - { title: It stays current, desc: "re-extracts on every commit, PR and redeploy, the map never drifts from reality", icon: "lucide:refresh-cw" }
  - { title: Everyone queries it, desc: "people in plain language, agents in the same ontology, one source of truth", icon: "lucide:messages-square" }
---

<!-- MUNGER simplicity. Four steps, no deep dive. Step 4 lands the human + agent shared-query payoff. -->

---
layout: feature
kicker: For the security review
title: Enterprise-grade security, <span class="accent2">on your terms.</span>
features:
  - { icon: "lucide:badge-check", title: "ISO 27001 & SOC 2 Type II", desc: "independently audited, the certifications enterprise procurement asks for" }
  - { icon: "lucide:server", title: "Deploys in any infrastructure", desc: "managed, your own cloud, or fully on-premises" }
  - { icon: "lucide:lock", title: "GDPR-compliant, EU-hosted", desc: "hosted in the EU, your data stays yours" }
---

<!-- ENTERPRISE TRUST, objection-handling right before the ask. Answers "can we trust them with our code?", the wall for both the repo offer and enterprise procurement (grill Q1a/Q2). Certs stated as fact per founder confirmation (real/live). Last beat before the CTA = "it's safe." -->

---
layout: end
title: See your own operating picture. Heads you win, tails you lose nothing.
subtitle: We built this because we couldn't answer these questions about our own systems either. Send us one repo, we map it free and walk you through it on a 20-minute call. No commitment, and worst case you're out the 20 minutes. We're early, and picking a few founding customers this quarter, if you run more than a handful of services, this is for you.
contact: iulia@knowledge-forge.com · vlad@knowledge-forge.com
---

<div class="site-cta">
  <a href="https://www.knowledge-forge.com" target="_blank" rel="noopener">
    <svg width="13" height="13" viewBox="0 0 28 28" fill="none" aria-hidden="true">
      <polygon points="14,2 26,8 26,20 14,26 2,20 2,8" stroke="currentColor" stroke-width="1.5" fill="none" />
      <circle cx="14" cy="14" r="2.5" fill="currentColor" />
      <line x1="14" y1="2" x2="14" y2="11.5" stroke="currentColor" stroke-width="1" opacity="0.6" />
      <line x1="14" y1="16.5" x2="14" y2="26" stroke="currentColor" stroke-width="1" opacity="0.6" />
      <line x1="2" y1="8" x2="11.5" y2="12.5" stroke="currentColor" stroke-width="1" opacity="0.6" />
      <line x1="16.5" y1="15.5" x2="26" y2="20" stroke="currentColor" stroke-width="1" opacity="0.6" />
      <line x1="26" y1="8" x2="16.5" y2="12.5" stroke="currentColor" stroke-width="1" opacity="0.6" />
      <line x1="11.5" y1="15.5" x2="2" y2="20" stroke="currentColor" stroke-width="1" opacity="0.6" />
    </svg>
    <span>www.knowledge-forge.com</span>
    <span class="arrow" aria-hidden="true">&rarr;</span>
  </a>
</div>

<style scoped>
.site-cta {
  display: flex;
  justify-content: center;
  margin-top: 1.4rem;
}
.site-cta a {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.5rem 1.1rem;
  border: 1px solid var(--accent);
  border-radius: 999px;
  color: var(--accent);
  font-family: var(--font-mono, 'Geist Mono', monospace);
  font-size: 0.78rem;
  font-weight: 600;
  letter-spacing: 0.06em;
  text-decoration: none;
  transition: background 0.18s ease, color 0.18s ease;
}
.site-cta a:hover {
  background: var(--accent);
  color: #0b0d12;
}
.site-cta .arrow {
  transition: transform 0.18s ease;
}
.site-cta a:hover .arrow {
  transform: translateX(3px);
}
</style>

<!-- PABRAI Dhandho: frame the buyer's decision as an asymmetric bet, tiny downside (one repo, minutes, free), big upside (a live map of the estate); they're confusing risk with uncertainty. CIALDINI reciprocity (free map) + commitment (one small repo) + scarcity (founding slots). The CTA is the COLD-APPROACH GOAL: earn the 20-minute call, not close the sale. Website surfaced as a clickable button now the deck is hosted/shareable; emails stay in the contact line. -->
