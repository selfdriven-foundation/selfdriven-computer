---
name: selfdriven-codes
description: "Build selfdriven.codes — human trust infrastructure for the synthetic reality era. Use when the user mentions selfdriven.codes, out-of-band trust codes, human courier networks, root trust delivery, trust phrases like ORBIT-LANTERN-482, or any work involving the selfdriven.codes platform, API, courier dispatch, code generation, or trust establishment between humans across compromised channels. Also use for content built on the two position papers: 'Out-of-Band Human Trust Establishment in the Age of Synthetic Reality' and 'Human Courier Networks for Root Trust Delivery'."
---

# selfdriven.codes Skill

Build selfdriven.codes properties — the human trust infrastructure layer of the selfdriven Foundation ecosystem. selfdriven.codes generates unique trust-establishment codes, cryptographically binds them to identities and sessions, and delivers them through a distributed network of trusted human couriers.

This skill builds on `selfdriven-ecosystem` (brand, KERI/ACDC, 8 Areas of Focus, Human Conductor model). Always consult that skill in parallel for any selfdriven.codes work — this skill captures only the domain-specific patterns for codes, couriers, and out-of-band trust.

## Core Concept

selfdriven.codes proposes a trust primitive for an era where:

- voices can be cloned,
- faces can be synthesised,
- writing styles can be replicated,
- and every digital channel can be convincingly impersonated.

The platform generates human-readable codes (e.g. `EMBER-RIVER-91`), binds them cryptographically to sessions and identities, and delivers them through independent human courier pathways — outside the primary (compromised) communication channel.

> The code itself is not the trust. The trust emerges from who generated it, how it was transported, who delivered it, and the independence of the delivery pathway.

## Conceptual Pillars

When writing copy, building UI, or designing flows, these pillars must come through:

1. **Out-of-band by default** — codes never travel through the same channel as the request they verify.
2. **Human couriers as infrastructure** — physical and social continuity is the security primitive, not a UX afterthought.
3. **Trust-preserving friction** — intentional checkpoints are a feature, not a bug. Never optimise for frictionless flow.
4. **Pixels → proofs** — visual recognition is replaced by cryptographic verification, anchored in KERI/ACDC.
5. **Compositional trust** — no single layer is sufficient; trust emerges from independent paths converging.

## Code Format

selfdriven.codes are short, memorable, verbally exchangeable trust phrases.

### Phrase format (default, human-friendly)

`ADJECTIVE-NOUN-NUM` where:
- ADJECTIVE and NOUN drawn from a curated word list optimised for distinctness, pronounceability, and absence of homophones
- NUM is 2–3 digits

Examples: `EMBER-RIVER-91`, `ORBIT-LANTERN-482`, `SOLAR-FOREST-229`, `AURORA-HARBOR-17`, `DELTA-COMPASS-803`

### Alphanumeric format (alternative)

`XXXX-XXXX-XXXX` using a Crockford-style ambiguity-free character set (`ABCDEFGHJKLMNPQRSTUVWXYZ23456789` — no `I`, `O`, `0`, `1`).

Examples: `K3PM-7VQR-2J9X`, `BNHT-4FYZ-8MCK`

### Code properties (always)

| Property | Value |
|----------|-------|
| Human-readable | Easy verbal exchange |
| Short-lived | Default TTL 5 minutes, configurable per session |
| Contextual | Bound to a specific session or interaction |
| Out-of-band | Never travels with the request it verifies |
| Memorable | Distinct enough to read aloud once |
| Rotatable | Continuous trust renewal supported |
| Decentralised | Codes are bound to KERI AIDs, no central authority |

### Word list discipline

When generating word lists for code phrases, follow these rules:
- 6+ characters preferred (longer words are more distinctive verbally)
- No homophones in the same list (`SEA`/`SEE`, `FOREST`/`FOR REST`)
- No words that sound similar (`HARBOR`/`ARBOR`, `LANTERN`/`PATTERN`)
- Concrete nouns and evocative adjectives — avoid abstract or technical terms
- No proper nouns, place names, or culturally specific terms
- Avoid anything that could be misheard as a numeral

## Architecture Layers

When describing or building the selfdriven.codes stack, use these six layers consistently:

| # | Layer | Function |
|---|-------|----------|
| 01 | Cryptographic | Code generation, session SAID binding, signature integrity |
| 02 | Identity | KERI AIDs (initiator and courier), ACDC role credentials, KEL continuity |
| 03 | Courier | Human transport — physical, relay, split-trust, proximity, community |
| 04 | Reputation | Courier trust scoring, interaction histories, Cardano anchoring |
| 05 | Session | Temporary interaction trust, session SAID, replay prevention via TTL |
| 06 | Governance | Rules, delegation, audit trails via append-only `ixn` events |

