# Brian Carl Skills

Practical AI skills for solo marketers and small marketing teams, built around editorial judgment, source fidelity, and useful outcomes.

## Available skills

| Skill | What it does |
| --- | --- |
| [Article Repurposer](skills/repurpose-articles/SKILL.md) | Turns an article into an X thread and LinkedIn post, compares three distinct hooks, recommends one, and preserves the author's wording. |
| [Hook Reviewer](skills/review-hooks/SKILL.md) | Reviews written, visual, and audible hooks, explains what works and what needs fixing, offers three distinct alternatives, and recommends an option to test. |

## Article Repurposer

The workflow has four parts:

1. **Source Editor:** reads the full article and extracts the argument, examples, and useful original phrases.
2. **Hook Editor:** compares different angles, checks their relevance and stakes, and recommends a defensible opening.
3. **Platform Writer:** adapts the selected angle into separate X and LinkedIn drafts.
4. **Final Editor:** checks the payoff, factual support, source wording, and conversion path.

Each run returns three hook options with a recommendation, finished drafts, and a short note identifying phrases retained from the article. The default goal is article visits and newsletter subscriptions.

The skill learns the user's voice from the current article and any supplied writing samples. It ships without a preset author, website, or voice profile. Use the [voice and project reference](skills/repurpose-articles/references/voice-and-project.md) as a guide to supplying personal preferences. Keep those preferences in separate user context so skill updates can preserve the public workflow without overwriting personal notes.

## Hook Reviewer

Start with why the hook matters to the particular viewer. Use specificity to make that relevance recognizable and emotion to make its significance felt. Apply credibility checks in proportion to the claim: context, examples, demonstrations, and sound reasoning can establish trust without an authority statement in every opening.

Each review returns:

1. The original hook or a baseline draft.
2. A **Keep**, **Sharpen**, or **Rebuild** verdict with specific feedback.
3. A compact checklist covering relevance, specificity, emotion, clarity, credibility, delivery, and the promised payoff.
4. Three distinct alternatives: a faithful refinement, a different emotional angle, and a different interest mechanism.
5. A recommendation, including keeping the original when it remains strongest.

The skill includes emotional language and formula banks. It can review a supplied hook or check one it drafts from supplied content. It also works alongside Article Repurposer while preserving that skill's source and voice constraints. Requests for a shorter review or a different format take precedence over the default response.

## Install

Use the [Skills CLI](https://github.com/vercel-labs/skills) with Node.js and npm installed. These commands install skills into supported agents such as Claude Code, Codex, and Cursor.

Choose skills and agents interactively:

```bash
npx skills add BrianCarl/brian-carl-skills
```

Install both skills globally, so they are available across projects:

```bash
npx skills add BrianCarl/brian-carl-skills --skill repurpose-articles review-hooks -g
```

Install only Hook Reviewer:

```bash
npx skills add BrianCarl/brian-carl-skills --skill review-hooks -g
```

To target a specific agent, append `--agent claude-code` or `--agent codex`. Omit `-g` to install into the current project instead.

Preview the available skills without installing:

```bash
npx skills add BrianCarl/brian-carl-skills --list
```

## Update

Updates are published to this repository. Skills installed through the Skills CLI can be refreshed manually; publishing a change does not automatically update someone's installed copy.

Update both global skills:

```bash
npx skills update repurpose-articles review-hooks -g
```

Update only Hook Reviewer:

```bash
npx skills update review-hooks -g
```

Use `-p` instead of `-g` for project installations. Review the [changelog](CHANGELOG.md) for published changes. Keep personal preferences and writing samples outside the installed skill folder, and supply them in your agent's context; an update may replace edited skill files.

## Use it

Keep the entire folder for the skill you want to use: `skills/repurpose-articles/` or `skills/review-hooks/`, including its supporting files. Import or install the folder using your agent's supported skill workflow.

If your agent does not automatically load skills, ask it to read `SKILL.md` and any referenced files before drafting.

Example requests:

> Use repurpose-articles to turn this article into an X thread and LinkedIn post. Compare three strong hooks and preserve my wording: [article URL or full text]

> Repurpose my latest article from [my website URL] for X and LinkedIn.

> Create only a LinkedIn post from this article.

> Use review-hooks to check this hook. Explain what works, suggest three alternatives, and recommend one: [hook]. Audience: [audience]. The content delivers: [payoff].

> Use review-hooks to write and review a hook for this content: [content].

Provide the full article text when the agent cannot access the URL. No publishing service or API key is required for drafting.

## What is included

Article Repurposer includes:

- `SKILL.md`: the coordinated workflow.
- `references/hook-editor.md`: hook comparison and editorial calibration.
- `references/voice-and-project.md`: author preferences and source language examples.
- `references/platforms.md`: X and LinkedIn delivery guidance.
- `references/validation-cases.md`: cases for testing the skill's behavior.
- `agents/openai.yaml` and `assets/icon.svg`: display metadata for compatible agents.

Hook Reviewer includes its self-contained `SKILL.md`, `agents/openai.yaml`, and `assets/icon.svg`.

## Scope

These skills prepare drafts and reviews. Posting and scheduling require a separate, explicitly authorized workflow. Hook selection is editorial judgment, not a guarantee of engagement or subscriber growth.

## Feedback

Use repository issues to share a concrete example, what failed, and what a better result should do. Avoid including private source material in public issues.
