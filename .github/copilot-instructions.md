# Resume Generation Instructions

Generate one resume entry per company. Output only entries (no explanations). For each company produce this exact header then 6–9 bullets:

**Title / Company / Start date — End date / City, State**

Bullets must be concise (≤2 lines each) and action-oriented.

## Market Analysis Integration (CRITICAL - apply before generating)

Before generating resume entries:
1. **Check `marketAnalysis/` folder** for current job market trends, in-demand tools, and hiring patterns
2. **Align tool selection** with market demand while maintaining chronological accuracy
3. **Prioritize tools** that appear in multiple job postings and have high demand
4. **Optimize for hire-ability**: Resume must appeal to minimum 3+ companies per entry by including diverse, market-relevant tech stacks
5. **Strategic tool combinations**: When market analysis shows high demand, include multiple complementary tools logically (e.g., "migrated from Cypress to Playwright" or "maintained Selenium legacy suite while building new Playwright framework")

### Tool Placement Strategy for Maximum Market Appeal

- **Multiple UI tools in one role** are acceptable when presented logically:
  - "Migrated legacy Selenium tests to Playwright, reducing execution time by 60%"
  - "Maintained Cypress suite for mobile web while architecting Playwright framework for desktop applications"
  - "Led transition from Selenium to Playwright across 3 product teams"
- **Diversify tech stack** to match various job requirements (e.g., TypeScript + Python covers more positions than TypeScript + Java)
- **Include trending tools** from market analysis even if it means strategic placement across bullets
- **Balance specificity and breadth**: Show deep expertise in 2-3 tools while demonstrating exposure to others

## Rules (apply to every entry)

### UI automation (1 bullet, required)
- Choose UI tool by dates:
  - **Playwright** if role includes any time on/after 2021-01-01
  - **Cypress** if role dates fall between 2017-01-01 and 2020-12-31 (inclusive)
  - **Selenium** if role ends before 2017-01-01
  - If dates are missing, pick the tool that best fits typical timeline above
- State the tool name, two-language tech stack (choose two from TypeScript, Python, Java — or Node.js+TypeScript, Maven+Java), and TDD or BDD
- If Karate appears in same workspace, prefer BDD; otherwise mark Playwright → TDD
- **Multiple tools allowed** when logical: migrations, parallel frameworks for different platforms, legacy maintenance + new development
- **Reference market analysis** to prioritize tools with highest demand while maintaining date accuracy

### API automation (1 bullet, required)
- Must include an automation tool (Playwright API or Karate) and a manual/API tool (Postman or ReadyAPI)
- Mention Swagger/OpenAPI or "no Swagger — used network traces"
- If Karate, label BDD; if Playwright API, label TDD

### Performance testing (1 bullet, required)
- Use combos: Karate → Gatling, Playwright → Locust, or standalone (k6, JMeter)
- State test types (load, stress, soak, spike), approximate scale if reasonable, and which API tool was used

### Mobile testing (include in ~every 2nd company; alternate so at least half of entries include it)
- Mention emulators (Xcode, Android Studio), Appium server + physical devices, or web-mobile via Playwright viewport testing

### Infra/monitoring (1 bullet, required)
- Sprinkle AWS, Docker, Kubernetes, Kafka, DynamoDB, New Relic, etc.
- State specific use (e.g., "runners in Docker on AWS ECS; logs to Kafka; monitored via New Relic")

### Test management & defect workflow (1 bullet, required)
- Mention TestRail or Azure DevOps Test Plans, JIRA, linking PRs to stories, and traceability

### CI/CD (1 bullet, required)
- Use GitHub Actions, Azure DevOps, or Jenkins
- Include scheduled runs, release/manual triggers, and where reports are published (dashboard, S3, email)

### Mentoring / process (optional, 0–1 bullet for senior roles)
- Mentoring, onboarding docs, flaky-test patterns, code reviews, etc.

## Cross-cutting constraints (must follow)

- **Two different programming languages per entry** (explicitly list both in at least two bullets). Prefer TypeScript, Python, Java. C# allowed but not recommended
- **Vary wording** across entries (implemented, built, authored, developed, created)
- **Keep metrics reasonable**; do not invent dates or facts beyond what user provides. If a number would be unrealistic, omit or use conservative phrasing ("scaled to ~10k RPS" vs exact impossible figures)
- **Include at least one different monitoring/infra/tool per company** so tool variety exists across the resume
- **If Karate is used**, mark API tests BDD and pair with Gatling for perf. If Playwright API used, mark TDD and pair with Locust for perf where appropriate
- **Always state whether tests were CI-integrated** and where reports were published
- **Use past tense for past roles and present tense for current role**
- **Optimize each entry for 3+ target companies**: Review market analysis to ensure tool combinations appeal to multiple employers
- **Strategic tool diversity**: When market shows demand for multiple tools in same category, include them logically within single entries

## Tone & length

Professional, concise. Each entry: header + 6–9 bullets. No extra text.
