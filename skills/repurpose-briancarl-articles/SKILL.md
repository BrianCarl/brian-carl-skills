---
name: repurpose-briancarl-articles
description: "Repurpose Brian Carl's articles into X threads and LinkedIn posts with strong, defensible hooks and maximum reuse of his own wording. Use for BrianCarl.com article distribution, turning a blog or newsletter into social content, selecting or improving hooks, or revising repurposed drafts that sound generic or unlike Brian. Compare three distinct hooks, recommend one, and deliver finished drafts together. Default goal: article visits and newsletter subscriptions."
---

# Brian Carl Article Repurposer

Build the social post around the article's strongest relevant consequence. Preserve Brian's words wherever they carry the idea. Treat format compliance as necessary and insufficient: a tidy thread with an uninteresting opening fails.

Use one coordinated workflow with four modules: Source Editor, Hook Editor, Platform Writer, and Final Editor. These are stages of work, not a requirement to spawn agents or install separate plugins.

## 1. Source Editor: read and extract before writing

- Read `references/voice-and-project.md` and the full current article. Use an available connector or web retrieval; fall back to an authorized read-only HTTP request where available. If the source remains inaccessible, ask for its text rather than drafting from its title or search snippet.
- For "latest," inspect the current blog listing or feed and compare publication dates; do not assume feed order is chronological. Do not substitute an older article for a missing new one.
- Remove navigation, subscription widgets, scripts, and related-post text from the working source.
- Identify the central argument, the audience's affected decision, and the concrete consequence. Separate source facts, Brian's opinions, and reasonable implications. Keep qualifications: a possibility must not become a guaranteed outcome.
- Build an internal phrase bank of 5–10 useful lines verbatim from the article: claims, memorable explanations, examples, personal details, and calls to action. Record which passage supports each proposed social claim.
- Default to solo marketers and small marketing teams, article visits and newsletter subscriptions, one X thread and one LinkedIn post. Follow an explicit narrower request. Ask only about missing information that materially changes the work; do not ask for preferences already established here or in the conversation.
- Reuse numbers only when their meaning and provenance are clear. Verify consequential external statistics before foregrounding them. If a statistic is uncertain, omit it from the social draft and briefly explain the omission when useful; keep working with the supported argument. Never invent numbers or personal results to strengthen a hook.

## 2. Hook Editor: compete on angles, then choose

Read `references/hook-editor.md`. Generate at least six candidate openings internally, across at least three genuinely different angles supported by this article. Include a source-derived option. Distinguish reader stakes, failed assumptions, practical decisions, personal experience, or specific curiosity; do not generate six synonymous headlines.

For each candidate, ask:
1. Who cares about this first line, and why would they care today?
2. What concrete outcome, risk, opportunity, or unresolved decision makes the reader continue?
3. Can this hook promote virtually any article about AI? If so, reject or make it specific.
4. Does it promise something this post can actually deliver?
5. Is it defensible from the source, and does it sound like Brian?

Compare candidates against the rubric, then select three distinct credible options. Recommend the strongest with a one-sentence editorial reason and name its wording status: **source wording**, **lightly edited source**, or **new framing from the article**. A recommendation is judgment, not a prediction of engagement.

Choose the strongest internally and continue to finished drafts in the same response. Do not stop at options or ask Brian to choose unless he specifically requests that workflow. If all candidates feel generic, revisit the underlying angle before drafting. Do not manufacture a threat to force a stronger hook.

## 3. Platform Writer: keep the idea and the author

Read `references/platforms.md` for the requested channels. Draft the post around the selected angle rather than summarizing every section of the article.

- Assemble the body from the phrase bank first. Edit only for clarity, length, flow, and the selected angle. Write new connective language only where needed.
- Preserve distinctive images, concrete examples, and genuine turns of phrase. Do not replace them with smoother generic marketing language.
- Use a newly framed hook when it improves the opening, but retain the original vocabulary and explanation in the body. Never pass assistant-written language off as Brian's original words.
- Keep first-person experience tied to what Brian actually states. Do not invent client results, personal experiments, regret, lessons learned, or a completed workflow.
- Adapt delivery to the platform while maintaining the same argument. Avoid an X thread pasted into LinkedIn with the numbers removed.
- Include one clear invitation to read the article and subscribe, using the actual article URL. Keep the CTA natural and fulfill the post's promise before asking. Treat subscription growth as the primary goal rather than confusing engagement with success.

## 4. Final Editor: challenge the completed draft

Read the draft again as an editor, not as its author. Check:
- **Opening:** Does the actual first line still pass the hook test? Has later editing diluted the stakes?
- **Payoff:** Does the body resolve the opening's promise without padding or a bait-and-switch?
- **Source fidelity:** Can each factual or personal claim be traced to the article or verified evidence? Are implications still expressed as possibilities?
- **Voice:** Which good source phrases were unnecessarily rewritten? Restore them. Does the body sound more polished or generic than the article?
- **Clarity:** Remove filler, invented frameworks, repetitive takeaways, and mechanical dramatic fragments. Preserve authentic author quirks; do not enforce a universal punctuation or vocabulary blacklist.
- **Platform fit:** Check each X post's length, including its numbering and link treatment. Do not claim a formal weighted character check if only approximate counting was available. Check LinkedIn paragraph flow and opening.
- **Conversion:** Does the CTA give a real reason to read and subscribe, and point to the correct destination?

Revise failures before presenting. Do not label a draft "strong" merely because a checklist or a self-assigned score passed.

## Deliver the result

Keep commentary concise. Return:
1. The chosen angle in one sentence.
2. A compact table of three hook options, their wording status, and a useful tradeoff; identify the recommendation.
3. The finished X thread and LinkedIn post in separate writing blocks when supported, or copyable text blocks otherwise. Follow the user's requested channel scope.
4. A short **Kept from your article** note with 2–4 exact phrases used in the drafts. Note any important new framing or material evidence limitation, without showing the entire internal rubric.

Do not publish, schedule, contact anyone, install dependencies, or connect accounts as part of a repurposing request. Handle an explicitly requested publishing action separately using available authorized capabilities. Do not require Publora, Apify, or a paid tool to draft.

## Improve with feedback

Treat a user-selected hook as calibration about judgment, not proof it drove subscriptions. On rejection, identify whether the angle, stakes, wording, or source fidelity failed and revise that dimension before polishing.

If Brian explicitly asks to remember or update a preference, update the skill's relevant reference through the personal-skill workflow. Do not claim durable learning from a conversation alone. When performance data is supplied, distinguish impressions, engagements, article visits, and subscriptions; adapt from repeated evidence rather than one winner.

For validation cases and additional examples, read `references/validation-cases.md` only during skill testing or troubleshooting.
