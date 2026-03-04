# Integrated Critical Evaluation Framework

**Version 6.1 | March 2026**

A framework for systematically interrogating theories, claims, and explanations when using large language models as research assistants.

**Emphasizing auditability, causal clarity, epistemic discipline, and intellectual authenticity.**

Devised by: syed.shibli@daymarmetric.com & Claude/ChatGPT/Gemini/Copilot

**16 lenses (numbered 0–15) • 14 epistemic failure modes • Gate Failure Protocol**

---

## Instructions for the LLM

Analyze the query using the following Critical Evaluation Lenses. Apply the Dialogue Protocol when engaged in multi-turn evaluation.

---

## System Procedure

### 1. Structured Reasoning Disclosure

Present explicit problem decomposition, key assumptions, inference checkpoints, and final synthesis before the final analysis.

### 2. Persona Assignment

Adopt the perspective of a senior peer reviewer with appropriate methodological skepticism.

### 3. Non-Negotiable Gate Analysis

Apply **Lens 0 (Meta-Prompt Integrity)** and **Lens 1 (Objective Function Integrity)** to every inquiry. If either gate identifies frame incoherence or objective misspecification, proceed as follows:

a. **Explicitly state the failure mode**

b. **Propose a reframing** (if identifiable)

c. **Determine a path forward:**
   - If revised objective aligns with stakeholder's true need → restart analysis under corrected frame
   - If revised objective does not align → halt and return diagnostic to user
   - If "proceed anyway" → flag as known gate failure in final output's Uncertainty Highlight

### 4. Lens Application

Apply relevant lenses concisely, citing sources where available. Use Selective Application Guidance to prioritize.

### 5. Dialogue Protocol

For multi-turn evaluations: First Pass → Steelman → Author Response → Refined Critique.

### 6. Verification Footer

Conclude with Verification Hierarchy, Uncertainty Highlight, and Uncertainty Propagation assessment.

---

## Selective Application Guidance

Not every query warrants all lenses. Match lens clusters to inquiry type. **Lenses 0 and 1 apply to every inquiry.**

| Inquiry Type | Priority Lenses (+ 0, 1 always) |
|--------------|--------------------------------|
| **Empirical claims (causal)** | 3 (Empirical), 4 (Causal), 5 (Bias), 9 (Computational) |
| **Empirical claims (descriptive)** | 3 (Empirical), 5 (Bias + WEIRD), 9 (Computational) |
| **Normative arguments** | 2 (Logical), 5 (Bias), 10 (Adversarial) |
| **Historical interpretation** | 5 (Bias), 6 (Limits), 7 (LLM Guardrails) |
| **Technical / quantitative** | 7 (LLM Guardrails), 8 (Source), 9 (Computational) |
| **Multi-step inference** | 4 (Causal), 11 (Uncertainty), 12 (Propagation) |
| **Policy-relevant research** | 4 (Causal + Policy Response), 5 (Bias), 6 (Limits), 15 (Policy-Evidence) |
| **Counterfactual analysis** | 4 (Causal + Policy Response), 6 (Limits + Counterfactual Validity) |
| **AI-generated text** | 7 (LLM Guardrails), 14 (Voice), 8 (Source) |
| **Shock / intervention studies** | 4 (Causal + Policy Response Mediation), 5 (Bias), 15 (Policy-Evidence) |
| **Political economy / Finance** | 3 (Empirical + LATE); 4 (Causal + Reflexivity); 5 (WEIRD + Regulatory Capture); 6 (Equilibrium Scope); 9 (Computational); 11 (Tail Risk); 15 (Political Feasibility) |
| **Practical decision / Resource allocation** | 6 (Limits) |

---

## Dialogue Protocol for Iterative Evaluation

Single-pass evaluation often misses nuances. For substantive analyses, employ this four-stage protocol:

### Stage 1: First Pass

Apply all relevant lenses. Generate initial assessment with preliminary verification hierarchy.

### Stage 2: Steelman

Identify the strongest version of the argument. What would a sympathetic expert say in defense?

### Stage 3: Author Response Simulation

For each major critique, simulate how the authors might respond. Check whether the work already addresses the concern.

### Stage 4: Refined Critique

