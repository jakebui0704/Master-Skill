# Jake's skill catalog

Taken from Jake's "Yours" page: ~96 skills, 1 disabled. If Jake has added or removed skills
and this file wasn't updated, **ask, don't guess**.

## Overlapping skills (pick ONE)

- **Website review:** needs an audit AND fixes to the code → `enhance-ux-ax`. Needs detailed
  measurements, report only → `ux-ui-audit`. Wants to pin notes or draw on the live page, then
  hand a brief to a coder → `critic-layer`. (`ux-ui-website-review` is OFF, so never suggest it.)
- **Research synthesis:** deep customer interviews with every quote traceable →
  `interview-synthesis`. UX angle, themes + user segments → `research-synthesis`. PM angle,
  roadmap recommendations → `synthesize-research`. Merging ALL discovery outputs into one final
  doc → `insight-synthesizer`.
- **User profiles:** behavioral/UX → `persona-builder`. Account-level/B2B (ICP) →
  `icp-profile`. "Expert role-play" for Claude → `persona` (a different kind of thing).
- **Product brainstorm:** `product-brainstorming` (deeper, PM) over `brainstorm`.
- **Building a prototype:** static screens or a design system → Claude Design. Interactive
  page/tool with state, viewed inside Claude → `web-artifacts-builder`. A public page strangers
  visit (ads, social, waitlist) → Jake builds it with Claude Code and deploys it. Thanh only
  joins for logins, databases or payments.

## 0. Orchestration & meta

- `skill-creator`: create, edit and test skills (including this master-skill).
- `persona` (/persona): spin up an "expert role" (e.g. senior UX designer) as a sub-agent.
- `coach` (Prompt Coach): give it a rough request, get back a better prompt.
- `learn`: when Jake wants to LEARN or UNDERSTAND a concept, not produce a deliverable.
- `terse`: force very short replies (+ a context meter in Claude Code).

## A. User research & insight synthesis

- **ux-superpowers** (the UX backbone): `ux-discover` (THE STARTING POINT for any real
  project: builds a UX Discovery doc), `research-intake` (bring in raw research data),
  `persona-builder`, `jobs-to-be-done` (what job users "hire" the product to do),
  `user-journey` (the before/during/after journey), `telemetry-designer` (define success
  metrics), `ux-validate` (check the product hasn't drifted from the research before
  shipping), `insight-synthesizer` (merge everything into one doc).
- **Customer Research Kit:** `interview-guide` (draft or review interview questions),
  `interview-synthesis` (synthesize transcripts, every quote traceable), `feedback-analysis`
  (sort and tag 20+ reviews or tickets), `churn-analysis` (why customers leave),
  `icp-profile` (ideal B2B customer profile).
- `user-research` (Design): plan and run interviews and usability tests.
- `ycofficehour`: YC-style thinking. "Is this worth building?", research first.

## B. Product shaping & strategy (PM)

