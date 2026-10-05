# Brian Carl Skills

Practical AI skills for solo marketers and small marketing teams, built around editorial judgment, source fidelity, and useful outcomes.

## Available skills

| Skill | What it does |
| --- | --- |
| [Article Repurposer](skills/repurpose-articles/SKILL.md) | Turns an article into an X thread and LinkedIn post, compares three distinct hooks, recommends one, and preserves the author's wording. |

## Article Repurposer

The workflow has four parts:

1. **Source Editor:** reads the full article and extracts the argument, examples, and useful original phrases.
2. **Hook Editor:** compares different angles, checks their relevance and stakes, and recommends a defensible opening.
3. **Platform Writer:** adapts the selected angle into separate X and LinkedIn drafts.
4. **Final Editor:** checks the payoff, factual support, source wording, and conversion path.

Each run returns three hook options with a recommendation, finished drafts, and a short note identifying phrases retained from the article. The default goal is article visits and newsletter subscriptions.

The skill learns the user's voice from the current article and any supplied writing samples. It ships without a preset author, website, or voice profile. Optional personalization belongs in the user's local copy of the [voice and project reference](skills/repurpose-articles/references/voice-and-project.md), so the public skill stays reusable.

## Use it

Keep the entire `skills/repurpose-articles/` folder together, including its supporting references. Import or install the folder using your agent's supported skill workflow.

If your agent does not automatically load skills, ask it to read `SKILL.md` and the referenced files before drafting.

Example requests:

> Use repurpose-articles to turn this article into an X thread and LinkedIn post. Compare three strong hooks and preserve my wording: [article URL or full text]

> Repurpose my latest article from [my website URL] for X and LinkedIn.

> Create only a LinkedIn post from this article.

Provide the full article text when the agent cannot access the URL. No publishing service or API key is required for drafting.

## What is included

- `SKILL.md`: the coordinated workflow.
- `references/hook-editor.md`: hook comparison and editorial calibration.
- `references/voice-and-project.md`: author preferences and source language examples.
- `references/platforms.md`: X and LinkedIn delivery guidance.
- `references/validation-cases.md`: cases for testing the skill's behavior.
- `agents/openai.yaml` and `assets/icon.svg`: display metadata for compatible agents.

## Scope

This skill prepares drafts. Posting and scheduling require a separate, explicitly authorized workflow. Hook selection is editorial judgment, not a guarantee of engagement or subscriber growth.

## Feedback

Use repository issues to share a concrete example, what failed, and what a better result should do. Avoid including private source material in public issues.
