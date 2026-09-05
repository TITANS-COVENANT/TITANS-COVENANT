# Paul Akogo

Accra, Ghana. I build systems end to end — model layer through deployment — then sell and maintain them, which is a separate discipline from building them.

---

## ClauseGuard — contract clause risk analysis

Transformer-based clause classification over the full CUAD taxonomy (41 categories), extended with 7 categories specific to freelance and SME contracts. A deterministic risk scorer sits on top; an LLM pass renders each flagged clause in plain English with a suggested alternative.

- **Classifier** — Legal-BERT hybrid (embedding similarity + keyword sieve), hot-swappable for a fine-tuned checkpoint
- **Pipeline** — `PDF → parser → classifier → risk scorer → simplifier → UI`, each stage independently testable
- **Stack** — FastAPI, PyTorch/Transformers, Next.js; pytest with model loading stubbed so CI runs without pulling weights
- **Constraint that shaped the design** — no persistent storage of contract content; documents are processed in memory and discarded

→ [contract-risk-analyzer](https://github.com/TITANS-COVENANT/contract-risk-analyzer) · MIT

---

## Production web systems for SMEs

I build and operate web systems for businesses in Accra on monthly retainers — visa advisory, property management, travel operations — plus internal tooling: LinkedIn lead enrichment, AI-generated Shopify product copy.

The hard part is not the code. It is shipping software to non-technical owners, on Ghanaian infrastructure, that still works six months later without me touching it. That constraint drives the engineering: boring dependencies, no client-side surprises, one-command deploys, and failure modes I can diagnose from a phone.

---

## Fluxpoint

SaaS sold into that existing client base rather than into a cold market. Distribution first, product second.

---

## How I work

Most of my code in 2026 is written through AI tooling. That moves the job up the stack — architecture, failure modes, and the decisions that are expensive to reverse — it does not remove it. I optimise for systems that survive my absence.

---

BSc Computer Science, Nov 2026 · [LinkedIn](https://www.linkedin.com/in/paul-akogo/)