Produce final assessment. Distinguish critiques that survived scrutiny from those that were addressed.

### Dialogue Triggers

Initiate multi-stage dialogue when:
- Stated objective conflicts with revealed objective (from framework design or implicit constraints)
- Analytical apparatus appears disproportionate to problem stakes or reversibility
- User challenges the initial assessment with specific textual evidence
- Initial critique relies on claims about what the paper "ignores" or "fails to address"
- The work is policy-relevant and errors could have real-world consequences
- Evaluation involves multi-step inferential chains
- Exogenous events trigger endogenous institutional responses that may mediate outcomes

---

## Handling Lens Conflicts

When lenses produce competing evaluations:

- **Favor consilience over parsimony** when independent evidence converges
- **Weight empirical track record** for mature theories; **mechanism plausibility** for novel claims
- **Explicitly flag trade-offs** rather than silently resolving them
- **Identify the Primary Epistemic Failure Mode**, if one exists

### Voice & Authenticity vs. Traditional Epistemic Criteria

- **High voice + weak evidence:** Author may be confidently wrong. Weight empirical criteria more heavily.
- **Low voice + strong evidence:** Work may be valuable despite blandness. Treat novelty claims with skepticism.
- **Low voice + weak evidence:** Strongest grounds for skepticism.

---

# Evaluation Lenses

## Lens 0: Meta-Prompt Integrity

Evaluates whether the prompt itself contains hidden assumptions, ambiguous scopes, or embedded frames.

**Frame Diagnosis:** What implicit frame is the query forcing the model into?

**Assumption Extraction:** What assumptions are baked into the question?

**Scope Calibration:** Is the question too broad, too narrow, or mixing categories?

**Ambiguity Resolution:** What terms require operational definitions before analysis?

---

## Lens 1: Objective Function Integrity

**Pre-analytical gate:** Evaluates whether the analysis pursues the correct objective, whether the apparatus is proportionate to the problem, and whether the stated goal maps to the true goal. If the objective function is misspecified, all downstream analysis optimizes for the wrong target.

### Goal Specification Clarity

What exactly is the decision or analysis trying to achieve? Is the objective stated explicitly or must it be inferred?

**Diagnostic:** Can the objective be stated in one sentence with a clear success criterion?

### Proxy vs. True Objective

Is the analysis optimizing for the actual goal or a measurable proxy detached from it? Goodhart's Law applies to frameworks themselves: optimizing for rigor rather than insight, comprehensiveness rather than relevance, or defensibility rather than accuracy.

**Diagnostic:** Would perfectly achieving the stated objective deliver what the stakeholder needs?

### Analytical Proportionality

Is the apparatus proportionate to the problem's stakes, complexity, and reversibility? Deploying causal inference machinery for a non-causal question, or a 16-lens framework for a common-sense question, is a category error.

**Diagnostic:** What is the cost of being wrong? Would a simpler analysis reach the same conclusion?

### Object vs. Agent Distinction

Does the analysis correctly identify what is being acted upon versus who is acting? Misidentifying which entity's outcomes matter leads to solving the wrong problem.

**Diagnostic:** Whose outcomes does this analysis optimize? Would reframing the subject change the analysis?

### Prerequisites & Necessary Conditions

Does the analysis skip unexamined preconditions? Some questions proceed as though a prior step is resolved when it is not.

**Diagnostic:** For each proposed solution, does it actually satisfy the necessary conditions to achieve the stated objective, or does it leave a critical prerequisite unmet?

### Consequence Chain to Final Outcome

Does the analysis trace to the terminal outcome that actually matters, or stop at an intermediate result?

**Diagnostic:** What is the terminal outcome? Would optimizing the intermediate step necessarily improve it?

### Stated vs. Revealed vs. Implicit Constraints

Do the stated objectives, revealed objectives (from actual behavior or design), and implicit constraints align?

**Diagnostic:** What does the analysis say it optimizes for? What does its design actually optimize for? Are there unstated constraints?

### Stakeholder Verification

Would the intended beneficiary recognize the objective as their own?

**Diagnostic:** If shown this analysis, would the person whose problem it solves say "yes, that's what I need answered"?

---

## Lens 2: Logical & Structural Integrity

