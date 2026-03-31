# Evaluation

Use this reference when the task is not just to fetch information, but to judge whether a project, tool, workflow, or public resource is worth using.

## Five-part evaluation frame

### 1. Problem-solution fit
Ask:
- What pain does this actually remove?
- Is it solving a real repeated problem or just bundling convenience?
- Is the user likely to benefit in their current environment?

### 2. Reality of implementation
Check:
- Is there real code, tests, docs, and recent maintenance?
- Does the implementation support the README promise?
- Is it mostly glue around external tools, unofficial APIs, or fragile browser automation?

### 3. Operational burden
Separate:
- zero-setup usable now
- needs auth / API keys / cookies / proxies / extra binaries
- high-maintenance or high-breakage components

### 4. Risk profile
Watch for:
- unofficial APIs
- cookie-based auth
- scraping behind login
- geo/IP dependence
- dependence on many third-party tools
- production unsuitability despite demo usefulness

### 5. Absorb-vs-adopt decision
Use one of these outcomes:
- **Adopt directly** — already fits this workspace well
- **Adopt partially** — use certain ideas/tools only
- **Learn from, don’t depend on** — useful concepts, risky implementation
- **Avoid** — maintenance/risk outweighs value

## Output pattern

A good practical recommendation usually contains:
- **Usefulness:** high / medium / low
- **Best fit:** personal use / research / prototyping / production
- **Main upside:** what is genuinely valuable
- **Main constraint:** what makes it fragile
- **Recommendation:** adopt / adapt / observe / avoid

## Red flags

Call these out explicitly when present:
- README promise is much broader than code reality
- many integrations but shallow reliability checks
- requires many external CLIs for core value
- login/cookie flow is treated as “easy” but is operationally annoying
- support matrix is really “possible with caveats”, not “works out of the box"
