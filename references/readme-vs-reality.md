# README vs Reality

Use this reference when a project has a polished README and you need to check whether the implementation really supports the promise.

## What a strong README can and cannot prove

A strong README can prove:
- the project has a clear positioning
- the maintainers understand the value proposition
- onboarding may be thoughtfully designed

A strong README cannot prove:
- reliability in real use
- low setup burden
- consistency across all listed features
- production suitability

## Cross-check pattern

For each major README claim, ask:
1. Is there code or structure that clearly supports this?
2. Is there docs/changelog evidence that it is maintained?
3. Do issues/PRs suggest repeated breakage or caveats?
4. Is the claim really “works out of the box”, or “possible with setup and caveats”?

## Common mismatch patterns

### 1. Broad support matrix, uneven reliability
A repo supports many channels/integrations, but only some are likely to work smoothly in normal environments.

### 2. Great onboarding, high long-term ops cost
The getting-started story is smooth, but ongoing maintenance is expensive.

### 3. Polished narrative, thin implementation
The positioning is excellent, but the code is mainly wrappers or glue.

### 4. Real implementation, understated burden
The project is genuinely strong, but users may underestimate auth, infra, or troubleshooting load.

## Reporting rule

When you spot a mismatch, phrase it clearly:
- “The README promise is directionally true, but operationally conditional.”
- “The repo is strongest as a scaffold/router, weaker as a stable one-stop platform.”
- “The implementation is real, but the convenience claim hides substantial setup cost.”
