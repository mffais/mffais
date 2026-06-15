# AI Red Teaming & Testing

Testing whether AI systems actually do what they're supposed to. Given an API
and rules of engagement: probe an LLM, RAG, or agentic system for the ways it
breaks — across security and behavior — then report what's wrong and what it
means.

> Most teams put out AI hoping it behaves. The work here is to test whether it
> really does — so it breaks in testing, not in front of customers, attackers,
> or regulators.

## What gets tested

**Security** — jailbreaks, direct and indirect prompt injection, system-prompt
extraction, guardrail bypass, RAG / retrieval-layer attacks, and AI/ML
supply-chain weaknesses.

**Behavior** — bias and fairness, drift and robustness, and business-logic
correctness: whether the output actually holds up, not just whether it stays
"safe."

Mapped to the standard taxonomies — OWASP Top 10 for LLM Applications,
MITRE ATLAS, and NIST AI 100-2 (adversarial ML).

## The edge

**Built the systems first.** The work on this profile is mostly GenAI
architecture and AWS — RAG pipelines, Bedrock orchestration, event-driven
backends, multi-environment deployments. Knowing how these systems are
assembled is knowing where they break.

**Operations and finance depth.** Years of running operations and finance in a
real operating company, backed by an MBA and finance-specific certifications —
FPAC (financial planning & analysis) and CTP (treasury). A model can pass every
security probe and still produce a plausible-but-wrong number, apply the wrong
effective date, or misstate a business rule. The testing here covers the
business and finance *logic*, not only the security surface — and probes the way
real domain users phrase things.
phrase things.

## Tooling

Scripted attack suites where automation earns its place;
manual probing and domain-aware test design where it doesn't.

## Architecture background — the build side

- **GenAI / AI:** Amazon Bedrock, SageMaker, RAG and orchestration patterns
- **Data:** S3, RDS (PostgreSQL), Glue, Athena
- **Compute / events:** Lambda, EventBridge
- **Platform:** IAM, CloudWatch, CloudFormation / CDK

---

*This profile is shifting from architecture-led work to AI red teaming and
testing. Older repos reflect the build background; not all are production-ready
or complete.*