## Courier Types

Four canonical courier categories — use these in any listing, network diagram, or onboarding flow:

| Code | Type | Description |
|------|------|-------------|
| COURIER · 01 | Community Members | Verified neighbourhood participants with established local reputation |
| COURIER · 02 | Licensed Professionals | Notaries, solicitors, accredited agents with ACDC credentials, often anchored to GLEIF vLEI |
| COURIER · 03 | Governance Participants | Members of validated trust networks with cryptographic attestations |
| COURIER · 04 | Organisation Representatives | Designated trust officers under KERI-delegated AIDs with scoped, time-limited authority |

## Delivery Models

Five delivery models — calibrate to interaction stakes and topology:

1. **Physical** — courier physically provides the code in person (highest assurance)
2. **Relay** — code transferred through a chain of trusted intermediaries
3. **Split trust** — multiple couriers deliver fragments; no single courier holds the full code
4. **Proximity** — codes exchanged only within geographic boundaries (geofenced)
5. **Community** — trusted local organisations act as delivery nodes

## Canonical Scenarios

When illustrating selfdriven.codes use cases, lead with the **CEO/CFO Payment Approval** scenario — it is the canonical six-step flow:

1. Urgent payment request arrives (channel: Email · Suspect)
2. Voice verification attempted (channel: Voice · Suspect)
3. Trust code requested (channel: KERI · ACDC)
4. Courier dispatch (channel: Courier · Out-of-band)
5. Code matched, identity bound (channel: SAID · Verified)
6. Root trust established (channel: Root trust ✓)

Other approved scenarios:
- **Executive impersonation defence** — out-of-band verification for any C-suite request
- **Financial transaction authorisation** — high-value wire transfers, governance votes
- **Nation-state diplomatic verification** — embassy-grade trust pathways
- **Emergency civil coordination** — disaster-resistant trust establishment
- **AI system verification** — separating verified humans from autonomous agents

Avoid romantic, medical, or family-emergency scenarios unless the user specifically requests — these can read as exploitative.

## Visual Language (extends selfdriven-ecosystem)

Inherits the full selfdriven brand system (flamingo `#C8442F`, Poppins, JetBrains Mono, 20px card radius, accent top-bars). Additions specific to selfdriven.codes:

### Code display

Trust codes are always rendered in JetBrains Mono:
- Hero/feature contexts: 28–44px, weight 700, letter-spacing 0.03em
- Inline contexts: 14–18px, weight 600, often with accent colour or accent-dim background
- Code containers should have a dashed accent border or accent-dim gradient background

### Channel pills

When labelling channels in a flow, use coloured pills:

```css
.suspect  { background: rgba(255, 99, 71, 0.15);  color: #ff7a5c; }  /* compromised */
.trusted  { background: rgba(132, 226, 137, 0.12); color: #84e289; } /* verified */
.courier  { background: rgba(232, 93, 74, 0.15);  color: #e85d4a; } /* out-of-band */
```

### Network diagrams

When visualising the courier network:
- Place suspect digital channel **above** (dashed line, muted red)
- Place courier pathway **below** (solid accent line)
- Use pulse rings on courier nodes (`@keyframes ringPulse`, staggered delays)
- Show a travelling code packet (animateMotion along the courier path)
- Label zones: `↑ DIGITAL · COMPROMISED ↑` and `↓ HUMAN · TRUSTED ↓`

## Mapping to 8 Areas of Focus

When building organisational pages or governance content for selfdriven.codes, map to the 8 Areas:

| # | Area | selfdriven.codes context |
|---|------|--------------------------|
| 01 | Direction | Trust primitive strategy, courier network expansion roadmap |
| 02 | Engagement | Courier onboarding, trust community building, institutional partnerships |
| 03 | Enablement | Courier training, integration SDKs, verification rituals education |
| 04 | Protocols | KERI/ACDC integration, code format standards, courier credential schemas |
| 05 | Sustainability | Courier compensation model, transaction-based revenue, network economics |
| 06 | Processes | Code generation, dispatch workflows, verification ceremonies, audit |
| 07 | Accountability | Append-only KEL audit trails, courier reputation, dispute resolution |
| 08 | Organisational | Distributed courier governance, trust officer structure, regional nodes |

## API Patterns

selfdriven.codes API extends the standard selfdriven server pattern (express, KERI auth middleware, passkey signing).

### Core endpoints

