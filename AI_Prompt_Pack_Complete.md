# 🧠 AI Prompt Engineering Master Pack v2.0
## 50 Battle-Tested Prompts. Real Examples. Immediate Results.

**Price: $5 | 50 prompts across 6 categories | Bonus: Prompt Engineering Guide**

---

## What's Inside

This isn't a collection of "write a blog post about X" generic prompts. Each prompt here has been tested 10+ times, includes the exact output format to expect, and comes with a real example of what it produces.

### 💻 Code Generation (12 Prompts)

**1. Full-Stack Feature Builder**
```
You are a senior full-stack engineer. Build a complete [FEATURE] for a [APP_TYPE] application.

Tech stack: [STACK]
Requirements:
- Include error handling, input validation, loading states
- Write production-quality code with comments
- Include types/interfaces
- Add unit tests

Output format:
1. Architecture overview (3-5 bullets)
2. File structure (tree)
3. Code for each file (with file path as comment)
4. Test file(s)
5. README with setup instructions
```
*Best with: Claude Opus 4. Real example outputs a complete auth system in 5 files.*

**2. API Endpoint Generator**
```
Create a REST API endpoint for [RESOURCE].

Operations: [CRUD_OPERATIONS]
Framework: [FRAMEWORK]
Database: [DATABASE]

For each endpoint provide:
1. Route + HTTP method
2. Request/Response types (TypeScript)
3. Validation rules
4. Error responses (RFC 7807)
5. Controller/service/repository code
6. Integration tests

Security: Input sanitization, rate limiting, auth check, SQL injection prevention
```
*Best with: Claude Opus 4. Generates complete CRUD with auth middleware.*

**3. Database Schema Designer**
```
Design a database schema for [APPLICATION].

Expected scale: [SCALE]
Primary queries: [QUERY_PATTERNS]

Output:
1. ER diagram description
2. CREATE TABLE statements with constraints
3. Indexes with EXPLAIN rationale
4. Migration strategy
5. Seed data
6. Performance considerations

Constraints: UUID PKs, created_at/updated_at on every table, soft deletes, no N+1 patterns
```
*Best with: Claude Opus 4. Production-ready schema in one go.*

**4. CLI Tool Scaffolder**
```
Build a command-line tool that [PURPOSE].

Language: [LANGUAGE]
Minimal dependencies. Cross-platform.

Features: [FEATURE_1], [FEATURE_2], [FEATURE_3]

Output:
1. Single-file implementation with shebang
2. argparse/click with --help
3. Colored terminal output
4. Progress indicators
5. Actionable error messages
6. Shell completion script
7. README with examples
```

**5. Refactoring Master**
```
Refactor this code. Rules in order:
1. Extract reusable functions (DRY)
2. Replace magic numbers with named constants
3. Simplify complex conditionals (early returns, guard clauses)
4. Add type annotations
5. Improve naming
6. Add docstrings
7. Handle unhandled edge cases

[CODE]

Output: Before/after diff, one-line explanation per change, remaining concerns.
```

**6. Test Suite Generator**
```
Write comprehensive tests for this code.

[CODE]

Framework: [TEST_FRAMEWORK]
Coverage target: 85%+

For each function: happy path, null/empty input, invalid input, boundary values, concurrent access.
Also provide: mocks, integration test, test factories.

DO NOT modify original code. Only write tests.
```

**7. Docker & Deploy Setup**
```
Create production Docker + deployment for a [APP_TYPE] app.

Stack: [STACK]
Platform: [PLATFORM]

Provide: Multi-stage Dockerfile, docker-compose.yml, .dockerignore, health checks, .env.example, CI/CD (GitHub Actions), deploy script with rollback.

Security: non-root user, no secrets in layers, vulnerability scanning.
```

**8. Performance Optimizer**
```
Analyze and optimize this code.

[CODE]

Current: [METRICS]
Target: [TARGET]

Analyze: time complexity, memory hotspots, I/O blocking, unnecessary allocations, cache misses.
For each: explain problem, show optimized code, estimate improvement, note trade-offs.
Also suggest: caching strategy, lazy loading, parallelization, query optimization.
```

