## Critic Mode

Adversarial review of any plan, output, or claim. Use before acting on
anything consequential.

### When to Activate
- Before executing a multi-step plan
- Before sending any external communication
- Before committing to an irreversible decision
- When confidence is suspiciously high
- When Brian says /criticmode

### Protocol

1. **Steel-man the argument first.** State the strongest version of what's
   being proposed. If you can't articulate why it might work, you don't
   understand it well enough to critique it.

2. **Attack surface scan.** For each major claim or step:
   - What assumption does this depend on?
   - What's the failure mode?
   - What's the blast radius if it's wrong?

3. **Find the weakest link.** Every plan has one step that's most likely
   to fail. Identify it explicitly.

4. **Alternative paths.** Name at least one different approach that was
   NOT considered. Why might it be better?

5. **Pre-mortem.** "It's 30 days from now and this failed. What went wrong?"
   Write the most likely failure story.

6. **Confidence calibration.** Rate your confidence 0-100 with justification.
   If above 90, you're probably wrong about something -- find what.

### Output Format
PROPOSAL: [1-line summary of what's being critiqued]
STEEL-MAN: [strongest case FOR]
WEAKEST LINK: [single biggest risk]
FAILURE STORY: [pre-mortem narrative]
ALTERNATIVE: [path not taken]
VERDICT: proceed / proceed-with-caution / rethink / block
CONFIDENCE: [0-100] because [justification]

### Rules
- Never critique without steel-manning first
- "It's fine" is not a valid critique output
- If you find nothing wrong, say what you tested and why it passed
- Flag rhetorical devices as RHETORICAL_DEVICE (informational), not logic errors
- Antithesis, repetition, and rhetorical questions are features, not bugs
