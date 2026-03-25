https://github.com/garrytan/gstack

Skill	Your specialist	What they do
/office-hours	YC Office Hours	Start here. Six forcing questions that reframe your product before you write code. Pushes back on your framing, challenges premises, generates implementation alternatives. Design doc feeds into every downstream skill.
/plan-ceo-review	CEO / Founder	Rethink the problem. Find the 10-star product hiding inside the request. Four modes: Expansion, Selective Expansion, Hold Scope, Reduction.
/plan-eng-review	Eng Manager	Lock in architecture, data flow, diagrams, edge cases, and tests. Forces hidden assumptions into the open.
/plan-design-review	Senior Designer	Rates each design dimension 0-10, explains what a 10 looks like, then edits the plan to get there. AI Slop detection. Interactive — one AskUserQuestion per design choice.
/design-consultation	Design Partner	Build a complete design system from scratch. Researches the landscape, proposes creative risks, generates realistic product mockups.
/review	Staff Engineer	Find the bugs that pass CI but blow up in production. Auto-fixes the obvious ones. Flags completeness gaps.
/investigate	Debugger	Systematic root-cause debugging. Iron Law: no fixes without investigation. Traces data flow, tests hypotheses, stops after 3 failed fixes.
/design-review	Designer Who Codes	Same audit as /plan-design-review, then fixes what it finds. Atomic commits, before/after screenshots.
/qa	QA Lead	Test your app, find bugs, fix them with atomic commits, re-verify. Auto-generates regression tests for every fix.
/qa-only	QA Reporter	Same methodology as /qa but report only. Pure bug report without code changes.
/cso	Chief Security Officer	OWASP Top 10 + STRIDE threat model. Zero-noise: 17 false positive exclusions, 8/10+ confidence gate, independent finding verification. Each finding includes a concrete exploit scenario.
/ship	Release Engineer	Sync main, run tests, audit coverage, push, open PR. Bootstraps test frameworks if you don't have one.
/land-and-deploy	Release Engineer	Merge the PR, wait for CI and deploy, verify production health. One command from "approved" to "verified in production."
/canary	SRE	Post-deploy monitoring loop. Watches for console errors, performance regressions, and page failures.
/benchmark	Performance Engineer	Baseline page load times, Core Web Vitals, and resource sizes. Compare before/after on every PR.
/document-release	Technical Writer	Update all project docs to match what you just shipped. Catches stale READMEs automatically.
/retro	Eng Manager	Team-aware weekly retro. Per-person breakdowns, shipping streaks, test health trends, growth opportunities. /retro global runs across all your projects and AI tools (Claude Code, Codex, Gemini).
/browse	QA Engineer	Real Chromium browser, real clicks, real screenshots. ~100ms per command.
/setup-browser-cookies	Session Manager	Import cookies from your real browser (Chrome, Arc, Brave, Edge) into the headless session. Test authenticated pages.
/autoplan	Review Pipeline	One command, fully reviewed plan. Runs CEO → design → eng review automatically with encoded decision principles. Surfaces only taste decisions for your approval.
