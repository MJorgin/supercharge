# Foundations

English companion to [the Chinese guide](../methods.md). Apply methods only when their assumptions fit; distinguish completed work from proposed validation.

## Ablation study
- **Use:** Assess a rule or component's contribution to a larger system.
- **Do:** Define an intact baseline and metric; remove one component at a time, keeping other conditions comparable. For generative tasks, use representative inputs, repeat trials, and consider blind scoring; test interactions when needed.
- **Limits:** Reliable improvement after removal suggests harm; reliable equivalence with a sufficiently sensitive test can suggest redundancy. Inconclusive differences do not prove redundancy. AI ratings are not real-world outcomes.

## Monte Carlo simulation
- **Use:** Explore uncertain outcomes when a model and defensible or explicitly assumed distributions can be specified.
- **Do:** Define the outcome, distributions and dependencies; sample repeatedly, verify the implementation, summarize probabilities and ranges, and test sensitivity to assumptions.
- **Limits:** Results are conditional on the model; more samples reduce sampling error, not model error. Do not report a simulation as run when it was not. For π, uniformly sample a square and use four times the proportion inside its inscribed circle.

## Pyramid principle
- **Use:** Organize a recommendation, presentation, or report for a specific audience.
- **Do:** Start with a supportable conclusion, group supporting arguments, then give evidence and actions. Adapt the structure to the user's narrative.
- **Limits:** Structure does not verify facts; label unsupported conclusions as hypotheses. Exploratory work need not lead with a fixed conclusion.

## Visual hierarchy and F-shaped scanning
- **Use:** Improve scanability of text-heavy screens and documents.
- **Do:** Arrange headings, grouping, contrast and spacing around the user's task; account for language, device and layout, and test with users.
- **Limits:** F-shaped scanning is observed in some contexts, not a universal eye path or a guarantee of design quality.

## Classic animation principles
- **Use:** Design character animation or motion.
- **Do:** Choose relevant principles such as anticipation, squash and stretch, follow-through, overlapping action, arcs and easing; specify timing and inspect the result.
- **Limits:** Not every principle fits every movement; generators may not follow instructions precisely.

## Progressive disclosure
- **Use:** Reduce overload where users face layers of information and actions.
- **Do:** Show what the current task needs first; reveal secondary features through discoverable controls, with clear feedback and navigation.
- **Limits:** Do not hide essential risks or frequent actions; excessive nesting hurts usability.

## Metaknowledge
- **Use:** Identify an approach when the problem or available methods are unclear.
- **Do:** Clarify the goal and constraints; compare candidate methods by inputs, costs and verifiable outcomes, and decide when to switch.
- **Limits:** Recognizing a name is not mastery or evidence of suitability.

## First principles
- **Use:** Challenge inherited assumptions when redesigning a process or solution.
- **Do:** Separate verified facts, assumptions, conventions and hard constraints; construct options from defensible foundations and check practical costs.
- **Limits:** Do not label guesses as fundamental facts; mature conventions may be better for routine, reversible tasks.

## Occam's razor
- **Use:** Compare explanations or solutions with comparable evidence and performance.
- **Do:** List necessary assumptions and what each explains; other things being equal, test the option with fewer unnecessary assumptions first.
- **Limits:** Simpler is not necessarily true; do not sacrifice essential evidence or constraints.

## Five whys
- **Use:** Investigate a recurring problem whose explanation is superficial.
- **Do:** Ask why iteratively; label supporting evidence and hypotheses, branch for multiple causes, and identify testable interventions.
- **Limits:** Five is not a required count; a chain of guesses does not establish a root cause.

## Fishbone diagram
- **Use:** Organize many possible causes of a problem.
- **Do:** Define the problem, group candidate causes under suitable categories, add evidence and prioritize tests.
- **Limits:** Entries remain hypotheses until verified; categories should fit the situation.

## Pareto analysis
- **Use:** Prioritize categories of complaints, failures or costs with usable data.
- **Do:** Define the metric; rank categories by frequency or impact and calculate cumulative shares; include cost of intervention.
- **Limits:** An 80/20 split is not guaranteed; rare high-consequence risks may deserve priority.

