<p align="center"><img src="https://raw.githubusercontent.com/budlum-xyz/.github/main/profile/assets/budlum-banner.png" alt="budlum" width="720"></p>

The name carries the intent: bud and lum, the bud and the light. A system named after flourishing is built on the idea that layers should open one another, not close over one another.

**Budlum is the next layer of the internet, built around data sovereignty and collective flourishing.** It is a settlement layer for heterogeneous networks. It does not replace other chains; it verifies them. PoW, PoS, BFT, isolated PoA and ZK domains each keep their own consensus and produce a proof of finality, while Budlum records cross-network movement as a cryptographic fact on a single `GlobalBlockHeader`. Sovereignty over data, keys and computation stays with the participants.

One discipline organises the whole architecture: **accept only what can be proven.**

**Finality with two signature families.** Every finality certificate carries a classical signature and a post-quantum one (ML-DSA under FIPS 204). A certificate carrying a single family is refused, so the system is quantum-ready by construction, with no migration to run later.

**Verified computation.** A state transition executes once and becomes a zero-knowledge proof; the network verifies the proof instead of re-running the work. The prover is BudZero, an in-tree STARK virtual machine.

**Erasure-coded storage.** Durability comes from codes that reconstruct lost shards rather than from triple replication, at a fraction of the redundant bytes. The storage core is B.U.D. (Broad Universal Database).

**Data sovereignty as a protocol decision.** Access to an asset is decided at protocol level — Pollen grants gate every read. A request without a grant is not an application error; it is a transaction that never happens, and no override path exists.

**Inference that reads and cites.** The intelligence layer answers only what it can cite. Content enters through named channels that each carry the digest of their own bytes, and through nothing else. Lubot, the reading AI on top of this layer, shows where every sentence came from — and generates nothing it cannot check.

**Settlement between consensuses.** Because finality arrives as proofs, networks that share nothing except mathematics can settle value with one another.

## How the codebase polices itself

**Every refusal is demonstrated.** A control that cannot show it rejects the defect it exists to catch is treated as broken; refusal paths are tested against deliberately injected defects.

**Critical values are pinned.** Behaviour is locked to measured values, and a change to them cannot pass quietly.

**Constraints run one way.** Thresholds only tighten. Silencing a warning or deleting a test is not available in the build.

An audit examines the code as it stood on a date. These rules examine the code that will be written tomorrow.

## Repositories

| Repository | What it is |
|---|---|
| [budlum](https://github.com/budlum-xyz/budlum) | Reference implementation: Universal Settlement Layer, BudZero STARK VM, B.U.D. storage, Pollen, AI inference layer ([Türkçe](https://github.com/budlum-xyz/budlum/blob/main/README.tr.md)) |
| [lubot](https://github.com/budlum-xyz/lubot) | The reading AI: answers from what the network stores, under its permissions, with a citation for every sentence |
| [seed](https://github.com/budlum-xyz/seed) | Transfer core of B.U.D. 3.0 as a standalone crate: content in, optical carrier plus recipe out, byte-for-byte rebuild — or a refused one |

## Project status

Research-grade software under active development: **no mainnet, no external audit.** Capabilities the code deliberately does not enable are pinned by tests that break if that changes — see [Project status](https://github.com/budlum-xyz/budlum/blob/main/README.md#project-status) and [AI verification status](https://github.com/budlum-xyz/budlum/blob/main/docs/AI_VERIFICATION_STATUS.md). We do not claim the system cannot be attacked; we claim every check it makes is demonstrated, pinned and one-way.

## License

[PolyForm Shield 1.0.0](https://github.com/budlum-xyz/budlum/blob/main/LICENSE.md). Security reports: see [Security](https://github.com/budlum-xyz/budlum/blob/main/docs/SECURITY.md).