```
POST   /api/v1/codes                       Generate a new trust code
GET    /api/v1/codes/:said                 Verify a code by its SAID
POST   /api/v1/codes/:said/rotate          Rotate (re-issue) a code mid-session
DELETE /api/v1/codes/:said                 Invalidate a code

POST   /api/v1/dispatch                    Dispatch a code via courier
GET    /api/v1/dispatch/:id                Dispatch status (pending, in-transit, delivered, verified)
POST   /api/v1/dispatch/:id/confirm        Courier confirms physical delivery
POST   /api/v1/dispatch/:id/verify         Recipient confirms code match

GET    /api/v1/couriers                    List available couriers (filtered by type, location, reputation)
GET    /api/v1/couriers/:aid               Courier profile with ACDC credentials and reputation score
POST   /api/v1/couriers/:aid/attestation   Attest to a courier interaction
```

### Response shape

Every mutating operation includes a `keriEvent` block (per selfdriven-ecosystem standard):

```json
{
  "data": {
    "code": "EMBER-RIVER-91",
    "said": "EJq8K3vN3wXyZmPq",
    "ttl": 300,
    "expiresAt": "2026-05-17T14:32:00Z",
    "boundTo": {
      "aid": "EKE4g_0hDGBOqDLKzNBT3kFOPxoP7wXkqt",
      "sessionRef": "SES-2026-05-17-44781"
    },
    "courierPath": null
  },
  "keriEvent": {
    "type": "ixn",
    "aid": "EKE4g_0hDGBOqDLKzNBT3kFOPxoP7wXkqt",
    "sn": 1747490400000,
    "digest": "sha256-..."
  }
}
```

### Dispatch states

`pending` → `assigned` → `acknowledged` → `in_transit` → `delivered` → `verified`

Each state transition is a KERI `ixn` event in the dispatch KEL. State changes that fail verification produce a `disputed` terminal state.

## Content Voice

When writing copy for selfdriven.codes properties:

- **Frame around the crisis, not the product**: Lead with what's broken (cloning, deepfakes, autonomous deception), then introduce the primitive
- **Treat couriers as infrastructure, not gig workers**: Diplomatic pouches, military couriers, historical envoys — the lineage is institutional, not commercial
- **Avoid security-vendor jargon**: No "industry-leading", "next-gen", "AI-powered". The product *resists* AI; it does not depend on it.
- **Use "trust" precisely**: Trust is established, delivered, anchored, verified. It is not "boosted", "enhanced", or "optimised".
- **Respect the ritual framing**: Codes are not credentials. The exchange is a "trust ritual" — seals, signatures, envoys, ceremonies.

Approved metaphors: diplomatic pouches, military couriers, historical messenger networks, secure device pairing, hardware roots of trust, ceremonial witnesses, social air gaps.

Avoid metaphors that imply commodification: tickets, vouchers, tokens (in the financial sense), keys (overused), passwords.

## Domain Family

selfdriven.codes sits within the trust layer of the selfdriven Foundation:

| Domain | Role in trust stack |
|--------|---------------------|
| selfdriven.foundation | Parent entity, governance |
| selfdriven.codes | **Human trust orchestration (this skill)** |
| selfdriven.institute | Position papers, research, frameworks |
| selfdriven.services | Professional services marketplace (consumes codes) |
| selfdriven.money | Banking (consumes codes for high-value transactions) |
| selfdriven.health | Health (consumes codes for clinical decisions) |

## Reference Papers

Two canonical position papers anchor the platform — link to them in any selfdriven.codes property:

- `/paper/out-of-band-human-trust-establishment` — the theoretical foundation
- `/paper/human-courier-networks-for-root-trust-delivery` — the delivery infrastructure

Always cite these as `selfdriven Institute` papers, not as marketing material.

## Checklist

Before delivering any selfdriven.codes output:

- [ ] Inherits full selfdriven brand (Poppins, JetBrains Mono, flamingo accent, 20px radius, accent top-bars)
- [ ] Dark mode supported and contrast-tested
- [ ] Codes rendered in JetBrains Mono with appropriate weight and letter-spacing
- [ ] Channel pills use the suspect/trusted/courier colour scheme
- [ ] If network diagram present: suspect channel above, courier path below, with pulse rings and traveling packet
- [ ] Code generation uses the canonical word list discipline (no homophones, 6+ char words)
- [ ] CEO/CFO scenario used as canonical example if a scenario is shown
- [ ] KERI/ACDC terminology correct (AID, SAID, KEL, `ixn`, ACDC role credential)
- [ ] Six architecture layers labelled 01–06 in correct order
- [ ] Four courier types (Community, Licensed Professional, Governance, Organisation) used consistently
- [ ] Five delivery models (Physical, Relay, Split trust, Proximity, Community) used consistently
- [ ] Voice avoids security-vendor jargon and gig-economy framing
- [ ] Links to both position papers if surface is public-facing