## Impact and feasibility assessment
- **Use:** Triage alternatives under resource constraints.
- **Do:** Compare expected impact, effort, risk and urgency; document evidence and uncertainty, including dependencies.
- **Limits:** Scores are discussion aids, not objective measurements; necessary enabling work may score poorly.

## Premortem
- **Use:** Identify preventable failure risks before a project or decision.
- **Do:** Imagine failure, list plausible pathways, prioritize risks and assign early signals, mitigation and owners.
- **Limits:** Imagined failures are not forecasts; proportion effort to risk.

## Decision matrix
- **Use:** Compare options against several decision criteria.
- **Do:** Apply hard constraints first, then score explicit criteria with stated weights and evidence; test whether changes in assumptions alter the ranking.
- **Limits:** Weights and scores can be subjective and cannot override hard requirements.

## Expected value and sensitivity analysis
- **Use:** Compare uncertain decisions with plausible probabilities and consequences.
- **Do:** Define outcomes, probabilities and costs; verify probabilities sum to one, calculate expected values, and vary key assumptions.
- **Limits:** Expected value alone does not capture liquidity constraints, irreversible loss, tail risk or risk tolerance.

## Controlled experiments and A/B testing
- **Use:** Evaluate whether a change causes a measurable difference.
- **Do:** Prespecify the hypothesis, metric and observation window; use a control and variant, randomize where possible, and assess uncertainty.
- **Limits:** Small samples, confounding and multiple simultaneous changes weaken causal claims. Never invent results.

## Minimum viable test
- **Use:** Test a critical assumption before costly full implementation.
- **Do:** Identify the most consequential falsifiable assumption; design a low-cost informative test and set criteria for proceeding, revising or stopping.
- **Limits:** Intent, demonstrations and actual purchases provide different evidence; do not remove conditions necessary for the test.

## MECE decomposition
- **Use:** Organize complex questions or work.
- **Do:** Choose a dimension and scope; separate parts with minimal overlap and adequate coverage, then identify priorities.
- **Limits:** Reality may overlap and information may be incomplete; decomposition does not replace evidence or action.

## Backward planning
- **Use:** Turn a clear objective and deadline into work.
- **Do:** Work backward from acceptance criteria through milestones, dependencies, owners, dates and the next step.
- **Limits:** Clarify or explore unclear objectives first; revise the plan when facts change.

## PDCA
- **Use:** Improve a process through repeated small cycles.
- **Do:** Plan an outcome and metric, implement a bounded change, check the result, and standardize or revise based on evidence.
- **Limits:** Without a metric or feedback, improvement has not been verified; match iteration speed to risk.

## Inversion
- **Use:** Reveal failure paths that a positive plan may overlook.
- **Do:** Reframe the goal as an outcome to avoid; identify plausible causes and prioritize prevention, detection or response.
- **Limits:** Do not replace urgent action or positive design with speculation; low-risk reversible tasks seldom need a formal exercise.

## Second-order thinking
- **Use:** Assess follow-on effects and stakeholder responses beyond an obvious immediate benefit.
- **Do:** Map likely consequences and time horizons; label assumptions and investigate material uncertainty.
- **Limits:** Long chains are not predictions; stop when further effects no longer inform the decision.

## Bottleneck analysis
- **Use:** Find a constraint limiting throughput in a multi-stage process.
- **Do:** Define output and process boundaries; inspect throughput, waits, work in progress and resource limits; validate and address the current constraint, then recheck.
- **Limits:** Without process data, bottlenecks are candidates, not proven causes; constraints can shift.

## Hypothesis-driven analysis
- **Use:** Investigate several plausible explanations with limited resources.
- **Do:** List competing hypotheses and existing evidence; identify observations that distinguish them; collect the most decision-relevant evidence and update.
- **Limits:** Alternatives may be missing; seek disconfirming as well as supporting evidence.
