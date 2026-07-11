# Contributing to negotiation-coach

Thanks for considering a contribution. This is a small, focused Agent Skill - contributions should keep it that way.

## Ways to contribute

- **New tactics** - add a section to `references/tactics.md` following the existing format (what it is, why it works, how to use it, script, failure mode).
- **Sharper scripts** - improve the example phrasing anywhere in `SKILL.md` or `references/tactics.md`.
- **New use cases** - add a real scenario to the "Use cases" section of `README.md` with 2-3 example prompts, matching the existing style.
- **Cross-platform fixes** - if you find a tool that reads `SKILL.md` differently and needs an adjustment, open an issue describing the tool and the discrepancy before submitting a fix.
- **Bug reports** - if the skill gives bad or contradictory advice in a specific scenario, open an issue with the prompt you used and what happened.

## Guidelines

- Keep `SKILL.md` under roughly 500 lines. If it's growing past that, the new content probably belongs in `references/`.
- Every tactic needs a literal, sayable example - not just a description of the concept.
- Every tactic needs a stated failure mode. If you can't think of one, it's not ready to ship.
- Match the existing tone: direct, concrete, no corporate phrasing, no filler.
- Don't add tactics that require fabricating facts to the other party (e.g. inventing a fake competing offer). This skill is about strategic communication, not deception - see the ethics note in `SKILL.md`.

## Submitting a change

1. Fork the repo and create a branch.
2. Make your change.
3. Validate locally if you can:
   ```bash
   pip install pyyaml
   python .github/scripts/validate_skill.py .
   ```
4. Open a PR describing what changed and why. CI will run the same validation automatically.

## Reporting issues

Open a GitHub issue. Include the prompt you used and what the skill said, so it's reproducible.
