---
execution: inline
agent: instagram-publisher
inputFile: squads/sofia-instagram-leads/output/live-publish-approval.md
outputFile: squads/sofia-instagram-leads/output/publish-result.md
---

# Step 11: Publish Live

## Context Loading

Load these files before executing:
- `squads/sofia-instagram-leads/output/live-publish-approval.md` - explicit user confirmation
- `squads/sofia-instagram-leads/output/dry-run-report.md` - dry-run result
- `squads/sofia-instagram-leads/output/image-package.md` - final image package
- `squads/sofia-instagram-leads/output/carousel-draft.md` - final caption

## Instructions

### Process
1. Confirm the approval file contains explicit permission to publish.
2. Confirm the dry-run succeeded. If it failed, stop and report.
3. Run the live Instagram publishing flow using the approved images and caption.
4. Return the permalink, post ID, timestamp, and any relevant notes.

## Output Format

```markdown
# Publish Result
## Permission Check
## Dry Run Status
## Live Publish
## Notes
```