- **Product Management:** `write-spec` (PRD/spec), `roadmap-update` (Now/Next/Later),
  `sprint-planning` (scope a sprint against the team's capacity), `product-brainstorming` /
  `brainstorm`, `competitive-brief`, `metrics-review`, `synthesize-research`,
  `stakeholder-update`.
- **perception-first-design** (a cognitive-psychology lens for design, copy and marketing):
  `analyze` ("what happens if…"), `solve` (produce a solution that meets constraints),
  `evaluate` (score an artifact, with citations), `pfd` / `all`. Strong for first impressions
  and conversion.

## C. Interface design & visual

- **Claude Design** (a separate product used inside Claude): build real UI and design systems.
- `frontend-design`: visual direction, typography, avoiding a "templated" look.
- **Design:** `design-critique`, `design-system`, `ux-copy` (microcopy, buttons, errors,
  empty states).
- `theme-factory`: apply a color/font theme (10 presets or custom).
- `brand-guidelines`: apply an Anthropic-style look & feel.
- **Image Deep Research:** `image-deep-research`, `find-reference-images` (moodboards from
  licensed images), `website-contact-sheet` (screenshot competitors and measure their
  colors and fonts).
- **Figma** (14 skills, the bridge between design and code): `figma-design-to-code`,
  `figma-generate-design`, `figma-generate-library` / `figma-use`, `figma-generate-diagram`,
  `figma-implement-motion`, `figma-swiftui`, `figma-code-connect`, etc. Mostly Thanh, or Jake
  when he works deep in Figma.

## D. Review & quality checks (JAKE'S STRENGTH)

- ⭐ `enhance-ux-ax` (Jake's own skill, ENABLED; behavior changed, see "Needs checking" below): audits and auto-FIXES a website for UX
  (humans) and AX (SEO, LLMs, AI crawlers): hero, CTA, mobile at 375/768/1440,
  WCAG, semantic HTML, meta/OG, JSON-LD, robots/sitemap/llms.txt. Gives a MoSCoW report
  (Must/Should/Could/Won't). Fix mode edits the files on a git branch. PREFER it for any
  "audit + fix" job.
- `ux-ui-audit`: every finding comes with a MEASUREMENT. Report only.
- **Critic Layer:** `critic-layer` (notes and drawings right on the live page, turned into a
  brief), `brief`, `verify` (check the fixes were done right).
- `accessibility-review` (Design): quick WCAG 2.1 AA check before handoff.
- `design-handoff` (Design): developer handoff spec for Thanh.
- (`ux-ui-website-review` is OFF.)

## E. Build / web / artifacts

- `web-artifacts-builder`: complex web artifacts (React/Tailwind/shadcn) with state and
  routing. Good for vibe-coding an interactive page or tool.
- `mcp-builder`: build MCP servers (dev work, so Thanh).
- `algorithmic-art`: generative art with p5.js. Little work relevance.

## F. Writing, communication & docs

- `docs`: shareable, commentable documents (the default for anything to keep, send or print).
- `google-workspace`: create and edit Google Docs, Sheets and Slides.
- `internal-comms`: status reports, leadership updates, FAQs, incident reports.
- **Slack:** `standup`, `summarize-channel`, `channel-digest`, `find-discussions`,
  `draft-announcement`, `slack-search`, `slack-messaging`.

## G. Productivity & utilities

- **Productivity:** `start`, `task-management`, `memory-management`, `update`.
- `import-memory`: bring in a memory export from another AI.
- **PDF Viewer:** `view-pdf` / `open` / `annotate` / `fill-form` / `sign`.
- **Desktop Commander** (local-machine tools, mostly Thanh): `terminal`,
  `computer-health-check`, `ai-tools-setup`, `knowledge-base`, `obsidian-vault`.

## H. Added Oct 2026 (Jake confirmed he uses these)

- `deep-research`: multi-source research reports (comparing options, markets, trends).
  Needs subagents. Jake, in claude.ai or Claude Code.
- `built-in-browser`, `chrome-browser`: let Claude drive a browser, for example to check a
  live page. `chrome-browser` uses Jake's real Chrome and sign-ins; `built-in-browser` is the
  in-app pane. Pick `chrome-browser` when a login is needed. Jake.
- `computer-use`: let Claude click and type in desktop apps. Only when no browser or
  connector route exists. Jake, on his own computer.
- `session-start-hook`: set up a repo so cloud Claude Code sessions can run tests and
  linters. Thanh's area.

## Needs checking: `enhance-ux-ax`

The live description changed: it now says "audit a whole website for UX and AX at low cost,
turn findings into tickets with annotated screenshots, and QA the fixes." The older "fix mode
edits files on a git branch" wording is gone. Until Jake has checked it, don't promise
auto-fix; say it audits, writes tickets and QAs fixes, and ask what he wants it to do.
(Jake paused this check on 2026-10-08.)

## Connected tools (NOT skills, so confirm before relying on them)

Seen connected in Jake's workspace in Oct 2026: Lovable (app builder), Vercel (hosting/deploy),
Webflow (site builder), Figma, Canva, Notion, ClickUp, Slack, Gmail, Google Calendar/Drive,
Fathom & Fireflies (meeting notes), Atlassian (Jira/Confluence), Higgsfield (AI image/video).
Suggest one only when it clearly beats the skill route, and say why.

## Jake vs Thanh

- **Jake** (claude.ai, Claude Design, Cowork **and Claude Code**): research, UX, copy, design
  review, specs, prompts, comms, prototypes, simple landing pages, and running
  `enhance-ux-ax` in fix mode. Groups 0, A, B, C, D, E (web-artifacts), F, G.
- **Thanh** (Claude Code): logins, databases, payments, anything that must not break with
  real users' data, Figma design-to-code, `mcp-builder`, Desktop Commander.
- **The bridge:** `design-handoff` (and `write-spec`) is how work moves from Jake to Thanh.
- Rule of thumb: if a mistake would only make a page look wrong, Jake can do it. If a mistake
  could lose data, money or user accounts, bring in Thanh.
