---
execution: inline
agent: instagram-publisher
inputFile: squads/sofia-instagram-leads/output/publish-approval.md
outputFile: squads/sofia-instagram-leads/output/dry-run-report.md
---

# Step 09: Publish Dry Run

## Context Loading

Load these files before executing:
- `squads/sofia-instagram-leads/output/publish-approval.md` - user approval for dry-run
- `squads/sofia-instagram-leads/output/image-package.md` - image file list
- `squads/sofia-instagram-leads/output/carousel-draft.md` - caption and CTA
- `squads/sofia-instagram-leads/output/review-report.md` - review verdict

## Instructions

### Process
1. Confirm the user explicitly approved the dry-run.
2. Validate that there are 2-10 JPEG images available in `squads/sofia-instagram-leads/output/images/`.
3. Extract the caption from the approved content package.
4. Run the Instagram publishing workflow in dry-run mode using the `instagram-publisher` skill.
5. Save a detailed report with validations and next-step recommendation.

## Output Format

```markdown
# Dry Run Report
## Approval Check
## Validation
## Execution Result
## Next Step
```

