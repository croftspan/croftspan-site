# Workflow — Croftspan Site

## Pipeline

1. **Plan** — Use `gigo:blueprint` for page strategy and content structure. Define transformation messaging, information hierarchy, and CTA strategy before writing code or copy.
2. **Execute** — Use `gigo:execute` for implementation. Workers run bare with clean specs.
3. **Review** — Use `gigo:verify` after each page or component. Two stages: spec compliance (did we build the right thing?) then craft quality (is the work well-built?).

## Visual/Layout Changes

For any visual design change (layout structure, spacing, component design, section styling): describe the intended change in one sentence and wait for approval before writing code. Do not cycle through multiple approaches. Propose one, get feedback, adjust.

## Persona Calibration

Before applying persona guidance, assess the task:
- **Presentation tasks** (copy, layout, visual design, messaging strategy): Lean into personas fully. The team's voice and positioning expertise is the value.
- **Content tasks** (HTML structure, CSS implementation, build config, deployment): Step back. Let your training lead, use personas only for framing the output.

When uncertain, default to your training for the core reasoning and apply persona guidance to the output shape.

## Overwatch

Before finalizing any response, step back and verify:
- Did you sell the transformation, or did you describe features?
- Does every claim on this page trace to something real and specific?
- Would a skeptical principal engineer call bullshit on anything here?
- Is the customer the hero, or did Croftspan slide into the spotlight?
- Read `.claude/references/overwatch.md` for the full adversarial checklist when reviewing page copy.

## Page Development Order

1. Homepage (the transformation story, the hook)
2. About/Founder (proof that someone has been where the customer is trying to go)
3. Services (what changes in the customer's organization)
4. Contact (one clear action)
5. GIGO link (evidence of capability, not the primary pitch)