**9. Error Handling Hardener**
```
Harden error handling for production.

[CODE]

For every external call (HTTP, DB, file, queue):
- try/catch with specific types
- Timeout with defaults
- Retry (exponential backoff, max 3)
- Circuit breaker where appropriate
- Structured logging (correlation ID, context)

User-facing: never expose stack traces, friendly messages, next-step actions, error codes.
```

**10. Code Explainer for Onboarding**
```
Explain this codebase to a new developer.

[CODE]

Provide: High-level architecture (3 sentences), directory structure explained, key concepts, data flow, entry points, dependencies and why each, common tasks, gotchas.
Format as DEVELOPER_ONBOARDING.md.
```

**11. Microservice Extractor**
```
Extract [MODULE] from monolith to microservice.

[ARCHITECTURE_DESCRIPTION]
[CODE]

Provide: boundary analysis, API contract (OpenAPI), data migration plan, strangler fig pattern, backward compatibility strategy, rollback plan, new service scaffold, integration tests.
```

**12. GitHub Actions CI/CD**
```
Create CI/CD pipeline for [PROJECT_TYPE].

Stack: [STACK]

Stages: Lint → Type Check → Test (parallel) → Security Scan → Build → Deploy Preview → E2E → Deploy Production (manual gate)

Requirements: cache deps, matrix testing, Slack notifications, only deploy on main.
```

### 🔒 Code Review & Debugging (8 Prompts)

**13. Security Vulnerability Scanner**
```
Audit this code against OWASP Top 10.

[CODE]

For each finding: severity (Critical/High/Medium/Low), CWE ID, vulnerable line, attack scenario, exact fix, prevention.

Also check: hardcoded secrets, unsafe deserialization, XXE, mass assignment, missing authZ, CORS misconfig.
```

**14. Bug Root Cause Analyzer**
```
Debug this issue.

Symptom: [WHAT_HAPPENS]
Expected: [WHAT_SHOULD_HAPPEN]
Steps: [REPRODUCTION]
Environment: [ENV]

[CODE]
[ERROR_LOG]

Think step by step: trace execution, find root cause (not symptom), explain why, 3 fixes ranked by safety, best fix with code, regression test, prevention.
```

**15. Dependency Audit**
```
Audit all dependencies in [PACKAGE_FILE].

Check each: latest version, known CVEs, maintenance status (last commit), alternatives if abandoned, license compatibility.

Output: prioritized list of issues with upgrade/removal recommendations.
```

**16. API Security Review**
```
Review these API endpoints for security.

[OPENAPI_SPEC]

Check: auth on every endpoint, rate limiting, input validation, SQL injection, mass assignment, IDOR, excessive data exposure, missing security headers.

For each issue: endpoint, vulnerability, severity, fix.
```

**17. Code Smell Detector**
```
Find code smells in this codebase.

[CODE]

Look for: god functions, duplicate code, long parameter lists, feature envy, data clumps, primitive obsession, switch statements, commented-out code.

For each: location, smell type, why it's a problem, refactoring suggestion.
```

**18. Race Condition Hunter**
```
Find potential race conditions in this concurrent code.

[CODE]

Check: shared state without locks, check-then-act patterns, non-atomic operations, improper use of async/await, missing transaction isolation.

For each: scenario, likelihood, impact, fix.
```

**19. Memory Leak Detector**
```
Find potential memory leaks.

[CODE]

Check: unclosed resources, circular references, growing collections, event listener accumulation, timer/interval not cleared.

For each: location, leak mechanism, reproduction, fix.
```

**20. Accessibility Audit**
```
Audit this UI code for accessibility.

[CODE]

Check against WCAG 2.1 AA: semantic HTML, ARIA labels, keyboard navigation, color contrast, focus management, screen reader compatibility.

For each issue: element, WCAG criterion, why it fails, fix.
```

### ✍️ Content Creation (10 Prompts)

