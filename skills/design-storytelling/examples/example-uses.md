# Design Storytelling example uses

## Prompt patterns

- “Here are my project notes. Help me find the strongest story.”
- “Critique this presentation for a cross-functional product review.”
- “I have 10 minutes with a VP. Adapt this story for that audience.”
- “Help me translate this usability finding into legitimate business relevance without inventing impact.”
- “This case study feels like a timeline of activities. Help me find the actual decisions.”
- “Rehearse this presentation with me and challenge the weak parts of the argument.”

## Worked example: from activity log to decision story

### Messy input

> We redesigned an enterprise data-import flow. We interviewed eight administrators, mapped the journey, reviewed support tickets, ran a workshop, created three concepts, and tested a prototype. Product wants better activation. Engineering says the import service is fragile. Support gets questions about stalled imports. We proposed a new progress screen. We do not yet have production results.

### Diagnosis

- **What the story appears to say:** The team's work changed the problem from a need for more onboarding instruction to a need for visible system state and safe recovery.
- **Strongest signal:** Administrators could not tell whether an import was working, failed, or safe to retry.
- **Highest-impact weakness:** The notes list activities but do not name the decision, alternatives, or evidence limits.
- **Missing information:** What did the eight administrators actually do? Which options were considered? What decision is needed now? Who owns it?
- **Writing problem:** The methods are given equal weight even though most do not change the audience's understanding.

### Improved structure

1. **Point:** Administrators do not primarily need another tutorial; they need visible import status and a safe recovery path. The team should test that focused change before funding a full rebuild.
2. **Situation and tension:** Import is necessary for activation, but the underlying service is fragile and its state is not legible to administrators.
3. **Insight and evidence:** In the small study, several administrators waited, retried, or sought help because they could not distinguish slow progress from failure. Support tickets suggest the problem also occurs in production, but inconsistent tagging prevents a prevalence claim.
4. **Decision and tradeoff:** A tutorial is faster but does not fix invisible state. Rebuilding the service may improve reliability but exceeds the current planning window. A status-and-recovery pilot addresses the observed confusion while accepting one engineering dependency.
5. **Business translation:** Confusing state can produce retries, slower onboarding, and avoidable support work. That makes activation, reliability, and support burden relevant; no revenue or retention impact is claimed.
6. **Action:** Product and Engineering decide whether to fund the bounded pilot. Measure completion, repeated attempts, recovery, and related support contacts before choosing broader investment.

### Why this is stronger

The revision does not force the project into five labeled sections or invent a successful outcome. It selects the evidence and choices that explain why the work mattered, translates them for the people in the decision, and makes the next action explicit.

## Adaptation example

The same story should change with the audience while preserving facts:

- **Engineering review:** emphasize service states, dependency risk, failure modes, and the boundary of the pilot.
- **Product review:** emphasize activation mechanism, sequencing, evidence limits, and the investment decision.
- **Portfolio interview:** emphasize the designer's reframing, influence, tradeoff judgment, collaboration, and what remains unproven.

These emphases are starting hypotheses. Ask what the actual audience owns and cares about rather than relying on job-title stereotypes.
