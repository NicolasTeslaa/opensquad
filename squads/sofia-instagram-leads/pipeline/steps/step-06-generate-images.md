---
execution: inline
agent: image-designer
format: instagram-feed
inputFile: squads/sofia-instagram-leads/output/approved-content.md
outputFile: squads/sofia-instagram-leads/output/image-package.md
---

# Step 06: Generate Images

## Context Loading

Load these files before executing:
- `squads/sofia-instagram-leads/output/approved-content.md` - approved carousel content
- `squads/sofia-instagram-leads/output/carousel-draft.md` - full slide copy and caption
- `squads/sofia-instagram-leads/pipeline/data/quality-criteria.md` - visual and publishing requirements
- `squads/sofia-instagram-leads/pipeline/data/anti-patterns.md` - visual mistakes to avoid

## Instructions

### Process
1. Define one visual direction for the whole carousel.
2. Create one image prompt per slide.
3. Generate JPEG images using `image-generator` and save them under `squads/sofia-instagram-leads/output/images/`.
4. Validate that the images feel like one coherent set.
5. Save a markdown package describing prompts, files, and observations.

## Output Format

```markdown
# Image Package
## Visual Direction
## Slide Assets
## Validation
```

