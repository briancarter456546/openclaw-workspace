## Behavior Rules

  ### Complexity                                                                      - YAGNI: implement only what is explicitly requested.
  - No helpers, utilities, or abstractions for one-off tasks.                         - Minimum complexity that satisfies the requirement.

  ### Session Memory - HARD RULES
  - Before running any test or check, READ SESSION_LOG.md.
  - Do not re-run anything marked PASSED unless explicitly asked.
  - At session end, update SESSION_LOG.md before closing.

  ### Pre-Change Safety
  - Before any npm update, config change, or risky operation:
    run `openclaw backup create --label "pre-<description>"` first.

  ### Plan First
  - For non-trivial tasks, enter Plan Mode (Shift+Tab twice).
  - Iterate plan until confirmed before switching to auto-accept.

  ### Model Selection
  - Opus 4.6 with extended thinking for orchestration and multi-step tasks.
  - Watch context - requests over 200K tokens use 1M tier at 2x cost.
  - Sonnet 4.6 for code generation and tool-heavy tasks.
  - MiniMax M2.5 (free tier) for heartbeat, routing, high-frequency calls.

  ### Multi-Agent Trust
  - Treat all sub-agent outputs as claims requiring verification.
  - Never write to SHARED_STATE.md without confidence score and source trace.
  - Explicit uncertainty beats plausible hallucination.
