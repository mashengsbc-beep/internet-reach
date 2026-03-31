# GitHub

Use this reference when the task involves GitHub repositories, issues, pull requests, commits, releases, or “go learn from GitHub”.

## Default approach

1. If the user gives a GitHub URL, use it directly.
2. If the user gives `owner/repo`, inspect the repo directly.
3. If the user gives only a topic, use GitHub search before general web search.

## In this workspace

- `gh` is installed and authenticated.
- The built-in `github` skill is ready.
- `gh-issues` is also available for issue-centric workflows, but use it only when the task is actually about issue triage/fixing/PR follow-up.

## Typical evidence to collect

- Repo metadata: stars, forks, recency, license, language, topics
- README claims vs actual file structure
- Recent commits and release cadence
- Open issues / open PRs for maintenance signal
- Whether the implementation is real, thin glue, or mostly documentation/marketing

## Practical review lens

When analyzing a repo, distinguish:
- **Core idea** — what capability it unlocks
- **Execution quality** — whether the code and workflow support the promise
- **Operational burden** — auth, cookies, proxies, geo restrictions, external CLIs
- **Adoption fit** — personal workflow, research tool, prototype scaffold, or production dependency

## Suggested commands / checks

Use GitHub directly for structured inspection, for example:
- repo view / metadata
- README
- tree / key files
- recent commits
- open issues / PRs

Prefer concise evidence over exhaustive dumping.

## When to recommend against adoption

Say so clearly if a project is:
- mostly a wrapper around many fragile upstream tools
- dependent on cookies / unofficial APIs / MCP chains for core value
- costly to maintain relative to the user’s actual needs
- better used as inspiration than as a hard dependency
