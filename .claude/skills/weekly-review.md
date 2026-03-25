## Weekly System Review

  Run every Sunday. Not just wiki maintenance — a quality audit of whether
  the system is actually using its intelligence layers or just decorating.

  ### 1. Wiki Health
  - Contradictions between pages?
  - Stale entries (unchanged > 30 days but referencing "current" state)?
  - Gaps that should be filled vs gaps that should be deleted (30-day rule)?
  - Cross-links missing between related pages?

  ### 2. Capture Quality
  - How many captures this week? If zero, why — no sessions or skipping the step?
  - Are captures getting thinner (less detail, shorter summaries)?
  - Any captures that should have been wiki entries instead?

  ### 3. Graveyard Discipline
  - Were any strategies tested this week that resemble graveyard entries?
  - Any graveyard entries missing kill reasons?

  ### 4. Decorative vs Functional Check
  - Grep the week's agent outputs for phrases like:
    "as per our operating principle"
    "in line with our commitment to"
    "leveraging our continuous learning"
    If found WITHOUT a corresponding action (graveyard check, scimode run,
    wiki write, capture file), flag it. The principle is being cited but not used.
  - Did scimode actually catch anything this week, or just rubber-stamp?
  - Did criticmode produce any VERDICT other than "proceed"?
    If every critique says proceed, the critic is asleep.

  ### 5. Process Improvements
  - Any mistake made twice? If so, what gate failed and how do we fix the gate?
  - Any new pattern worth adding to a skill or SOUL.md?
  - Any rule in SOUL.md or CLAUDE.md that's being ignored? Remove or enforce.

  ### Output
  Write to wiki/meta/review-log.md with date and findings.
  Update wiki/meta/gaps.md.
  If a process change is needed, draft it and flag Brian for approval.
  Commit: git add wiki/ && git commit -m "weekly-review: YYYY-MM-DD"
