## SHARED_STATE.md - Append-Only

Format for all writes:
## [domain] [ISO8601 timestamp] [agent_id]
STATUS: ...
SIGNAL: ...
DECISION: ...
CONFIDENCE: 0-100
SOURCE: memory/YYYY-MM-DD.md#section

Rules:
- Orchestrators append only; never overwrite
- Confidence score required on every write
- Workers read only; never write directly
