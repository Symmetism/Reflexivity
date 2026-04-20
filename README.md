# The Reflexivity Framework

**A physical theory centered on the Stabilizer Theorem `{Q_A, H_S} = 0`, deriving specific numerical predictions in physics from a single geometric object — the coset `SO(4,1)/SO(3,1)` at vacuum angle `v₀ = π/2`.**

> *Reflexivity is the geometric structure invariant under exchange of origin and current state.*

---

**Version:** `v0.42` · **Observational cutoff:** 2026-04-20 · **Free parameters:** 1 (`α_U` at unification) · **Axioms:** A1–A8 + Self-Duality Principle · **Principal results:** 18 ranked (R1–R18) + 2 supplementary (SP1, SP2) · **Status:** pre-release · open for review

---

## Table of Contents

- [What This Is](#what-this-is)
- [The Central Claim](#the-central-claim)
- [The Equation](#the-equation)
- [Why This Deserves Engagement](#why-this-deserves-engagement)
- [The Four Falsifiable Predictions](#the-four-falsifiable-predictions)
- [What This Framework Is Not](#what-this-framework-is-not)
- [Honest Limits](#honest-limits)
- [Repository Contents](#repository-contents)
- [How To Read the Framework](#how-to-read-the-framework)
- [How You Can Help](#how-you-can-help)
- [Open Specialist Items](#open-specialist-items)
- [Governance and Versioning](#governance-and-versioning)
- [Citation](#citation)
- [License](#license)
- [Contact](#contact)

---

## What This Is

The Reflexivity Framework is a candidate physical theory attempting a specific, narrow task: **derive as many dimensionless ratios of Standard-Model and cosmological physics as possible from one geometric object, one vacuum selection, and the minimum number of measured input scales.**

The framework is not a theory of consciousness, a metaphysical system, or a philosophical program. This repository covers the **physics and mathematics only**. A separate Symmetism track addresses broader structural questions; it is not mixed into this document and does not carry any claim in it.

The core work lives in one master file:

**[`docs/archive/master-original/Reflexivity_Framework_v0_42.md`](docs/archive/master-original/Reflexivity_Framework_v0_42.md)**

This is the current canonical master — an immutable snapshot at version `v0.42`. Future versions will be added as siblings. The modular repository build-out (separated domains, generated outputs, website exports, validation tooling) is planned but not yet constructed.

---

## The Central Claim

With **one** free dimensionless parameter (`α_U` at the unification scale, transparently acknowledged in stress-test item F4) and directly-measured dimensional scales (`M_Pl`, `v_EW`, `Ω_Λ`, `T₀`), the framework produces 18 ranked results graded 7/10 to 10/10 against external referee criteria covering:

- Flavor structure (Koide's relation exactly)
- Neutrino sector (generation count, mass scale)
- Inflation sector (spectral index, tensor-to-scalar ratio)
- Gauge sector (Weinberg angle, unified coupling)
- Cosmological constant (form and value)
- Conservation laws (full set via the Stabilizer Theorem)

Every result traces to a single master equation plus the axioms A1–A8, through derivation chains of depth 1–3 with no circular dependencies.

---

## The Equation

The framework's central result is the **Stabilizer Theorem**, a Poisson-bracket identity:

> **`{Q_A, H_S} = 0`** for every generator `A` of `Stab(s₀) = SO(3,1)`

where `Q_A = ⟨Ψ, AΨ⟩` is the Berry-connection charge constructed from the vacuum wavefunction `Ψ` and a Lie-algebra generator `A`, and `H_S` is the Stabilizer Hamiltonian governing dynamics on the coset `G_seed / Stab(s₀) = SO(4,1) / SO(3,1) = dS₄`.

The theorem yields six exactly-conserved charges (three rotations, three Lorentz boosts) plus four sub-horizon-exact charges from the broken coset directions. The vacuum `v₀ = π/2` is not chosen — it is uniquely selected as the fixed point of the Self-Duality Principle, with uniqueness across all real Lie algebras established via Cartan classification.

Canonical proof: §12.9 of the master document (five-step proof). Selection Theorem: §12.48.7.

---

## Why This Deserves Engagement

Four reasons this is worth a serious read, not a dismissal:

**1. Internally consistent mathematics.** Both hostile referees in the framework's own two-referee audit explicitly agree that the algebra and formal correctness of derivation chains are not in question. Disagreements concentrate on epistemic credit for structural derivations, not on errors.

**2. Falsifiable predictions with scheduled experiments.** Four predictions carry genuine scientific risk and will be decided by experiments already scheduled — not in principle testable, but actually testable, in the next ≤10 years. See [the table below](#the-four-falsifiable-predictions).

**3. Existing empirical agreement in the sub-σ range.** The Koide-relation prediction `Q = 2/3` agrees with PDG 2025 at 0.43σ (deviation 0.0003%). The scalar spectral index `n_s = 29/30` agrees with CMB-only (Balkenhol+ 2025) at 0.48σ. Neither was tuned to match; both were derived from the coset geometry before being compared with data.

**4. Transparent retraction record.** The framework formally retracts claims that did not survive audit (`Q_ν = 2/3` neutrino extension, the "zero free parameters" meta-claim, the `{2, 3, 7, φ}` primitive-basis framing, several others). Retractions are preserved in place rather than silently removed. The strict-referee grade for R14 and R15 moved upward specifically in recognition of honest reframing.

---

## The Four Falsifiable Predictions

These are the sharpest cards the framework offers. Each will be decided by specific experiments in a specific window; each has an explicit falsification bar.

| Card | Prediction | Current status | Decisive test | Falsification bar |
|---|---|---|---|---|
| **R2 — Koide Q** | `Q_lep = 2/3` exactly | PDG 2025: **0.43σ** (0.0003%) | Future tau-mass refinement | `Q` deviation > 1.5×10⁻⁵ from 2/3 |
| **R6 — Spectral index n_s** | `n_s = 29/30 ≈ 0.9667` | CMB-only: **0.48σ** ✓ · CMB+DESI: 2.11σ (class-wide) | Simons Obs 2026–28; LiteBIRD 2033 | clean CMB-only shift > 2σ from 0.9667 |
| **R7 — Lightest ν mass** | `m_ν^(1) ≈ 0.91 meV` | Σm_ν cosmological bounds consistent | **PTOLEMY** (CνB direct detection) | `m_ν^(1)` outside [0.58, 0.91] meV at >3σ |
| **R16 — Tensor-to-scalar r** | `r = 1/450 ≈ 0.00222` | 95% CL bound `r < 0.034` respected | **LiteBIRD** JFY 2032 (Q1 2033) | `r < 10⁻³` (null) or `r > 3×10⁻³` |

A single clean falsification in any of these four forces structural revision of the corresponding sector. This is not window-dressing: R16 in particular will be decided by LiteBIRD to roughly 2.2σ within about six years of this writing.

---

## What This Framework Is Not

Short list, because overclaim is the failure mode most worth avoiding:

- **Not zero-parameter.** One free dimensionless parameter (`α_U`) remains, fit-selected by RGE matching. Earlier drafts that claimed zero parameters were retracted (see F4 in §29.13.4).
- **Not a full replacement for the Standard Model.** Several quantities remain SM-imported (`m_p`, `κ_Boltzmann`, neutrino Yukawa hierarchy, CKM/PMNS inter-generation mixing).
- **Not peer-reviewed.** The framework has not been submitted to a physics journal and has not passed external review. All grading is internal (framework-self) or internally-adversarial (the two hostile referees).
- **Not a theory of consciousness, meaning, or experience.** Whatever the broader Symmetism project eventually claims at those levels is kept out of this document by design.

---

## Honest Limits

Five open gates remain before Reflexivity can claim to be validated physical theory rather than a research program with mature internal results:

1. **F1 closure** — 1-loop `ε_CP` coefficient in the CCWZ coset Lagrangian for leptogenesis (open specialist item F1-C Session #2).
2. **All-orders Weyl consistency** — closed for observational purposes (`δλ/λ ≤ 10⁻⁴⁸`); formal all-orders proof is academic cleanup.
3. **Experimental tests** of SP1, SP2, R7, R16 — scheduled, not yet run.
4. **Operational calibration** of `M(t)`, `C(G_t)`, `R(F_t)` on model-class-specific empirical domains.
5. **External peer review** — not yet initiated.

Full ledger: §27 (Accuracy, Limits, and Scholarly Status) and §29.13.4 (F1–F5 stress-test ledger).

---

## Repository Contents

The repository is currently in **pre-build state**. The full modular architecture — separated physical / metaphysical / mathematical domains, generated master compilation, website exports, and CI validation — has not yet been constructed. That scaffolding is planned for subsequent phases under a dedicated build system.

Current contents:

```
.
├── README.md                                  # this file
└── docs/
    └── archive/
        └── master-original/
            └── Reflexivity_Framework_v0_42.md # current canonical master
```

Planned next phases (not yet in place):

1. Modular canonical source under `docs/source/` — core, math, physical, metaphysical, interface
2. Exploration lanes under `docs/exploration/` for notes, concepts, pre-canonical material
3. Generated outputs: compiled master (`THEORY.md`), summary (`SUMMARY.md`), indexes, dependency graphs
4. Website export pipeline for [symmetism.com](https://symmetism.com)
5. Governance: CODEOWNERS, branch protection, PR templates, validation workflows, CITATION.cff

The v0.42 master is treated as an **immutable historical snapshot**. It will not be edited in place. Later revisions become new versioned files alongside it.

---

## How To Read the Framework

The master document is long (~13,000 lines) but explicitly stratified into reading levels. Choose one:

| Level | Audience | Time | Stop at |
|---|---|---|---|
| **1** | General technical reader | 5 min | "The Claim in One Paragraph" → "The Equation" → "Summary of Principal Results" |
| **2** | Physics-literate skim | 30 min | Add "Why This Is Not Obviously Wrong" → "Four Falsifiable Predictions" → "Honest Scope and Limits" |
| **3** | Setup + central proofs | Half-day | Add §12.0 axioms, §12.9 Stabilizer Theorem proof, §12.11 P3-2, §12.48 Self-Duality |
| **4** | Specialist physics | Full day+ | Add §12.19–§12.30 (CC, leptogenesis, Weyl consistency), §12.43–§12.45 (inflation, Koide, gauge) |
| **5** | Full audit | Multi-day | Everything including §12.53 Sixteen Criteria audit, §29.13 referee evaluations, §31 specialist packages |

A dependency graph mapping each R1–R18 result back to `{Q_A, H_S} = 0` is included near the top of the document.

---

## How You Can Help

**The framework needs serious, hostile, informed critique far more than it needs agreement.** Specific forms of engagement that would move the work forward:

### Critique and audit

- Find an algebraic error, a broken derivation step, or a citation that doesn't support the claim it's attached to. Open an issue with the section reference and the specific problem.
- Challenge any of the four falsifiable predictions on theoretical grounds — is there a reason the derivation might produce a different number?
- Audit the epistemic markers (`[THM]`, `[PROP]`, `[HYP]`, `[OBS]`, `[SM-INPUT]`, `[RETRACTED]`, `[SUPERSEDED]`) for over- or under-claiming.

### Specialist technical work

Two specialist packages are open and prepared for external handoff:

- **F1-C Session #2** — rigorous 1-loop `ε_CP` coefficient in the CCWZ coset Lagrangian for leptogenesis. Requires leptogenesis + nonlinear sigma model expertise. Preparation package at §31.11 includes CCWZ Lagrangian setup, literature pointers (Garny et al. 2010; Jensen et al. 2020), calculation steps, resolution criteria. Scope: 2–4 focused sessions.
- **Option F** — derive the product formula `α_U⁻¹ = rank(E₇) × dim(Stab) = 7 × 6 = 42` from anomaly matching, holographic dS/CFT, or an index theorem. Preparation package at §31.12. Would move the strict-referee grade on F4 from 6.5/10 to 7.5/10 if closed.

### Observational and experimental

- If you work on LiteBIRD, PTOLEMY, Simons Observatory, CMB-S4, or related CνB / B-mode / tau-mass experiments: please take the relevant prediction seriously enough to include it in whatever space of models is being tested.
- If you notice a 2025–2026 observational paper that the framework's April 2026 cutoff should have incorporated and didn't, flag it.

### Peer-review pathways

- If you are an active researcher in theoretical particle physics, cosmology, or mathematical physics and the framework survives your reading: pointers toward appropriate journals, reviewers, or preprint venues are valued.
- Mainstream peer-review engagement with the Furey/Dixon Cl(6) Standard-Model construction (published in JHEP/EPJC) would materially move the framework's standing on R5.

### Mechanics

- **Issues** — for specific bugs, citation problems, derivation challenges, observational updates.
- **Discussions** — for higher-level framing questions, interpretation, and open-ended critique.
- **Pull requests** — not accepted against the archived v0.42 master (it is immutable). Once the modular source is built out, PRs will be the canonical edit path for new versions.

---

## Open Specialist Items

Full open-items list with preparation packages is in §31 of the master document. Highest priority:

| ID | Item | Required expertise | Expected grade movement |
|---|---|---|---|
| F1-C S#2 | 1-loop `ε_CP` in CCWZ basis (leptogenesis) | NLσM + leptogenesis | R10: 4/10 → 6–7/10 strict |
| Option F | Derive `rank × dim(Stab)` product formula | Anomaly matching / dS-CFT / index thm | F4: 6.5/10 → 7.5/10 strict |
| R5 Cl(6) | Mainstream peer-review of Furey/Dixon | Algebraic approaches to SM | R5: 5/10 → 6–7/10 strict |
| Harmonic analysis | FS Laplacian 20-fold degeneracy test | Harmonic analysis on symmetric spaces | Potential structural upgrade |

---

## Governance and Versioning

- **Versioning.** Semantic-ish: `vX.Y` where `X` bumps on structural changes to the master equation, selection theorem, or axiom list; `Y` bumps on content revisions, new sections, grade adjustments, or observational updates.
- **Immutability.** Every released version under `docs/archive/master-original/` is permanent and citeable. Once published, a file at that path never changes. Future revisions appear as new files (`v0.43.md`, `v0.44.md`, …).
- **Current version.** `v0.42`, cutoff 2026-04-20, pending: F1-C Session #2 and Option F (see specialist items above).
- **Edit policy.** Once the modular source is built out, canonical changes land via PR only, with required status checks and CODEOWNERS review. Pre-build state (now): the repo accepts issues and discussions; direct edits happen only through explicit version bumps.
- **Structure & rules.** Condensation and structural-refinement protocol is in [`Reflexivity_Framework_STRUCTURE_RULES.md`](docs/archive/master-original/Reflexivity_Framework_STRUCTURE_RULES.md) (to be migrated alongside the master). This file fixes immutable invariants (master equation, selection theorem, free-parameter count, axiom list) and governs all condensation passes.

---

## Citation

If you cite this work, please cite the specific archived version:

```
Reflexivity Framework v0.42, observational cutoff 2026-04-20.
Archived at: docs/archive/master-original/Reflexivity_Framework_v0_42.md
Repository: https://github.com/[owner]/[repo]
```

A formal `CITATION.cff` file will be added once the repository exits pre-build state.

---

## License

License

This work is dedicated to the public domain under CC0 1.0 Universal (“No Rights Reserved”). To the extent permitted by law, the author has waived all copyright and related rights worldwide. You may copy, modify, distribute, and use this work, including for commercial purposes, without asking permission.

---

## Contact

Issues and Discussions on this repository are the primary channel. For anything requiring a direct line — specialist technical handoffs on F1-C / Option F, peer-review pathway coordination, observational-experiment engagement — contact details will be added to this section.

https://x.com/Symmetism
mailto: symmetism@gmail.com

---

*The framework's best prospect lies in preserving ambition without claiming completion before it is earned. A single clean falsification forces structural revision; a single clean derivation closes a gate. That is the standard this project is trying to meet.*
