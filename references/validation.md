# Validation

Use this reference when checking whether the skill is actually usable in the current OpenClaw environment.

## Validation checklist

### 1. Structure validation
Confirm that the skill:
- has a valid `SKILL.md`
- has only necessary resource files
- can be packaged successfully

### 2. Real-path validation
Confirm at least one real task route works end-to-end.

For this workspace, the most important route is:
- GitHub project analysis via authenticated `gh`

### 3. Routing validation
Check that the skill chooses the right path for the source type.

Example:
- GitHub URLs should prefer `gh` / GitHub-native access
- generic docs/articles should prefer direct fetch or web search + fetch

### 4. Failure-mode validation
A blocked path is still useful information if it confirms the router should choose a better path.

Example:
- if generic web fetching of GitHub pages is blocked or degraded, that reinforces the rule to use GitHub-native access instead of treating GitHub as a normal webpage source

## Current confirmed validation for this workspace

- skill structure passes validation and packaging
- GitHub auth via `gh` works
- GitHub repo inspection works through `gh`
- generic page-fetch is not the preferred path for GitHub content here

## Rule

A skill is not "usable" merely because it packages successfully. It should also demonstrate at least one correct real-world route in the target environment.
