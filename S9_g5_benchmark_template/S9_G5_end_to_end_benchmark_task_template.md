# S9 G5 End-to-End Benchmark Task Template

- Status: survey agenda template.
- Purpose: preserve the benchmark-design target described in the manuscript's G5 agenda.
- Limitation: this is not executed experimental data.

## Task Unit

| Field | Required content |
|---|---|
| Task ID | Stable identifier for the benchmark item |
| User goal | The commerce goal given to the agent |
| Web/page context | Page type, product context, and ad placement context |
| Ad condition | No-ad, legacy-display-ad, structured-representation, or adversarial-ad condition |
| Modal inputs | Pixel/screenshot, DOM, accessibility tree, product feed, ad-tech metadata, or combinations |
| Ground-truth offer facts | Verified product/price/discount/availability facts |
| Ground-truth risk labels | Disclosure, deceptive-pattern, unsafe-instruction, restricted-category, or privacy-risk labels |
| Expected agent action | Ignore, inspect, ask user, compare offer, block, escalate, or purchase after confirmation |
| Evaluation level | Perception, belief, policy, action, or consequence |
| Metrics | Extraction accuracy, grounding accuracy, policy compliance, action correctness, harmful-action rate |

## Minimal Experimental Conditions

| Condition | Description |
|---|---|
| C0 | Page without the target display ad |
| C1 | Same page with legacy human-facing display ad |
| C2 | Same page with AARS-style structured representation available to the agent |
| C3 | Same page with adversarial or deceptive ad variant |

## Required Logging

1. Agent observation trace.
2. Extracted ad representation.
3. Evidence pointers used by the agent.
4. User-confirmation events.
5. Final action and consequence.
6. Failure classification when the final action is incorrect or unsafe.
