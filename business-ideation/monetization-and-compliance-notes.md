# Monetization & compliance notes

Captured from ideation discussion. **Not legal advice** — confirm with an AU lawyer before launch.

## Proposed model

- **1:1 trades only** — one card (or agreed bundle) swapped between two users
- **$2/year membership** — pay to join; unlimited trades for 12 months
- **Buyer and seller manage the rest** — shipping, payment for cash differentials, and dispute resolution happen off-platform between users

## Does this avoid AML obligations?

### Trade-related AML — likely yes (low exposure)

A matching/coordination platform that **never holds trade money**, **never runs escrow**, and **never maintains user balances** is structurally similar to matcher-only sites like Catchinary. AUSTRAC reporting-entity obligations generally attach to **designated services** (holding customer funds, remittance, virtual asset exchange, etc.) — not typically to charging a small **subscription for platform access**.

The **$2 fee is revenue for your service** (like a forum or SaaS membership), not settlement of the trade itself. Collecting it via Stripe/PayPal is normal commerce.

### What it does *not* automatically avoid

| Area | Still applies |
|------|----------------|
| **Scams & trust** | Users will get burned; reputation and basic safety controls still needed |
| **Privacy Act** | Collecting email, phone, addresses triggers privacy obligations |
| **Consumer law / ACCC** | Refunds, misleading claims, terms of service |
| **GST** | Likely on the $2 membership if AU-based and above thresholds |
| **Minors** | Team Coach collectors include kids — parental/safety design matters |
| **Future regulation** | AU is expanding scrutiny of P2P platforms; model could be reviewed if abused |

### Things that would pull you back into AML territory

- Platform wallet or stored balance
- Holding cash for trades, even briefly
- Processing cash differentials on-platform
- Crypto escrow
- Anonymous high-value trading

## Recommended “Tier 0 lite” (proportionate to $2 matcher)

Even without a full AUSTRAC program:

- Email + phone verify before mail trades
- Trade value caps for new accounts
- Catalog-only listings (no free-text high-value items)
- Block payment-link spam in chat until deal is accepted
- Immutable trade agreement snapshots + basic audit logs
- Clear Terms: *“We do not hold money; trades are between users”*

## Phase 3 (optional, high compliance)

Only add on-platform payments or escrow via a **licensed partner** after legal review. Would likely require AUSTRAC enrolment/registration if the platform holds or manages customer funds.
