# The Snap

*Whatever it takes to protect the project.*

When the operator asks to save progress, wrap up, or end a session, follow this protocol. Two jobs, in this order:
1. **Protect the project** — audit, sacrifice what has to go so what matters survives
2. **Capture learnings** — route new knowledge to the right file

Job 1 is more important. A lean project with missing knowledge outperforms a bloated one with everything.

## The Audit (every session, not optional)

Before saving anything new, audit the existing rules. This runs every time.

**1. Line check.** Scan each `.claude/rules/` file. Any file approaching ~60 lines needs content moved to `.claude/references/` with a "When to Go Deeper" pointer.

**2. Derivability check.** For each rule, ask: "Can the agent figure this out by reading the project files?" If the codebase now makes a rule obvious, let it go.

**3. Overlap check.** Rules that say the same thing in different words. Merge into one clear statement. Check cross-file redundancy. A rule should live in at most two auto-loaded locations.

**4. Staleness check.** Has any rule become irrelevant? Early-project rules often don't apply once the project matures. Let them go.

**5. Cost check.** For each surviving rule: "Is this worth loading on every single conversation?" If no, move to `.claude/references/`.

**6. Persona calibration check.** Do personas contain domain knowledge that belongs in references? Persona entries should be alignment signal only.

**7. Total budget check.** Count total lines across ALL `.claude/rules/` files. Target ~300 total, ~60 per file.

**8. Coverage check.** Has the project grown into areas the team doesn't cover? Offer to invoke `gigo:maintain` if so.

**9. Overwatch check.** Is the Overwatch section present in `workflow.md`? Is The Overwatch in `CLAUDE.md`? Is `.claude/references/overwatch.md` present?

**10. Review criteria check.** Compare `.claude/references/review-criteria.md` against current personas and standards. Flag staleness.

## Saving New Learnings

| Learning type | Where it goes |
|---|---|
| Brand/voice pattern | `.claude/rules/brand.md` |
| Conversion or layout insight | `.claude/rules/standards.md` → Quality Gates |
| Copy anti-pattern | `.claude/rules/standards.md` → Anti-Patterns |
| Workflow improvement | `.claude/rules/workflow.md` |
| Deep reference material | `.claude/references/{topic}.md` |

Before adding: Does it overlap? Is it derivable? Is it needed every conversation? Will it push past ~60 lines?

## If Nothing Was Learned

Still run the audit. Say "No new learnings. Rules audited — [clean / let go of X / moved Y to references]."