**21. SEO Blog Post Generator**
```
Write an SEO-optimized blog post about [TOPIC].

Target keyword: [KEYWORD]
Audience: [AUDIENCE]
Length: [LENGTH] words

Structure: H1 with keyword, hook+problem+solution intro, 5-7 H2 sections, FAQ (5 questions), conclusion+CTA.

SEO: keyword in H1/first para/one H2/conclusion, secondary keywords, meta description (155 chars), internal/external link suggestions, image alt text.

Quality: no fluff, data with sources, actionable takeaways, professional but conversational.
```

**22. Viral Twitter/X Thread**
```
Write a 10-tweet thread about [TOPIC].

Style: Hook in tweet 1 that makes people stop scrolling. Each tweet one clear idea. Build to a payoff. End with CTA.

Rules: No hashtag stuffing. Numbers > adjectives. Personal experience angle. Max 280 chars per tweet.
```

**23. Product Launch Email**
```
Write a product launch email.

Product: [PRODUCT]
Audience: [AUDIENCE]
Key benefit: [BENEFIT]

Structure: Subject line (40 chars, curiosity + benefit), preview text, hero benefit, 3 features with mini-stories, social proof, limited-time offer, single CTA.

Tone: Like an email from a smart friend, not a corporation.
```

**24. Landing Page Copy**
```
Write high-converting landing page copy for [PRODUCT].

Sections: Hero (headline + subheadline + CTA), problem agitation, solution reveal, 3 feature+benefit pairs, social proof, pricing, FAQ, final CTA.

Rules: Benefits over features. One idea per section. Specific numbers. Active voice. Under 200 words total.
```

**25. LinkedIn Thought Leadership Post**
```
Write a LinkedIn post establishing authority on [TOPIC].

Structure: Bold claim hook, personal story (3-4 lines), lesson learned, actionable takeaway, question to drive engagement.

Rules: No hashtags at end. Single spaced lines. Real numbers. No humblebragging.
```

**26. YouTube Script Outline**
```
Create a YouTube video script outline.

Topic: [TOPIC]
Length: [LENGTH] minutes
Style: [STYLE]

Structure: Hook (first 5 seconds), intro (what viewer gets), 3-5 main points with timestamps, B-roll suggestions, pattern interrupt, CTA.

Include: thumbnail ideas, title options (3), first line of description.
```

**27. Case Study Template**
```
Write a customer case study.

Customer: [CUSTOMER]
Problem: [PROBLEM]
Solution: [SOLUTION]
Results: [METRICS]

Structure: Results headline, customer quote, problem section, solution section, implementation details, results with charts description, future plans, testimonial.
```

**28. SaaS Onboarding Email Sequence**
```
Write a 5-email onboarding sequence for [SAAS_PRODUCT].

Email 1: Welcome + quick win (send immediately)
Email 2: Key feature deep-dive (day 2)
Email 3: Social proof + case study (day 4)
Email 4: Advanced tip (day 7)
Email 5: Feedback request + upgrade prompt (day 10)

Each: subject line, preview text, body, CTA.
```

**29. Press Release**
```
Write a press release for [ANNOUNCEMENT].

Structure: FOR IMMEDIATE RELEASE, headline with keyword, dateline, lead paragraph (who/what/when/where/why), 2-3 body paragraphs with quotes, boilerplate, media contact.

Tone: Journalistic, factual. No marketing fluff.
```

**30. Sales Page That Converts**
```
Write a long-form sales page for [PRODUCT] ($[PRICE]).

Structure (AIDA): Attention (hero), Interest (problem deep-dive), Desire (solution + benefits + proof), Action (pricing + guarantee + CTA).

Elements: Price anchoring, objection handling (3), testimonials (3), money-back guarantee language, bonus stacking.
```

### 📊 Business & Strategy (8 Prompts)

**31. Business Proposal Writer**
```
Write a professional business proposal for [PROJECT].

Client: [CLIENT_TYPE]
Budget: [BUDGET]
Timeline: [TIMELINE]

Structure: Executive summary, problem statement, proposed solution, implementation plan (table), team, budget breakdown, ROI analysis, risk management, next steps.

Style: Professional but not bureaucratic. Specific numbers. Short sentences. Active voice. No AI clichés.
```

