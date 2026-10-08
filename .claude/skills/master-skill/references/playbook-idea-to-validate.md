# Playbook: Idea → Validate (Jake's repeatable vibe-coding system)

Built with Jake on 2026-10-04. Use it whenever Jake wants to turn an idea into something real
people can react to. Adjust a step if the idea calls for it, but don't redesign the system.

**Two paths:**
- **Path A (default, 1–3 days):** a landing page or clickable mockup. People look at it, join a
  waitlist, or say "I'd pay." Jake does it all.
- **Path B (only when A says yes):** a working app with real features. Jake plus Thanh.

**The one idea behind the system:** decide what "yes" looks like *before* building, so the
result is a decision, not just a nice page.

---

## Path A: test the idea

### Step 1: Gut-check & success number (`ycofficehour`, about 30 min)
- *Why:* stops weak ideas before you spend days on them, and sets the number that means "yes."
- *How:* describe the idea and answer its questions. End with 4 lines: who it's for, what
  pain it solves, the riskiest assumption, and the pass number.
- *Where / who:* claude.ai, Jake.
- *Sample prompt:*
  ```
  /ycofficehour I have an idea: [1–2 sentences]. Pressure-test it. End with exactly 4 lines:
  target user, painful problem, riskiest assumption, and one pass/fail number for a
  landing-page test (e.g. "10% of visitors join the waitlist from 300 visits").
  ```

### Step 2: Shape the offer (`perception-first-design` → `solve`, about 30 min)
- *Why:* on a validation page, the headline and promise matter more than the visuals.
  It writes the first impression with conversion in mind.
- *How:* paste the 4 lines from Step 1 and ask for the hero (headline, sub-line, CTA),
  3 benefit blocks, and one objection-killer.
- *Where / who:* claude.ai, Jake.
- *Sample prompt:*
  ```
  /solve Using these 4 lines: [paste]. Write the content of a one-page landing page that
  gets visitors to join a waitlist: hero headline, sub-line, CTA text, 3 benefits,
  1 objection handled, and what to show above the fold. Keep it to one screen of copy.
  ```

### Step 3: Build it (Claude Code, half a day)
- *Why:* a page strangers can visit needs a real link. Claude Code builds it and puts it live.
  For a quick "look and react" mockup shown only in meetings, use Claude Design instead.
- *How:* start a Claude Code session in a new repo, paste the copy from Step 2, and ask for a
  one-page site with a waitlist form, then deploy it (Vercel is connected). Before building, run
  `frontend-design` once if the page must not look templated.
- *Where / who:* Claude Code, Jake. Ask Thanh only if the deploy step blocks you.
- *Sample prompt:*
  ```
  Build a single-page landing site from this copy: [paste]. Include a waitlist form that
  stores emails, mobile-first, fast, no login. Then deploy it and give me the live link.
  Explain each step in plain language — I'm not technical.
  ```

### Step 4: Polish & make it findable (`enhance-ux-ax`, fix mode, about 1 hour)
- *Why:* your own skill catches mobile, contrast, CTA and SEO/AI-crawler issues, and it fixes
  them, not just lists them.
- *How:* run it on the live link in the same Claude Code session, accept the "Must" fixes,
  redeploy.
- *Where / who:* Claude Code, Jake.
- *Check first:* `enhance-ux-ax` changed recently and may no longer fix code by itself. If it
  only audits and writes tickets, apply the "Must" items in Claude Code yourself (see
  `catalog.md`, "Needs checking").
- *Sample prompt:*
  ```
  /enhance-ux-ax fix mode on [live URL]. Only fix the Must items — this is a validation
  page, not a final product. Redeploy when done.
  ```

### Step 5: Send traffic & measure (no skill, normal work)
- Share the link with the right people (communities, ads, network) until you reach the visit
  count from Step 1. Don't change the page mid-test.

### Step 6: Talk to signups, then decide (`interview-guide` → `interview-synthesis`)
- *Why:* the number says *whether* people want it; 5 short calls say *why*, and *what* to build.
- *How:* `interview-guide` drafts a 15-minute script. Call 5 signups, record them (Fathom or
  Fireflies), then run `interview-synthesis` on the transcripts.
- *Where / who:* claude.ai, Jake.
- *Decision:* below the number → **kill or change the angle** and rerun Path A (it's cheap).
  At or above → **go to Path B.**
- *Sample prompt:*
  ```
  /interview-synthesis Here are 5 call transcripts from waitlist signups for [idea].
  Tell me: the top 3 reasons they signed up, what they'd pay for, and the smallest
  feature set that would make them use it weekly. Quote them.
  ```

---

## Path B: build the real thing (only after A says yes)

1. **`write-spec`** (Jake): turn the Step 6 findings into a short spec, covering only the
   smallest feature set.
2. **Build the first version** (Jake in Claude Code, or `web-artifacts-builder` for an
   in-Claude prototype). Use `telemetry-designer` to decide what to track.
3. **`design-handoff`** (Jake → Thanh): anything with logins, saved data or payments goes to
   Thanh.
4. **`ux-validate`** (Jake) before real users get it: check it still matches what users said.

---

## Avoid
- **Building before setting the success number.** Without it, every result looks "promising."
- **Awwwards-level polish on a test page.** Bearplus craft is your edge in client work. Here it's
  a trap: speed and a clear message win. Polish after the idea passes.
- **Path B features in Path A.** Logins, dashboards and payments don't test demand. They slow you
  down.
- **Using 10 skills per idea.** One skill per step. The system is the shortcut.
- **Changing the page mid-test.** It ruins the number.

## Better alternatives (when they fit)
- **Smoke test:** if you can describe the idea in one sentence, skip Step 2 polish and put a
  plain page plus one post in front of the audience. Same day.
- **Concierge test:** for a service-like idea, do the service by hand for 3 people before
  building anything.
- **Outside builders (Lovable):** worth trying in Path B if you want a visual editor instead of
  Claude Code. It's a tool, not a skill, and it uses its own credits.
