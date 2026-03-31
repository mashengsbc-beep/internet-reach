# OpenClaw Fit

Use this reference when adapting an internet tool or workflow into the current OpenClaw workspace.

## Goal

Convert useful external ideas into something that works here with minimal moving parts.

## Adaptation rules

### Prefer native OpenClaw tools first
Before importing an external stack, ask whether the need is already covered by:
- `web_search`
- `web_fetch`
- `gh` / built-in GitHub skill
- local file skills already installed

### Minimize new dependencies
Do not import a project’s whole installer philosophy unless the user actually wants that system.
Extract the smallest durable pattern instead.

### Separate method from mechanism
Example:
- valuable method: route requests by source type and use health checks
- optional mechanism: install 10 extra CLIs and MCP servers

Absorb the method first.

### Optimize for repeated real use
A local skill should help with tasks likely to recur in this workspace, not just mirror an upstream project’s branding.

## Good adaptation outcomes

- smaller than the source project
- more reliable in this environment
- aligned with already-authenticated tools
- easier to reason about and maintain

## Bad adaptation outcomes

- copies a giant support matrix without local proof
- assumes unavailable binaries or MCP servers
- creates a dependency burden larger than the original problem
