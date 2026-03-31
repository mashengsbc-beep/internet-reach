---
name: internet-reach
description: Structured internet research and cross-platform content access for this OpenClaw workspace. Use when the user asks to search, inspect, summarize, compare, or learn from public information on GitHub, websites, articles, docs, videos, RSS feeds, or developer/community platforms. Especially use when a request involves GitHub repos/issues/PRs, "go learn from GitHub", reading links, extracting practical takeaways from public resources, or deciding which retrieval path is most reliable in this environment.
---

# Internet Reach

Use this skill as a router for internet-facing research in the current OpenClaw environment.

## Core rule

Prefer the most direct, already-working access path in this workspace instead of broad web searching first.

Default order:
1. **GitHub tasks** → use the built-in GitHub capability (`gh` / `github` skill) first.
2. **Known URL provided by the user** → fetch/read the URL directly.
3. **General web research** → use web search, then fetch the best sources.
4. **Only mention unsupported external CLIs/MCP stacks as optional follow-up ideas** unless they are actually installed and needed.

## Workflow

1. **Classify the request**
   - GitHub / code / issues / PRs / repo learning → read `references/github.md`
   - Public web pages / docs / articles / RSS → read `references/web.md`
   - Videos / transcripts / channel discovery → read `references/video.md`
   - Community / social / forum-style sources → read `references/community.md`
   - Practicality / worth-using / should-we-adopt questions → read `references/evaluation.md`
   - Repeatable task flow needed → read `references/research-playbooks.md`

2. **Pick the lowest-friction path**
   - Prefer tools already available in OpenClaw (`gh`, `web_search`, `web_fetch`, direct repo inspection).
   - Do not assume extra CLIs from upstream projects are installed.
   - If the user gave a GitHub URL, use GitHub directly instead of search engines.
   - If the user gave a normal webpage URL, fetch it before searching for mirrors or summaries.

3. **Use evidence in the right order**
   - Prefer source code, docs, changelog, issues, PRs, and commit history over marketing copy.
   - Read `references/evidence-order.md` when claims and reality may diverge.

4. **Assess practical reliability, not marketing claims**
   For any tool/project/source you evaluate, separate:
   - what works with zero setup
   - what works after auth/config
   - what is fragile, rate-limited, geo-blocked, or cookie-dependent
   - what is suitable for personal experiments vs production use
   - what should be adopted directly vs merely learned from

5. **Distill learning on purpose**
   - When the user asks you to learn from a source, read `references/learning-distillation.md`.
   - Extract durable methods, routing rules, and evaluation heuristics.
   - Do not overfit to one repo’s exact stack or marketing language.

6. **Produce two layers of output when asked to “analyze and learn”**
   - **User-facing analysis**: usefulness, risks, fit, recommendations.
   - **Agent-facing learning**: reusable rules, routing preferences, pitfalls, and what should become skill knowledge.
   - If useful, shape the reply using `references/output-patterns.md`.

## Environment-specific constraints

- This workspace already has working GitHub auth via `gh`; prefer it for GitHub learning tasks.
- Use OpenClaw-native web tools for URL fetch/search before inventing curl-heavy workflows.
- Do not turn upstream installer projects into mandatory dependencies unless the user explicitly wants installation.
- Favor a small, reliable skill over a large but brittle omnibus skill.
- When adapting external ideas into this workspace, read `references/openclaw-fit.md` and optimize for local reliability, not feature-count.

## Output standard

When evaluating an internet-facing tool/project, try to cover:
- **What it is**
- **What problem it actually solves**
- **What is genuinely usable here and now**
- **What is conditional / fragile / risky**
- **What parts are worth absorbing into this workspace’s long-term workflow**
- **Whether to adopt directly, adapt partially, learn-from-only, or avoid**

Be explicit when something is:
- good for personal use but weak for production
- a useful router/scaffold rather than a deep platform
- more valuable as a source of methods than as a dependency

When the user wants a decision, prefer a structured verdict:
- use `references/scoring.md` for a lightweight scorecard
- use `references/adoption-template.md` for the concrete adoption plan

## References

- `references/github.md` — GitHub-first learning and repo analysis
- `references/web.md` — URLs, docs, articles, RSS, and structured reading
- `references/video.md` — video/transcript research strategy
- `references/community.md` — forums, community signals, and fragile social sources
- `references/evaluation.md` — practicality and adoption judgment
- `references/evidence-order.md` — what evidence to trust first
- `references/output-patterns.md` — response structures for repo/tool analysis
- `references/openclaw-fit.md` — how to adapt outside ideas into this workspace
- `references/research-playbooks.md` — repeatable workflows for GitHub/project research
- `references/learning-distillation.md` — how to turn research into durable rules
- `references/scoring.md` — lightweight practicality scorecard
- `references/adoption-template.md` — concrete adopt/adapt/avoid output template
- `references/validation.md` — how to verify the skill works in this environment
- `references/project-types.md` — evaluate platforms, tools, and scaffolds differently
- `references/readme-vs-reality.md` — how to cross-check polished positioning against implementation reality
