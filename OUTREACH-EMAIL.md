# KnowledgeForge — cold outreach (v2, offer-(c)-first)

Decisions baked in from the grill:
- **Offer (c): public-repo-map FIRST.** No "send us your code" ask on first touch — zero trust wall.
  The private-repo map + 20-min call is the *upsell*, not the opener.
- **Sequence: startups first** (they act cold → give logos/proof), enterprise second with that proof.
- **Deliver a LINK to a live/interactive map, not a PDF attachment.** Deck PDF = leave-behind.
- **Hybrid by tier:** shortlist gets their *real* map in email 1; volume gets a teaser + offer.
- Trust-closer available: ISO 27001 / SOC 2 Type II / EU-hosted / on-prem (real).
- Sender: `contact@knowledge-forge.com` (see deliverability note re: apex domain).

---

## A — SHORTLIST (≤~50 targets you truly want; map their public repo BEFORE emailing)

**Subjects (A/B top two):**
1. I mapped {Company}'s architecture — take a look
2. The operating picture of {Company}'s software
3. {repo} → a living map, in 3 minutes

**Preheader:** Every service, dependency, and owner — straight from your source. Live map inside.

**Body (~100 words):**

Hi {Name},

I pointed KnowledgeForge at {Company}'s `{public-repo}` and it built the **operating picture** of it — every service, dependency, and owner, straight from the source. Live, interactive map: **{link}**

Nobody drew it. It took a few minutes, and it re-builds on every commit — so it never goes stale. Your engineers, your execs, and your AI agents all read the same map (it conforms to ISO/IEC/IEEE 42010, the international standard for architecture description).

We built KnowledgeForge because we couldn't answer these questions about our own systems either. If it's useful, I'll map a private repo of your choice and walk your team through it on a 20-minute call. SOC 2 Type II, ISO 27001, EU-hosted — your data stays yours.

Worth 20 minutes?

— Iulia & Vlad, KnowledgeForge · knowledge-forge.com

**P.S.** Taking a few founding customers this quarter.

---

## B — VOLUME (teaser + offer; map on reply)

**Subjects:**
1. What breaks if you change that service?
2. Your architecture diagram is already out of date
3. A living map of {Company}'s codebase — free

**Preheader:** Reply with one repo. We map it, you keep it. No call unless you want one.

**Body (~90 words):**

Hi {Name},

Nobody at {Company} can draw your whole architecture from memory — your code already encodes it. KnowledgeForge turns any repo into its **operating picture** in minutes: every service, dependency, and owner, straight from the source, current on every commit.

Here's what it did to `{well-known OSS repo in their stack}`: **{link}**

We built it because we couldn't answer these questions about our own code either. Reply with one public repo and I'll send back the same map of yours — free, no call, nothing leaves the public repo. If it lands, we'll talk.

— Iulia & Vlad, KnowledgeForge · knowledge-forge.com

---

## Follow-up (no reply, ~4 days later, same thread)

> Quick nudge — want me to just map one of your public repos and send the graph back? No call, takes me 3 minutes. Curious what you'd make of it.

## Enterprise variant (Phase 2, after startup proof exists)

- Swap the hook to the boardroom pain (what do we run / risk / audit / CVE blast-radius) — deck slides 7–9.
- Lead the trust close harder: **ISO 27001, SOC 2 Type II, GDPR, EU-hosted, on-prem** (deck slide 11).
- Expect champion-led nurture, not a cold 20-min call. Attach nothing; link a hosted map + the deck.

## Send hygiene / legal

- **Domain:** you chose `contact@knowledge-forge.com` (apex). Works, but cold volume can dent the apex's reputation → your normal business mail. If you scale past ~20–30/day, move cold sends to a **separate domain** (e.g. `try-knowledgeforge.com`) and keep the apex for replies/warm.
- SPF/DKIM/DMARC set; 2-week warmup; plain text; **one link**; personalize the first line for real.
- **GDPR (EU):** legitimate-interest basis for B2B, real sender identity, and a **one-line opt-out** ("Not relevant? Reply 'no' and I won't follow up.") in every cold mail.
- One CTA per email. Attachment (if any) named `KnowledgeForge-overview.pdf` — but prefer a link.
