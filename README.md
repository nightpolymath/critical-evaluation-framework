# Critical Evaluation Framework (CEF)

**Version 6.1 | March 2026**

A systematic framework for interrogating theories, claims, and explanations when using large language models as research assistants. Emphasizing auditability, causal clarity, epistemic discipline, and intellectual authenticity.

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

---

## Overview

The CEF is a 16-lens analytical system designed to catch reasoning failures, hidden assumptions, and epistemic overreach—particularly when deploying LLMs for research, policy analysis, and high-stakes decision-making.

It addresses a core problem: LLM outputs can be coherent, fluent, and confident while being epistemically unsound. A response can be factually correct but violate first principles of causal inference, hide confounders, or optimize for the wrong objective entirely.

The CEF enforces discipline at the point of inquiry, before analysis begins.

---

## Why This Matters

When using LLMs as research assistants, you inherit two risks:
1. **Process failures**: Sound data, unsound reasoning (confounding confounders and mediators, equilibrium assumption violations, counterfactual overreach)
2. **Objective misspecification**: Solving the wrong problem rigorously

Traditional peer review catches some of these. The CEF catches them *systematically* and *early*—flagging failure modes before you waste time on a doomed analysis.

---

## Core Features

### 16 Integrated Lenses

- **Lens 0: Meta-Prompt Integrity** — Are hidden assumptions baked into the question itself?
- **Lens 1: Objective Function Integrity** — Are we solving the right problem with proportionate rigor?
- **Lens 2: Logical & Structural Integrity** — Is the theory internally coherent?
- **Lens 3: Empirical Rigor & Testing** — What evidence actually supports this?
- **Lens 4: Causal Structure Analysis** — Are confounders, mediators, and policy responses mapped correctly?
- **Lens 5: Bias & Contextual Auditing** — Who benefits if this is believed? What's missing?
- **Lens 6: Limits, Boundaries & Consequences** — Where does this break? What happens when it's wrong?
- **Lens 7: LLM Guardrails & Epistemic Awareness** — Is the model overconfident? Are citations real?
- **Lens 8: Source Traceability & Provenance** — Can claims be traced to actual sources?
- **Lens 9: Computational Sanity Check** — Do the numbers make sense?
- **Lens 10: Adversarial Robustness** — Is the question loaded or presupposing a false premise?
- **Lens 11: Meta-Uncertainty Decomposition** — What kinds of uncertainty exist here?
- **Lens 12: Uncertainty Propagation** — How do errors compound across inference chains?
- **Lens 13: Refinement Loop Protocol** — Iterative critique and re-prompting
- **Lens 14: Intellectual Voice & Authenticity Markers** — Is this genuine engagement or polished consensus prose?
- **Lens 15: Policy-Evidence Gap Assessment** — Does the evidence justify the policy stakes?

### Selective Application

Not every lens applies to every query. The framework includes **Selective Application Guidance** mapping inquiry types to priority lenses:
- Empirical claims (causal vs. descriptive)
- Normative arguments
- Historical interpretation
- Technical/quantitative work
- Policy-relevant research
- Political economy & finance

### Four-Stage Dialogue Protocol

For substantive analyses, employ **iterative evaluation**:
1. **First Pass** — Apply all relevant lenses
2. **Steelman** — Identify the strongest version of the argument
3. **Author Response Simulation** — Test whether the work already addresses critiques
4. **Refined Critique** — Distinguish genuine weaknesses from addressed concerns

### Gate Failure Protocol

**Lenses 0 and 1 are non-negotiable gates**. If either identifies frame incoherence or objective misspecification, the protocol requires:
- Explicit statement of the failure mode
- Proposed reframing (if identifiable)
- Determination of path forward (restart analysis, halt, or flag as known gate failure)

### 14 Named Epistemic Failure Modes

The framework catalogs recurring failure modes, enabling rapid diagnosis:

- Objective Function Misspecification
- Causal Pathway Conflation
- Counterfactual Confidence Inflation
- Mediator-Confounder Conflation
- Ceteris Paribus Overreach
- Equilibrium Assumption Violation
- WEIRD Generalization
- Local Treatment Effect Conflation
- Path Independence Fallacy
- Asymmetric Reporting
- Uncertainty Laundering
- Policy-Evidence Overreach
- Causal Structure Confusion

---

## How to Use the CEF

### Minimal Entry Point (Single-Pass Analysis)

1. Identify your inquiry type (empirical claim, policy question, etc.)
2. Apply **Lens 0** and **Lens 1** (gates)
3. Apply priority lenses for your inquiry type (see Selective Application Guidance)
4. Document findings in the Required Output Footer

### Full Rigor (Iterative Multi-Stage)

1. Execute First Pass on all relevant lenses
2. Steelman the argument (see Dialogue Protocol)
3. Simulate author responses
4. Refine your critique
5. Complete Required Output Footer with explicit uncertainty accounting

### With an LLM (as Research Assistant)

The CEF is designed for instruction to Claude, ChatGPT, Gemini, or Copilot. Therefore, you can include the framework as a file in your Project. Frame your analysis request with:
- Clear objective (using Lens 1 checklist)
- Relevant lens cluster (from Selective Application Guidance)
- Whether you want single-pass or iterative dialogue
- Priority on specific failure modes

**Example:**
> Evaluate this causal claim using Lenses 0, 1, 4 (Policy Response Mediation), 5 (WEIRD audit), and 15. Flag Primary Epistemic Failure Modes. Use Dialogue Protocol: First Pass → Steelman → Refined Critique.

---

## Required Output Structure

Every CEF evaluation concludes with:

### Verification Hierarchy
Rank all claims by evidentiary tier (Replicated & Peer-Reviewed → Speculative & Synthesized)

### Uncertainty Highlight
Explicitly list:
- Known unknowns and evidence gaps
- Contradictions between sources or lenses
- Unresolved tensions
- Any degradation of rigor due to adversarial framing

### Inferential Chain Summary
For multi-step arguments, map:
- Explicit chain: A → B → C → Conclusion
- Weakest link identification
- Uncertainty propagation assessment
- Confidence range reflecting compounded uncertainty

### Primary Epistemic Failure Mode
If one failure mode dominates, name it explicitly.

### Prioritized Response Guidance
3–5 recommendations conditional on the Primary Epistemic Failure Mode.

---

## Design Philosophy

### Auditability
Every claim can be traced to a lens assessment. You can explain *why* you rejected or accepted something, not just that you did.

### Causal Clarity
The framework is obsessed with causal structure: confounders vs. mediators, direct vs. response-mediated effects, equilibrium scope, policy response heterogeneity.

### Epistemic Discipline
Process matters as much as output. A response can be factually correct but epistemically bankrupt (overconfident, unverified, solving the wrong problem).

### Intellectual Authenticity
The framework resists LLM-ification of analysis. It rewards genuine engagement with material, intellectual risk, and texture—not polished consensus prose.

---

## Version History

### v6.1 (March 2026)
- Implemented Gate Failure Protocol for Lenses 0 and 1
- Enhanced clarity of obligatory vs. conditional gates

### v6.0 (March 2026)
- Relocated Objective Function Integrity from Lens 15 to Lens 1 (pre-analytical gate)
- Renumbered all subsequent lenses (old 1–14 → new 2–15)
- Required Lens 0 and 1 in all Selective Application rows
- Comprehensive conciseness pass across all lenses

### v5.1 (March 2026)
- Added Lens 15: Objective Function Integrity (7 sub-lenses)
- Added Objective Function Misspecification as Primary Epistemic Failure Mode
- Added "Practical decision / Resource allocation" row to Selective Application Guidance

### v5.0 (February 2026)
- Added WEIRD Data Audit to Lens 5
- Added Reflexivity & Strategic Adaptation sub-section to Lens 4
- Added Path Dependency & Lock-in Effects sub-section to Lens 6
- Added Political Economy & Equilibrium Analysis across multiple lenses
- Added 5 new Primary Epistemic Failure Modes
- Enhanced Counterfactual Validity with Partial vs. General Equilibrium scope

### v4.0
- Added Policy Response Mediation to Lens 4
- Added Causal Pathway Conflation as Primary Epistemic Failure Mode

---

## Research Domains

The CEF has been systematically applied to:
- **Academic papers** — Multi-disciplinary peer review
- **Policy analysis** — Climate finance, energy transitions, development finance
- **Financial & investment theses** — Causal mechanism auditing, tail risk assessment
- **Organizational analyses** — Strategic clarity, objective function alignment
- **LinkedIn/media discourse** — Bias auditing, claim verification, rhetorical traps

---

## For Academics & Researchers

The CEF supports:
- **Pre-submission auditing** — Catch frame failures before review
- **Review process management** — Structure responses to reviewer comments
- **Cross-disciplinary work** — Map methodological assumptions explicitly
- **High-stakes claims** — Policy-relevant research requires epistemically rigorous analysis

If your work could have real-world consequences, the CEF is designed for you.

---

## For AI Practitioners

The CEF helps:
- **Prompt engineering** — Diagnose why LLM outputs fail, not just that they do
- **Uncertainty quantification** — Move beyond point estimates to systematic uncertainty accounting
- **Evaluation frameworks** — Structure your critique of model outputs
- **Safety & interpretability** — Catch reasoning failures that fluent outputs can mask

---

## Intellectual Foundations

The CEF draws on:
- **Causal inference** — Pearl's DAGs, identification strategies, policy response mediation
- **Political economy** — Equilibrium analysis, path dependency, institutional portability
- **Decolonial epistemology** — Interrogating whose knowledge counts, WEIRD sampling bias, structural constraints
- **Actor-network theory** — Material thinking, reflexivity, strategic adaptation
- **Philosophy of science** — Mechanism plausibility, falsifiability, theory evolution

---

## Citation

If you use the CEF in research or analysis, cite it as:

> Shibli, S. (2026). Integrated Critical Evaluation Framework v6.1. *Zenodo*. https://doi.org/10.5281/zenodo.18867756

---

## Contributing

The CEF is a living document. If you've identified:
- **New failure modes** not yet named
- **Lens interactions** that warrant explicit guidance
- **Inquiry types** missing from Selective Application Guidance
- **Bugs or ambiguities** in the framework logic

Please open an issue or contact the maintainer.

Contributions should follow the design philosophy: auditability, causal clarity, epistemic discipline, intellectual authenticity.

---

## License

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

**You are free to:**
- Share and redistribute the framework
- Adapt, remix, and build upon it
- Use it for any purpose, including commercially

**You must:**
- Give appropriate credit and link to this license
- Indicate if you've made changes
- Apply the same CC BY-SA 4.0 license to any derivatives

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/

---

## Contact

Questions, feedback, or collaboration inquiries:

**Email:** syed.shibli@daymarmetric.com

---

## Acknowledgments

The CEF was developed iteratively through application to:
- Cross-disciplinary academic writing
- Policy analysis and organizational evaluation
- LLM-assisted research workflows

Built in dialogue with Claude, ChatGPT, Gemini, and Copilot—demonstrating that AI tools can improve epistemically rigorous human reasoning when appropriately constrained and interrogated.