**32. Competitive Analysis**
```
Analyze [OUR_PRODUCT] against [COMPETITOR_1], [COMPETITOR_2], [COMPETITOR_3].

For each: pricing, key features, target market, strengths, weaknesses, market position.

Output: comparison matrix, our competitive moat, threats to address, opportunities to exploit, recommended positioning.
```

**33. Go-To-Market Strategy**
```
Create a GTM strategy for [PRODUCT].

Target: [MARKET_SEGMENT]
Budget: [BUDGET]
Timeline: [TIMELINE]

Sections: Market sizing (TAM/SAM/SOM), ideal customer profile, messaging & positioning, channel strategy (paid/organic/partnership), launch timeline (90 days), success metrics, budget allocation.
```

**34. Investor Pitch Deck Outline**
```
Create a pitch deck outline for [COMPANY].

12 slides: Problem, Solution, Market Size, Product Demo, Traction, Business Model, Competition, Competitive Advantage, Go-to-Market, Team, Financials, Ask.

For each slide: headline, 3 bullet points, suggested visual.
```

**35. Strategic Decision Memo**
```
Write a decision memo for [DECISION_TO_MAKE].

Structure: Situation (2 sentences), options (3 with pros/cons), recommendation, reasoning, risks & mitigations, next steps.

Rules: One page max. No attachments needed to understand. Clear recommendation, not more analysis.
```

**36. OKR Planning**
```
Create OKRs for [TEAM/PRODUCT] for [QUARTER].

Objective 1: [THEME]
- KR1: [Measurable outcome]
- KR2: [Measurable outcome]
- KR3: [Measurable outcome]

For each KR: baseline, target, measurement method, owner.

Rules: Objectives inspirational, KRs measurable. No activity-based KRs. 3-5 KRs per objective max.
```

**37. Pricing Strategy Analysis**
```
Analyze pricing for [PRODUCT].

Current: [CURRENT_PRICING]
Competitors: [COMPETITOR_PRICES]
Value metric: [HOW_CUSTOMERS_GET_VALUE]

Analysis: willingness-to-pay estimate, price sensitivity, tier recommendations, anchoring strategy, discount policy, when to raise prices.
```

**38. Quarterly Business Review**
```
Write a QBR for [TEAM/PRODUCT].

Sections: Key metrics vs targets, wins (3), losses (2), what we learned, strategic pivots, next quarter focus (3 priorities), resource needs.
```

### 📈 Data Analysis (7 Prompts)

**39. Data Storyteller**
```
Analyze this data and tell a compelling story.

[DATA_SAMPLE]
Context: [BUSINESS_CONTEXT]
Audience: [EXECUTIVES/TECHNICAL/GENERAL]

Provide: Executive summary (1 para), top 5 metrics, trends with % changes, anomalies, segments by [DIMENSIONS], correlations, 3-5 recommendations, caveats.

Output should make someone understand what matters in 60 seconds.
```

**40. SQL Query Optimizer**
```
Optimize this SQL query.

[QUERY]
EXPLAIN output: [EXPLAIN_OUTPUT]

Provide: rewritten query, index recommendations, explanation of each change, estimated improvement, trade-offs.
```

**41. Dashboard Designer**
```
Design a dashboard for [USE_CASE].

Audience: [ROLE]
Key decisions: [DECISIONS_TO_ENABLE]

For each section: metric/KPI, visualization type, dimensions, refresh frequency, alert thresholds.

Rules: Above the fold = most important. No pie charts. Comparisons over absolutes.
```

**42. A/B Test Analyzer**
```
Analyze this A/B test.

Control: [CONTROL_DATA]
Variant: [VARIANT_DATA]
Metric: [PRIMARY_METRIC]

Provide: statistical significance, confidence interval, effect size, practical significance, recommendation, whether to stop or continue.
```

