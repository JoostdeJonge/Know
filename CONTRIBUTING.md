# Contributing to KNOW

KNOW is an open protocol. It succeeds only if people with different expertise contribute. This document maps out where help is needed most.

## Where to start

1. **Read the [concept paper](CONCEPT.md)** -- especially the [open questions](CONCEPT.md#open-questions).
2. **Pick the area that matches your expertise** (see below).
3. **Open a Discussion or Issue** with your thoughts, critique, or proposal.

Disagreement is welcome. Falsifiability is a core principle -- it applies to the protocol itself.

## Areas of contribution

### Pattern Specification
*For people who think in type systems, schemas, and interfaces.*

The most immediate need: define exactly what a KNOW pattern looks like as a data structure. What are the input/output type contracts? How are proof levels represented? How do dependencies reference each other? This is the foundation everything else builds on.

**Start here**: Propose a draft schema (JSON, protobuf, or your preferred format) in a Discussion.

### Extraction & Compilation
*For people who work on LLM reasoning traces, code generation, or program synthesis.*

How do you go from a probabilistic reasoning chain to a deterministic executable? What classes of patterns can be reliably compiled, and where are the hard boundaries? What does the extraction pipeline look like?

**Start here**: Take one concrete example (e.g., a math derivation an LLM performs repeatedly) and walk through how you would extract and compile it. Share your process.

### Verification & Falsification
*For people in formal methods, testing, or AI safety.*

How do we verify that an extracted pattern is correct? How do we test edge cases systematically? How does falsification work in practice -- what triggers a retraction or amendment? How do we prevent adversarial patterns?

**Start here**: Propose a verification framework for a single pattern type (transformation, decision, or reasoning template).

### Routing & Retrieval
*For people who work on search, recommendation, or agent orchestration.*

When a query arrives, how does the system match it to known patterns efficiently? How does routing work at scale (millions of patterns)? Can routing itself be incrementally compiled?

**Start here**: Describe how you would build a router for 100 patterns. Then describe what breaks at 1 million.

### Decentralized Infrastructure
*For people in distributed systems, blockchain, or peer-to-peer networks.*

How should patterns be stored, replicated, and verified across a decentralized network? What are the right tradeoffs between on-chain integrity and off-chain storage? How do incentive mechanisms (contribution rewards, usage fees) work at the protocol level?

**Start here**: Evaluate existing infrastructure (IPFS, Arweave, Solana, etc.) against KNOW's requirements. What fits, what's missing?

### Economics & Incentive Design
*For people who think about mechanism design, token economics, or game theory.*

How do you reward contributions proportionally to value? How do you prevent gaming? What's the right balance between contribution incentives and usage costs? How does the system bootstrap before network effects kick in?

**Start here**: Model the economics of anchoring a single pattern -- from extraction cost through usage revenue. What assumptions matter most?

### Societal Impact & Knowledge Representation
*For people in education, philosophy of science, knowledge management, or AI ethics.*

How does a human-readable knowledge network change education, research, or accountability? What are the risks of externalizing machine knowledge this way? How should proof levels map to trust in practice?

**Start here**: Describe a concrete scenario where someone (student, researcher, auditor) uses the KNOW network. What do they see? What do they learn?

## Guidelines

- **Substance over polish.** A rough idea in a Discussion is more valuable than a perfect document that never ships.
- **Critique is contribution.** If you think part of the concept is wrong, say so with reasoning. That's exactly how this is supposed to work.
- **Small is fine.** You don't need to solve an entire open question. One concrete example, one counterargument, one draft schema -- all useful.
- **No gatekeeping.** If you're interested, you belong here.

## Code of conduct

Be constructive. Argue ideas, not people. This is a scientific endeavor -- we follow the evidence.