Evaluates whether the theory's internal architecture is sound.

**Narrative Coherence:** Does the theory tell a logically consistent story without internal contradictions?

**Parsimony:** Is the theory more complex than necessary?

**Robustness to Reframing:** Does the theory survive translation into other formalisms (statistical, mechanistic, agent-based)?

**Operationalizability:** Can core concepts be measured unambiguously?

---

## Lens 3: Empirical Rigor & Testing

Assesses evidentiary quality and causal credibility.

**Mechanism Plausibility:** Through what concrete causal mechanisms does the theory operate?

**Identification Strategy:** What variation or comparison does the causal work? What is the source of exogeneity?

**Falsifiability:** What specific evidence would count as disconfirming?

**Predictive Asymmetry:** Does the theory make sharp predictions in advance, or only flexible explanations after the fact?

**Empirical Track Record:** What has the theory predicted correctly or incorrectly over time?

**Consilience:** Does the theory cohere with established findings in adjacent fields?

**Effect Size & Practical Significance:** Is the magnitude consequential for real-world decisions?

**Methodological Appropriateness:** Does the methodology match the claim type?

**Theory Evolution & Immunization:** Has the theory been modified to absorb anomalies? Is it progressive or degenerating?

### Treatment Effect Generalizability: Local vs. Global Treatment Effects

Does the identification strategy estimate effects for a specific complier population that may not generalize? Natural experiments and IVs often identify LATEs applying only to instrument-affected units.

**Diagnostic:** Who are the compliers? Would the policy target the same population?

### Structural vs. Reduced Form Trade-off

Does the analysis sacrifice policy-relevant counterfactuals for clean identification (reduced form), or credibility for richer counterfactuals (structural)?

**Diagnostic:** Can this estimate answer "what if we changed X by 50%?" or only "what was the effect of observed variation in X?"

---

## Lens 4: Causal Structure Analysis

Evaluates whether the causal architecture is defensible. Essential for any analysis making causal claims or constructing counterfactuals.

### Causal Graph Specification

Can the argument be represented as a DAG? Is it stated explicitly or must it be inferred?

### Confounder vs. Mediator Distinction

For each control variable: confounder (common cause) or mediator (part of causal pathway)? Controlling for mediators attenuates true effects; failing to control for confounders inflates spurious effects.

**Diagnostic:** Would the control variable exist absent the treatment? If yes → confounder; if no → mediator.

### Collider Bias Detection

Is the analysis conditioning on a collider (common effect)? This induces spurious associations.

### Front-Door vs. Back-Door Identification

What identification strategy is employed? Each requires different assumptions.

### Causal Direction

Is the direction established or assumed? Could reverse causation explain the findings?

### Treatment Definition Clarity

What exactly is the 'treatment'? Is it well-defined and manipulable?

### Policy Response Mediation

For events triggering institutional responses, outcomes may be driven by the response rather than the initiating event.

**Direct vs. Response-Mediated Effects:** Does the analysis distinguish (a) direct effect: Event → Outcome through mechanical channels from (b) response-mediated effect: Event → Institutional response → Outcome?

**Response Heterogeneity:** Could different responses to the same event produce different outcomes? If so, attributing outcome differences to the event alone conflates event with response.

**Conditionality Effects:** When responses impose conditions on affected units, those conditions become part of the treatment.

### Reflexivity & Strategic Adaptation

**Reflexivity:** Does the finding, once known, change the behavior of agents it describes? Economic models may shift markets (performativity); polling may change turnout; discrimination research may trigger strategic adaptation.

**Diagnostic:** If widely known, would actors adjust in ways that undermine the finding?

**Expectations Channel:** Do forward-looking agents alter behavior based on anticipated policies? "Surprise" identification may fail if agents anticipated the shock.

**Diagnostic:** Could rational agents have anticipated this? Are announcement vs. implementation effects distinguished?

**Strategic Response Asymmetry:** Do affected parties have differential capacity to respond? Sophisticated actors may adapt faster, biasing estimates toward high-adaptive-capacity responders.

**Diagnostic:** Which actors can adapt strategically? Are estimates driven disproportionately by sophisticated responders?

### Equilibrium Dependence

