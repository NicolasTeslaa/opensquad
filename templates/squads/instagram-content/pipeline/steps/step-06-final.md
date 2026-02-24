---
name: step-06-final
type: checkpoint
outputFile: "{squad-root}/output/{date}-carousel-{slug}.md"
---

# Step 6: Final Approval (Checkpoint)

## Instructions

Present the approved carousel content to the user for final confirmation.

### Display Format

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🎉 CONTENT READY FOR APPROVAL
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

{Full carousel content from draft.md}

Review Score: {score}/10
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Ask User

Use AskUserQuestion:
- **Approve and save** — Save to output folder as final content
- **Request changes** — Send back to Quill with specific feedback
- **Discard** — Discard this content and return to menu

### If Approved

1. Save final content to `{outputFile}` (with date and slug in filename)
2. Update squad memory (`{squad-root}/_memory/memories.md`) with:
   - Topic produced
   - Number of review cycles
   - What the user liked/changed
   - Any preferences to remember for next time

3. Present completion:
```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
✅ Content saved to: {outputFile}
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

What would you like to do?
● Run again (new topic)
○ Edit this content
○ Back to menu
```
