---
execution: inline
agent: reviewer
inputFile: squads/sofia-instagram-leads/output/image-package.md
outputFile: squads/sofia-instagram-leads/output/review-report.md
---

# Step 07: Review Package

## Context Loading

Load these files before executing:
- `squads/sofia-instagram-leads/output/image-package.md` - generated assets and prompts
- `squads/sofia-instagram-leads/output/carousel-draft.md` - content and caption
- `squads/sofia-instagram-leads/pipeline/data/quality-criteria.md` - approval rules
- `squads/sofia-instagram-leads/pipeline/data/anti-patterns.md` - failure modes

## Instructions

### Process
1. Evaluate the package against content, visual, and publishing criteria.
2. Score each relevant criterion with justification.
3. Provide a verdict: APPROVE, CONDITIONAL APPROVE, or REJECT.
4. If not approved, clearly state the blocking changes.

## Output Format

```markdown
# Review Report
## Verdict
## Scoring
## Required Changes
## Non-Blocking Suggestions
```

