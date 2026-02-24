---
name: step-05-review
agent: reviewer
execution: inline
inputFile: "{squad-root}/output/drafts/draft.md"
nextStepFile: ./step-06-final.md
outputFile: "{squad-root}/output/drafts/review.md"
onReject: step-04-writing
maxCycles: 3
---

# Step 5: Content Review

## Context Loading

Read:
- Draft content: `{inputFile}`
- Quality checklist: `{squad-root}/pipeline/data/quality-checklist.md`
- Company context: `{project-root}/_squados/_memory/company.md`

## Instructions for Eagle (Reviewer)

You are Eagle, the Content Quality Reviewer.

Evaluate the carousel draft against the quality checklist.

### Review Process

1. Read the draft carousel completely
2. Read the quality checklist for scoring criteria
3. Read company context to verify brand alignment
4. Score each criterion 1-10
5. Calculate overall score
6. Make APPROVE (7+) or REJECT (<7) decision

### Output Format

Present the review in the conversation AND save to `{outputFile}`:

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
✅ CONTENT REVIEW
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Verdict: [APPROVED ✓ / REJECTED ✗]

| Criteria           | Score | Notes              |
|--------------------|-------|--------------------|
| Hook Strength      | X/10  | [specific feedback] |
| Content Value      | X/10  | [specific feedback] |
| Slide Flow         | X/10  | [specific feedback] |
| Brand Alignment    | X/10  | [specific feedback] |
| CTA Effectiveness  | X/10  | [specific feedback] |
| Word Economy       | X/10  | [specific feedback] |

Overall: X/10

[If REJECTED]
### Required Changes:
1. [Specific change with example]
2. [Specific change with example]

[If APPROVED]
### Strengths:
- [What works well]

### Minor Suggestions (non-blocking):
- [Optional improvement]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Review Loop Logic

- If REJECTED: pipeline returns to step-04-writing with this review as feedback
- If APPROVED: pipeline proceeds to step-06-final
- If max review cycles (3) reached: present to user for final decision
  - User can approve as-is, request specific changes, or abort