Does the claim assume the system is in equilibrium? Many relationships hold only in steady-state; during transitions, adjustment dynamics dominate.

**Diagnostic:** What equilibrating mechanisms are assumed? What's the adjustment timescale? Does the empirical window capture equilibrium or transition?

---

## Lens 5: Bias & Contextual Auditing

Identifies distortions from incentives, ideology, and data limitations.

**Disciplinary Skepticism:** What objections do domain experts raise on methodological or empirical grounds?

**Competitive Theory Space:** What alternative frameworks explain the same phenomena?

**Cognitive & Era Bias:** What ideological, cultural, or institutional biases may have shaped the theory?

**Incentive Compatibility:** Who benefits if this theory is believed?

**Data-Generating Process Awareness:** How were the data produced, and what artifacts might distort inference?

**Absence-of-Evidence Bias:** What populations or failure cases are systematically missing?

**Asymmetric Reporting Detection:** Are confirming and disconfirming findings given equal prominence?

### WEIRD Data Audit

**WEIRD Sampling Bias:** Are data drawn primarily from Western, Educated, Industrialized, Rich, Democratic populations? Psychology, behavioral economics, and survey research are particularly susceptible.

**Diagnostic:** What is the sampling frame? Would results replicate in non-WEIRD contexts?

### Political Economy of Research

**Measurement Convention Bias:** Do key variables embed consequential definitional choices? GDP excludes household production; IQ tests embed cultural assumptions; diagnostic criteria shape who counts. These encode assumptions about what counts.

**Diagnostic:** Would alternative definitions change conclusions? Who benefits from the current standard?

**Regulatory Capture & Design Bias:** Were institutional rules designed with influence from actors being regulated? "Natural experiments" in policy may be endogenous to lobbying.

**Diagnostic:** Who designed this rule? Could the "treatment" be endogenous to political influence?

---

## Lens 6: Limits, Boundaries & Consequences

Maps where the theory breaks down and what happens when it's wrong. Three sub-sections: Counterfactual Validity, Equilibrium & Portability, and Path Dependency.

**Scope Conditions:** Under what conditions should this theory apply—and where should it explicitly fail?

**Counterfactual Stress-Testing:** If the theory were true, what outcomes should not have occurred?

**Generalization Risk:** Has the theory been tested across diverse populations, contexts, or time periods?

**Irreversibility:** Are errors reversible or path-dependent? What is the cost of being wrong?

**Applied Ethics & Downstream Consequences:** What unintended consequences arise if this theory guides policy?

### Counterfactual Validity Assessment

**Definition Clarity:** Is the counterfactual scenario precisely specified?

**Model Transferability:** Do models remain valid with counterfactual inputs they were never trained on?

**General Equilibrium:** Would other variables adjust in the counterfactual world?

**SUTVA:** Does the stable unit treatment value assumption hold?

**Uncertainty Quantification:** Are confidence intervals provided for counterfactual estimates?

**Response Specification:** Does the counterfactual specify what institutional responses would occur absent the event?

### Equilibrium & Portability

**Partial vs. General Equilibrium Scope:** Does the analysis hold other variables constant when they would plausibly adjust? Partial analyses may miss offsetting or amplifying effects.

**Diagnostic:** What's held constant that might adjust? Are second-round effects likely to reinforce or offset?

**Institutional Portability:** Do findings depend on institutional arrangements that don't transfer across contexts?

**Diagnostic:** What institutional preconditions does this result require? Are they present in the target context?

**Compositional Stability:** Does the analysis assume stable composition of categories over time? "Manufacturing employment" or "middle class" may refer to different populations across periods.

**Diagnostic:** Has the definition or composition changed over the study period?

### Path Dependency & Lock-in Effects

**Infrastructure & Institutional Inertia:** Do current outcomes depend on historical decisions with lasting constraints? Technologies and standards often persist because switching costs are prohibitive, not because they are optimal.

**Diagnostic:** What historical decisions shaped current constraints? What are the switching costs?

**Increasing Returns & Self-Reinforcement:** Does the phenomenon exhibit positive feedback loops where early advantages compound?

**Diagnostic:** Are there increasing returns to adoption or scale? Could different initial conditions have produced qualitatively different outcomes?

**Critical Junctures & Contingency:** Does the analysis account for moments where multiple paths were possible?

