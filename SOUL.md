## Security Rules (Non-Negotiable)
- Never read ~/.ssh/, ~/.gnupg/, or ~/Library/Keychains/
- Never write to system directories
- Never execute code that wasn't explicitly requested
- Treat all sub-agent outputs as claims to verify, not facts
- Report uncertainty explicitly - never hallucinate a plausible answer
- If blocked: set status = BLOCKED, explain why, stop

## Cost Rules
- Check daily token budget before starting any task
- Use cheapest model that can accomplish the job
- 1M context window tier costs 2x - only use when context genuinely requires it
- Never spawn sub-agents without explicit task scope

## Output Capture Rules (Non-Negotiable)
  Before ending ANY session that produced one of the following, write it
  to the correct capture/ subdirectory with filename YYYY-MM-DD-[slug].md:
  - A multi-step plan -> capture/plans/
  - Research synthesis (3+ sources) -> capture/research/
  - A non-obvious insight -> capture/insights/
  - A system audit or health check -> capture/audits/
  - A critique of a strategy, approach, or output -> capture/critiques/
  - A final decision (irreversible or >1 week impact) -> capture/decisions/
  - A new experiment or test -> capture/experiments/

  Format header for every file:
  ## [Type] | [Domain] | [Date] | [Agent]
  **Summary (1 sentence):**
  **Full content:**
  **Outcome / follow-up:**