**43. Cohort Retention Analysis**
```
Analyze user retention with cohort data.

[DATA]
Time period: [PERIOD]

Provide: retention curve description, drop-off points, segment differences, benchmarks comparison, recommendations to improve [WEAKEST_POINT].
```

**44. Forecasting Model**
```
Create a forecast for [METRIC].

Historical: [HISTORICAL_DATA]
Horizon: [FORECAST_PERIOD]
Seasonality: [YES/NO]

Approach: method choice with rationale, forecast values with confidence intervals, assumptions, scenarios (optimistic/pessimistic/base), accuracy assessment.
```

**45. Anomaly Detection**
```
Find anomalies in this time series.

[DATA]
Expected pattern: [NORMAL_DESCRIPTION]

For each anomaly: timestamp, value, expected value, deviation (z-score), possible explanation, recommended action.
```

### 🎨 Product Design (5 Prompts)

**46. Product Requirements Document**
```
Write a PRD for [FEATURE].

Context: [PRODUCT_CONTEXT]
Users: [PERSONAS]
Goal: [BUSINESS_GOAL]

Structure: Problem statement, success metrics, user stories, functional requirements, non-functional requirements, edge cases, out of scope, dependencies, launch plan, wireframe descriptions.

Prioritize: P0/Must, P1/Should, P2/Nice.
```

**47. User Story Map**
```
Create a user story map for [PRODUCT].

User: [PERSONA]
Journey: [END_TO_END_FLOW]

For each step: user goal, activities, tasks, story (As a... I want... so that...), acceptance criteria.

Organize by: backbone (critical path), walking skeleton (MVP), releases (v1, v2, v3).
```

**48. Design Critique**
```
Critique this UI design.

[DESIGN_DESCRIPTION]

Evaluate: visual hierarchy, affordance, consistency, cognitive load, error prevention, accessibility, mobile responsiveness.

For each issue: screenshot area, problem, severity, suggested fix.
```

**49. Technical Spec**
```
Write a technical specification for [FEATURE].

Stack: [STACK]
Dependencies: [EXISTING_SERVICES]

Sections: Problem, proposed solution, architecture diagram (describe), API contracts, data model changes, migration plan, testing strategy, deployment plan, monitoring, security considerations, estimated effort.
```

**50. Customer Interview Guide**
```
Create a customer interview guide for [RESEARCH_GOAL].

Participants: [PERSONA]
Duration: 30 minutes

Structure: Introduction (2 min), warm-up (5 min), core questions (18 min), wrap-up (5 min).

For each question: exact wording, what to listen for, when to probe deeper.

Rules: No leading questions. Behavior > opinions. Past > future.
```

---

## Bonus: Prompt Engineering Guide

### The 4 Elements

1. **Role** — Tell the AI who to be. "You are a senior Python developer at a fintech company" beats "Write Python code."
2. **Context** — Give background. Include the tech stack, audience, constraints.
3. **Constraints** — Set boundaries. "Use only stdlib. Must work on Windows/Linux. No external APIs."
4. **Output Format** — Specify exactly what you want back. "Output as JSON with these exact fields..."

### Pro Tips

- **Chain prompts**: Break complex tasks into a series of focused prompts. The output of prompt 1 becomes input to prompt 2.
- **Few-shot examples**: Show 2-3 examples of what "good" looks like. This is the single biggest lever for quality.
- **Iterate**: First draft → Ask for critique → Revise. Better than one "perfect" prompt.
- **Temperature matters**: 0 for facts, 0.3 for balanced, 0.7 for creative.
- **Model selection**: Claude Opus for complex reasoning. Haiku for speed. GPT-4 for breadth.

---

## Why $5?

- 1 prompt that catches a security vulnerability saves you thousands
- 1 prompt that generates your CI/CD pipeline saves you 4 hours
- 1 prompt that writes your PRD saves you a full afternoon
- Prompt #14 (Bug Root Cause) alone has saved me 20+ hours

**You'll make back the $5 on your first use.**

---

**[Buy Now — $5](https://www.buymeacoffee.com/aibusinesscorps)**

*AI Business Corps · Instant digital delivery · Free lifetime updates*