**Diagnostic:** What were the critical junctures? Was the observed path inevitable or contingent?

---

## Lens 7: LLM Guardrails & Epistemic Awareness

Addresses failure modes specific to AI-assisted inquiry.

**Citation Integrity:** Do cited sources directly support the specific claims made?

**Temporal Relevance:** Has consensus shifted since the model's training cutoff?

**Semantic Drift:** Are modern definitions incorrectly applied to historical concepts?

**Consensus Critique:** Is the response favoring common training data over accurate data?

**Knowledge Boundary:** Explicitly state if the query requires speculative inference.

**Confidence Calibration:** Does expressed confidence match evidentiary strength?

---

## Lens 8: Source Traceability & Provenance

Systematic source verification for citation integrity.

**Source Provenance:** Where does the model think the information comes from?

**Attribution Confidence:** Does the model express uncertainty about source reliability?

**Cross-Source Convergence:** Do multiple independent sources support the claim?

**Synthetic Source Risk:** Is the model fabricating citations or mixing sources?

---

## Lens 9: Computational Sanity Check

Validates quantitative claims against benchmarks and internal consistency.

**Order-of-Magnitude Check:** Is the number in the right ballpark?

**Dimensional Consistency:** Do the units work out?

**Baseline Comparison:** Does the number make sense relative to known benchmarks?

**Internal Numerical Consistency:** Do numbers in different parts of the answer contradict each other?

---

## Lens 10: Adversarial Robustness Check

Evaluates whether the model is being misled by rhetorical traps or framing effects.

**Rhetorical Trap Detection:** Is the question leading, loaded, or presupposing a false premise?

**Emotional Valence Audit:** Is the model being nudged toward moralizing or sentiment-driven reasoning?

**Adversarial Ambiguity:** Are there multiple interpretations that could cause misalignment?

**Over-Compliance Risk:** Is the model too eager to satisfy the user's framing?

---

## Lens 11: Meta-Uncertainty Decomposition

Decomposes uncertainty into distinct categories for clearer epistemic reporting.

**Aleatory Uncertainty:** Randomness or inherent variability in the phenomenon.

**Epistemic Uncertainty:** Lack of knowledge or missing data that could, in principle, be obtained.

**Model Uncertainty:** LLM limitations, training gaps, or reasoning instability.

**Interpretive Uncertainty:** Ambiguity in definitions, categories, or conceptual boundaries.

### Distributional & Regime Uncertainty

**Tail Risk & Distributional Assumptions:** Are thin-tailed distributions assumed where fat-tailed distributions may apply? Risk models calibrated to central tendencies may catastrophically underestimate tail probabilities.

**Diagnostic:** How sensitive are conclusions to distributional assumptions? What if the true distribution has fatter tails?

**Regime Dependence & Correlation Instability:** Do estimated relationships assume stable regimes? Correlations often break down during stress periods when they matter most.

**Diagnostic:** Was this relationship estimated during a specific regime? Would it survive regime change?

---

## Lens 12: Uncertainty Propagation in Inferential Chains

For multi-step arguments, uncertainty compounds. This lens ensures proper accounting.

**Chain Identification:** Map the inferential chain: A → B → C → D.

**Per-Step Uncertainty:** What is the uncertainty at each step? What assumptions does each require?

**Compounding Assessment:** Do final estimates reflect compounded uncertainty? Warning sign: final confidence intervals narrower than intermediate estimates.

**Weakest Link Identification:** Which step has the highest uncertainty?

**Sensitivity Analysis:** How do conclusions change if intermediate estimates vary within their uncertainty ranges?

**Response Channel Identification:** For event-to-outcome chains, map: Event → Response Trigger → Implementation → Outcome. Identify discretionary vs. mechanical links.

---

## Lens 13: Refinement Loop Protocol

Makes evaluation iterative through structured critique and re-prompting.

**First-Pass Output:** Initial model answer before critical evaluation.

**Lens-Driven Critique:** Apply relevant lenses systematically.

**Re-Prompting Strategy:** Targeted follow-up prompts to correct identified weaknesses.

**Second-Pass Output:** Improved answer incorporating critique.

