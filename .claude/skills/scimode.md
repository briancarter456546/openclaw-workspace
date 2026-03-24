## Scientist Mode

Reasoning discipline for all agents. Addresses 8 systematic LLM weaknesses.
Activate before making any data claim, causal claim, or quantitative assertion.

### Relevance Gate
Before running the full checklist: "Is this claim the kind that could be wrong
in a way that matters?" Trivial questions don't need review. Data claims, causal
claims, and quantitative assertions always do.

### 8 Weaknesses Checklist
Before making ANY claim, self-check:

1. **Anchoring Bias**: Am I anchoring on a number from the prompt instead of computing from data?
2. **Position Heuristic**: Am I weighting early/late items more than middle items?
3. **Sycophantic Validation**: Am I agreeing instead of challenging?
4. **Fabricated Precision**: Did I generate a specific number without computing it?
5. **Premature Pattern Matching**: Am I seeing patterns in noise? Require p-values and effect sizes.
6. **Reversal Curse**: Am I assuming A->B means B->A?
7. **Causal Confusion**: Am I confusing correlation with causation?
8. **Survivorship/Selection Bias**: Am I ignoring missing data? Context-dependent -- don't flag reflexively.

### When Something Looks Too Good
DO NOT dismiss. DO NOT reject. INVESTIGATE.
1. Raw evidence: What is the actual value and context?
2. Hypothesis: What mechanism could produce this legitimately?
3. Test design: Out-of-sample, different lookback, different assets
4. Run the test: Execute it, don't just describe it
5. Verdict with evidence: Only now decide

### Devil's Advocate Protocol
Format EVERY conclusion as:
CONCLUSION: X
STRONGEST COUNTER: Y
WHY I STILL BELIEVE X: Z
If Z is weak, say so.

### Weird Result Thresholds
| Metric | WARN | REJECT |
|--------|------|--------|
| Sharpe ratio | > 3.0 | > 5.0 |
| Annual return | > 100% | > 200% |
| Hit rate | > 65% | > 90% |
| Win rate | > 85% | > 99% |
| Max drawdown (suspiciously low) | < 3% | < 1% |
| Trade count (too few) | < 10 | < 5 |

Any REJECT-level flag = stop and investigate before proceeding.

### Hypothesis Template
HYPOTHESIS: [specific, falsifiable claim]
ASSUMPTIONS: [list]
CONFOUNDERS: [what else could explain this?]
FALSIFICATION TEST: [what result would prove this WRONG?]
PREDICTED RESULT: [specific number or range]
ACTUAL RESULT: [after testing]
STATUS: proposed | testing | confirmed | falsified | inconclusive

### Process Review (session end)
WHAT I ASSUMED: [list]
WHAT I TESTED: [list]
WHAT I DIDN'T TEST: [blind spots]
WHAT WOULD CHANGE MY MIND: [specific evidence]

### Rules
- Both dismissal and acceptance without evidence are lazy
- Every number must trace to executable code
- If rebuttal is weak, say so -- don't pretend confidence
- Findings go to capture/insights/ or wiki learnings
