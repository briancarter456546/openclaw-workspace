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
