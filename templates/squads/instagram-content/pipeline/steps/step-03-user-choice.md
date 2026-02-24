---
name: step-03-user-choice
type: checkpoint
nextStepFile: ./step-04-writing.md
outputFile: "{squad-root}/output/drafts/selected-idea.md"
---

# Step 3: User Choice (Checkpoint)

## Instructions

Present the ideas to the user and ask them to choose using AskUserQuestion.

Use the 5 ideas from the previous step as options. Include the title and hook for each.

Example:
```
Which idea should we develop into a full carousel?
```

Options derived from step 2 output:
- Idea 1: "{title}" — {hook}
- Idea 2: "{title}" — {hook}
- Idea 3: "{title}" — {hook}
- Idea 4: "{title}" — {hook}
- Idea 5: "{title}" — {hook}

## After User Chooses

Save the selected idea's full details to `{outputFile}` so the copywriter can reference it.

Confirm the selection:
```
Great choice! ✍️ Quill will now write the carousel based on:
"{selected title}"
```
