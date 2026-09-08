<p align="center"><img src="https://raw.githubusercontent.com/budlum-xyz/.github/main/profile/assets/budlum-banner.png" alt="budlum" width="720"></p>

# budlum

The name carries the intent: bud and lum, the bud and the light. A system named after blossoming is built on the idea that layers should open one another, not close over one another.

Budlum is a settlement layer for heterogeneous networks. It does not replace other chains; it verifies them. Each network keeps its own consensus and produces a proof of finality, while Budlum records cross-network movement as a cryptographic fact on a single header. Sovereignty over data, keys and computation stays with the participants.

One discipline organises the whole architecture: accept only what can be proven.

**Finality with two signature families.** Every finality certificate carries a classical signature and a post-quantum one. A certificate carrying a single family is refused, so the system is quantum-ready by construction, with no migration to run later.

**Verified computation.** A state transition executes once and becomes a zero-knowledge proof; the network verifies the proof instead of re-running the work.

**Erasure-coded storage.** Durability comes from codes that reconstruct lost shards rather than from triple replication, at a fraction of the redundant bytes.

**Data sovereignty as a protocol decision.** Access to an asset is decided at protocol level. A request without a grant is not an application error; it is a transaction that never happens, and no override path exists.

**Inference that reads and cites.** The intelligence layer of the stack answers only what it can cite. Content enters through named channels that each carry the digest of their own bytes, and through nothing else.

**Settlement between consensuses.** Because finality arrives as proofs, networks that share nothing except mathematics can settle value with one another.

## How the codebase polices itself

**Every refusal is demonstrated.** A control that cannot show it rejects the defect it exists to catch is treated as broken; refusal paths are tested against deliberately injected defects.

**Critical values are pinned.** Behaviour is locked to measured values, and a change to them cannot pass quietly.

**Constraints run one way.** Thresholds only tighten. Silencing a warning or deleting a test is not available in the build.

An audit examines the code as it stood on a date. These rules examine the code that will be written tomorrow.

Reference implementation: [budlum-xyz/budlum](https://github.com/budlum-xyz/budlum)