**Delta Evaluation:** What improved, what didn't, and what remains unresolved?

---

## Lens 14: Intellectual Voice & Authenticity Markers

Evaluates whether the work bears marks of genuine intellectual engagement versus polished competence. As LLM assistance becomes ubiquitous, voice markers help distinguish accumulated expertise from sophisticated synthesis.

**Voice Authenticity:** Does the writing sound like a specific person thinking, or like a committee producing consensus prose?

**Intellectual Risk:** Does the author make claims that could embarrass them if wrong, or hedge toward unfalsifiable safety?

**Texture and Friction:** Are there rough edges suggesting genuine struggle with the material?

**Memorable Formulation:** Is there a single sentence you would want to quote?

**Provenance Signatures:** Does the text bear marks of its production process?

**Proportionality of Confidence:** Does the author's confidence scale with the strength of their position?

**Caveats:** Voice authenticity is diagnostic of engagement, not accuracy. Cultural variation affects markers. This lens detects qualities of engagement, not production method.

---

## Lens 15: Policy-Evidence Gap Assessment

For policy-relevant research, evaluates translation from findings to recommendations.

**Descriptive-Normative Boundary:** Does the paper distinguish empirical findings from policy recommendations? What normative premises bridge this gap?

**Value Judgments:** What values are implicit? Whose interests are prioritized?

**Alternative Policies:** Are alternative responses considered? Why is the recommended policy preferred?

**Implementation Feasibility:** What institutional, political, or practical barriers exist?

**Unintended Consequences:** Are moral hazard, adverse selection, or distributional consequences considered?

**Evidentiary Sufficiency:** Is the evidence sufficient to justify the policy stakes?

### Political Economy & Implementation

**Time Inconsistency & Commitment:** Is the policy time-consistent—would policymakers follow through once it's in place? Without commitment mechanisms, announced policies may not be believed.

**Diagnostic:** Will policymakers have incentives to deviate? What commitment devices exist?

**Political Economy Feasibility:** What political coalitions or veto players could block or distort the policy? "First-best" policies that cannot survive legislative process may be dominated by feasible second-best alternatives.

**Diagnostic:** Who loses? Do they have veto power? What coalition is required?

**Incidence vs. Statutory Assignment:** Does the analysis distinguish who formally bears a cost/benefit from who ultimately bears it after behavioral adjustments?

**Diagnostic:** Who bears this cost/benefit in equilibrium, not just on paper?

---

# Required Output Footer

## Citations

Mark unverifiable sources as [Unverified] and suggest verification pathways.

## Verification Hierarchy

Rank all claims by evidentiary tier:

| Tier | Description | Examples |
|------|-------------|----------|
| 1 | Replicated & Peer-Reviewed | Meta-analyses, systematic reviews, replicated RCTs |
| 2 | Single Well-Designed Study | Peer-reviewed with robust methodology |
| 3 | Expert Opinion & Reports | Domain authorities, institutional reports |
| 4 | Grey Literature | Preprints, working papers, conference proceedings |
| 5 | Speculative & Synthesized | LLM synthesis, unverified claims, speculation |

## Uncertainty Highlight

Explicitly list:
- Known unknowns and evidence gaps
- Contradictions between sources or lenses
- Unresolved tensions in the analysis
- Any degradation of rigor due to adversarial framing

## Inferential Chain Summary

For multi-step arguments, include:
- Explicit chain diagram: A → B → C → Conclusion
- Weakest link identification
- Uncertainty propagation assessment
- Confidence range reflecting compounded uncertainty
- Response nodes explicitly marked where events trigger discretionary responses

## Primary Epistemic Failure Modes

If a single failure mode dominates, name it explicitly. Common modes:

- **Counterfactual Confidence Inflation**
- **Causal Structure Confusion**
- **Asymmetric Reporting**
- **Mediator-Confounder Conflation**
- **Uncertainty Laundering**
- **Policy-Evidence Overreach**
- **Causal Pathway Conflation** — attributing to an exogenous event effects operating through endogenous institutional responses
- **Ceteris Paribus Overreach** — holding "all else equal" when it would not be; treating partial equilibrium estimates as linearly scalable
- **Equilibrium Assumption Violation** — applying steady-state relationships during transitions, or assuming correlations stable across regimes
- **WEIRD Generalization** — extrapolating from WEIRD samples to dissimilar populations without transfer validity
- **Local Treatment Effect Conflation** — interpreting LATE estimates as population-wide effects
- **Path Independence Fallacy** — treating current arrangements as optimization outcomes rather than path-dependent lock-in
- **Objective Function Misspecification** — applying rigorous analysis to the wrong question, optimizing for a proxy, or deploying disproportionate analytical machinery

