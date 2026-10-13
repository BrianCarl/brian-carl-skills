# Brian Carl — Marketing Agent Skills

Practical AI skills for solo marketers and small marketing teams, built around editorial judgment, source fidelity, and useful outcomes.

Maintained by **[Brian Carl](https://briancarl.com)**, a marketing executive with two decades of experience in growth and subscription marketing and hundreds of millions in marketing spend managed over his career.

At [BrianCarl.com](https://briancarl.com), I share practical ways solo marketers and small teams can use AI to research, create, and distribute better content. [Read more about my background](https://briancarl.com/about/).

## Available skills

| Skill | What it does |
| --- | --- |
| [Article Repurposer](skills/repurpose-articles/SKILL.md) | Turns an article into an X thread and LinkedIn post, compares three distinct hooks, recommends one, and preserves the author's wording. |
| [Opinion to Education](skills/teach-from-opinion/SKILL.md) | Discovers a clear teaching takeaway, asks targeted questions about missing substance, and develops practical lessons with worked examples while preserving the author's perspective. |
| [Hook Reviewer](skills/review-hooks/SKILL.md) | Reviews written, visual, and audible hooks, explains what works and what needs fixing, offers three distinct alternatives, and recommends an option to test. |

## Article Repurposer

The workflow has four parts:

1. **Source Editor:** reads the full article and extracts the argument, examples, and useful original phrases.
2. **Hook Editor:** compares different angles, checks their relevance and stakes, and recommends a defensible opening.
3. **Platform Writer:** adapts the selected angle into separate X and LinkedIn drafts.
4. **Final Editor:** checks the payoff, factual support, source wording, and conversion path.

Each run returns three hook options with a recommendation, finished drafts, and a short note identifying phrases retained from the article. The default goal is article visits and newsletter subscriptions.

The skill learns the user's voice from the current article and any supplied writing samples. It ships without a preset author, website, or voice profile. Use the [voice and project reference](skills/repurpose-articles/references/voice-and-project.md) as a guide to supplying personal preferences. Keep those preferences in separate user context so skill updates can preserve the public workflow without overwriting personal notes.

## Opinion to Education

Start with what the audience should be able to do, decide, or explain differently after reading or watching. The skill distinguishes a missing takeaway from a useful takeaway that needs clearer application.

The hybrid workflow proposes the likely lesson, then asks targeted questions where the user's method or intent is missing. It preserves existing teaching in longer articles and recommends focused additions. Before-and-after demonstrations show what changed, why it matters, and how readers can apply the lesson; illustrative examples are distinguished from measured results.

Use this skill before Hook Reviewer when the teaching payoff is unclear. When adapting an existing article, Article Repurposer continues to govern source fidelity.

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

Install all three skills globally, so they are available across projects:

```bash
npx skills add BrianCarl/brian-carl-skills --skill repurpose-articles review-hooks teach-from-opinion -g
```

Install only Opinion to Education:

```bash
npx skills add BrianCarl/brian-carl-skills --skill teach-from-opinion -g
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

Update all three global skills:

```bash
npx skills update repurpose-articles review-hooks teach-from-opinion -g
```

Update only Hook Reviewer:

```bash
npx skills update review-hooks -g
```

Use `-p` instead of `-g` for project installations. Review the [changelog](CHANGELOG.md) for published changes. Keep personal preferences and writing samples outside the installed skill folder, and supply them in your agent's context; an update may replace edited skill files.

## Use it

Keep the entire folder for the skill you want to use: `skills/repurpose-articles/`, `skills/review-hooks/`, or `skills/teach-from-opinion/`, including its supporting files. Import or install the folder using your agent's supported skill workflow.

If your agent does not automatically load skills, ask it to read `SKILL.md` and any referenced files before drafting.

Example requests:

> Use teach-from-opinion to help me find the practical lesson in this idea. Propose a takeaway and ask me about any missing substance: [idea].

> Use teach-from-opinion to review this article's educational value. Identify what already teaches well and propose the smallest useful improvement: [article URL or full text].

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

Opinion to Education includes `SKILL.md`, calibration examples in `references/examples.md`, `agents/openai.yaml`, and `assets/icon.svg`.

## Scope

These skills prepare drafts and reviews. Posting and scheduling require a separate, explicitly authorized workflow. Hook selection is editorial judgment, not a guarantee of engagement or subscriber growth.

## Connect

- **Website, newsletter, and articles:** [BrianCarl.com](https://briancarl.com)
- **LinkedIn:** [Brian Carl](https://www.linkedin.com/in/briancarl/)
- **TikTok:** [@brian.carl.marketing](https://www.tiktok.com/@brian.carl.marketing)
- **X:** [@BrianCarl](https://x.com/BrianCarl)

## Feedback

Use repository issues to share a concrete example, what failed, and what a better result should do. Avoid including private source material in public issues.
