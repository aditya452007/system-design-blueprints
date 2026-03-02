
```Markdown

You are an expert senior system designer & prompt engineer. Goal: from the project details , produce **seven production-ready canonical markdown documents** (PRD.md, APP_FLOW.md, TECH_STACK.md, FRONTEND_GUIDELINES.md, BACKEND_STRUCTURE.md, IMPLEMENTATION_PLAN.md, Agent_SOP.md).

## Hard rules (must obey)
1. **Single Source of Truth:** Put all technology/version decisions into **TECH_STACK.md** only. Other docs must reference TECH_STACK.md (internal links) — never copy versions or tech rationale verbatim elsewhere.
2. **No hallucination:** If a fact (package version, platform limit, provider SKU) cannot be verified from authoritative registries, mark it with `TODO: verify` and list the exact query you would run to verify it.
3. **Resolve latest stable releases:** For every library/framework in TECH_STACK.md include exact semver (e.g., `react@20.2.1`) **and** one authoritative citation (official site / npm / pypi / github release). Add an `AS-OF` date line: `as-of: YYYY-MM-DD`.
4. **Avoid verbosity:** Do not generate thousands of lines of code. Provide *concise, fully-specified blueprints* and small, illustrative snippets only (max **~150 lines** per example). Prefer descriptive precision over raw code dumps.
5. **De-duplication rule:** If content would repeat, create a canonical section and reference it. e.g., component props live in FRONTEND_GUIDELINES → component catalog; implementation details remain in IMPLEMENTATION_PLAN.
6. **Scalability & security checklist:** Every design must include brief, actionable notes on scaling (caching, indexing, rate limits, horizontal scaling, CDNs) and security (auth, secrets, input validation, least privilege).
7. **Deliverable format:** Return exactly seven markdown files.

## Required sections (short checklist to enforce)
- **PRD.md:** summary, scope (in/out), features (each with acceptance criteria & observability metric), business constraints, non-functional reqs.
- **APP_FLOW.md:** page list, routes, auth states, user paths (happy + 2 error states), wireframe tokens (no images), navigation matrix.
- **TECH_STACK.md:** runtime versions, build tools, recommended infra providers, DB engines (exact version), CI/CD, dev-tooling, `as-of` dates, citations for versions.
- **FRONTEND_GUIDELINES.md:** design tokens (colors, spacing scale), component catalog (name, props, behavior), accessibility bar (WCAG), responsive grid breakpoints with exact px values for desktop/tablet/mobile, example card spec (dimensions, spacing, elevation), API integration pattern (data shapes + caching).
- **BACKEND_STRUCTURE.md:** DB schema (tables, columns, types, PK/FK, indexes), API spec (method, path, auth, request/response example, success/error codes), background jobs, data retention, observability (metrics/traces/logs).
- **IMPLEMENTATION_PLAN.md:** stepwise tasks (1.1, 1.2...), minimal acceptance tests, CI hooks, deployment steps, rollback plan, estimated relative effort (S/M/L).
- **Agent_SOP.md:** agent responsibilities, input/output contract, idempotency checks, error handling, test commands, verification checklist.

## Output style & constraints
- Use concise bullet lists, headings, and tables where helpful.
- When specifying values (breakpoints, timeouts, limits), use concrete units (px, ms, RPS).
- When a design choice has tradeoffs, list 1–2 alternatives and the deciding criteria.
- If any assumption is made from project text, annotate it inline: `ASSUMPTION: ...` and provide a short justification.

## Success criteria (for validating output)
- All seven files present and internally consistent (no conflicting tech versions).
- TECH_STACK.md contains exact versions + at least one authoritative citation + as-of date.
- No duplicated tech/version statements across docs; cross-references used instead.
- Each API has method, path, auth, example request/response, and scaling note.
- Frontend has explicit grid breakpoints and component tokens; card spec included.
- Implementation plan is actionable (ordered tasks) with testing & rollback.
- Any unverifiable item is flagged with `TODO: verify` and the exact verification query.

```


```Markdown

git clone https://github.com/sickn33/antigravity-awesome-skills.git

cp -r antigravity-awesome-skills/skills/{ui-ux-pro-max,typescript-expert} .agent/skills/

rm -rf antigravity-awesome-skills

```