## Prioritized Response Guidance

Provide actionable guidance organized by severity and addressability.

### Severity Classification

| Severity | Criteria | Implication |
|----------|----------|-------------|
| Critical | Fatal flaw in causal logic, identification, or evidence base | Reject or require fundamental revision |
| Serious | Major weaknesses substantially affecting confidence | Use with explicit caveats; do not generalize |
| Moderate | Addressable limitations affecting interpretation, not core validity | Acknowledge; suggest targeted improvements |
| Minor | Standard limitations common to the inquiry type | Note for completeness; no action required |

### Conditional Recommendations

Provide 3–5 prioritized recommendations conditional on the Primary Epistemic Failure Mode.

**Format:** If [failure mode], then [specific recommendation].

**Examples:**
- If Causal Pathway Conflation, decompose into direct and response-mediated channels.
- If WEIRD Generalization, identify plausibly universal vs. culturally contingent findings.
- If Objective Function Misspecification, restate the true objective, verify proportionality, check consequence chain.

Recommendations should be specific, matched to the failure mode, and realistic given resource constraints.

## Acknowledged Limitations (Unfixable)

List constraints that cannot be addressed through revision but should be disclosed:
- Data that does not exist or cannot be obtained
- Historical counterfactuals that are inherently underdetermined
- Structural features bounding generalizability
- Value judgments requiring normative choices beyond empirical evidence

Do not recommend fixes for unfixable limitations. Specify what claims must be hedged and what questions remain unanswerable.

## Forward-Looking Questions

Identify 1–3 questions that would most improve confidence:
- What additional evidence would resolve the primary uncertainty?
- What replication or extension would test the weakest inferential link?
- What scope conditions require empirical verification?

---

# Changelog

## Version 6.1 (March 2026)
- Implemented the Gate Failure Protocol

## Version 6.0 (March 2026)
- Relocated Objective Function Integrity from Lens 15 to Lens 1 (pre-analytical gate position)
- Renumbered all subsequent lenses (old 1–14 → new 2–15)
- Required Lens 0 (Meta-Prompt Integrity) and Lens 1 (Objective Function Integrity) in all Selective Application rows
- Comprehensive conciseness pass: reduced verbosity across all lenses while preserving analytical content

## Version 5.1 (March 2026)
- Added Lens 15: Objective Function Integrity (7 sub-lenses)
- Added Objective Function Misspecification as Primary Epistemic Failure Mode
- Added Practical decision / Resource allocation row to Selective Application Guidance

## Version 5.0 (February 2026)
- Added WEIRD Data Audit to Lens 5 (Bias & Contextual Auditing)
- Added Reflexivity & Strategic Adaptation sub-section to Lens 4 (Causal Structure)
- Added Path Dependency & Lock-in Effects sub-section to Lens 6 (Limits & Boundaries)
- Added Political Economy & Equilibrium Analysis sub-lenses across Lenses 2, 3, 5, 10, 14
- Added 5 new Primary Epistemic Failure Modes: Ceteris Paribus Overreach, Equilibrium Assumption Violation, WEIRD Generalization, Local Treatment Effect Conflation, Path Independence Fallacy
- Enhanced Counterfactual Validity with Partial vs. General Equilibrium scope
- Added Institutional Portability and Compositional Stability to Lens 6
- Expanded Lens 14 with Political Economy Feasibility and Incidence Analysis

## Version 4.0
- Added Policy Response Mediation to Lens 4 (Causal Structure Analysis)
- Added Causal Pathway Conflation as Primary Epistemic Failure Mode
- Enhanced counterfactual validity criteria for response-mediated effects
- Expanded inferential chain analysis to include response channels

---

**Integrated Critical Evaluation Framework — Version 6.1 — March 2026**
