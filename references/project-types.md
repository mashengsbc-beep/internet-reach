# Project Types

Use this reference when a GitHub project’s category should change how you evaluate it.

## 1. Platform project

Examples: OpenClaw, OpenHands

Characteristics:
- broad scope
- many subsystems
- many open issues/PRs
- docs and repo structure are large signals

How to evaluate:
- judge architecture clarity and maintenance energy
- expect more open issues; volume alone is not failure
- look for active merges, docs depth, release/update cadence
- separate product breadth from operational complexity

Main risk:
- easy to be impressed by scope while underestimating setup/ops burden

## 2. Tooling project

Examples: Playwright MCP, focused CLIs, single-purpose libraries

Characteristics:
- narrower promise
- smaller surface area
- easier to compare README claims against real code

How to evaluate:
- check whether the core loop is clean and dependable
- inspect open issues for repeated edge-case failures
- weigh token/context cost if the tool is for agents

Main risk:
- narrower scope can still hide brittle edge cases in real-world usage

## 3. Aggregator / scaffold project

Examples: multi-tool installers, internet reachability bundles, wrappers over many upstream tools

Characteristics:
- value comes from integration and routing
- many features depend on external tools or unofficial access paths
- README often looks stronger than the true zero-config reality

How to evaluate:
- separate routing value from dependency burden
- identify which parts are actually zero-config
- ask whether the same value can be recreated more simply in the local environment

Main risk:
- convenience today becomes maintenance debt tomorrow

## Rule

Do not use the same standard for all repos. A large platform, a focused tool, and a scaffold/integrator should be judged differently.
