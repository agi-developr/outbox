# Outbox / Loop — handoff

Written for an AI agent picking this up cold. Read this file first, then `BUILD-THIS.md`.

## What this repo is

A demo built live at the IxDF San Francisco "Design Hackathon: Vibe Coding Night", 2026-08-28,
530 Howard St. Sixty-minute build, designer-heavy judging panel, demo link required. Ilia
presented it. The submitted link was `https://agi-developr.github.io/outbox/`.

Stack is deliberately trivial: one self-contained `index.html` per version, React 18 and Babel
standalone from unpkg CDN, no build step, no dependencies, no backend. Deploys by pushing to
`main`; GitHub Pages serves from the repo root. This was chosen so a venue wifi failure or an
npm install could not kill the demo.

## The four versions, and which one is canonical

Ilia's verdict after presenting: **version 1 was the best one.** It is restored at the root.

| Path | Commit of origin | What it is |
|---|---|---|
| `/` (root `index.html`) | `c8c3fb9` | **Canonical.** Four-lane board over email: Needs you, Reply ready, Chasing for you, Handled. Cards carry a drafted reply, a one-line reason, event invites with gain-versus-cost, and agent-owned CEO follow-ups with attempt counters. Header has "Call me and ask" (an interview modal that asks the three questions it cannot decide and clears cards as you answer) and "Deliver a new email" (a live triage animation). Cloudy light skin. |
| `/v2/` | `d308a4a` | Three-column commitment board: Waiting on them, Waiting on you, Closed today. Voice capture. Teach-once rules. |
| `/v3/` | `1a0cfaa` | Voice-first single screen. One mic, a short list of native actions, "Text him too?", "Always do that?". |
| `/v4/` | `6b4afa3` | The fused four-column dashboard: adds a "Doing now" column, an inline interview strip, gain-versus-cost event cards, native Maps action, spam blocking, and the learn layer, all on one page. |

Every version is also recoverable from git history at the commits above.

## The mistake to not repeat

Across the session Ilia gave roughly twelve product ideas. Each time, I replaced the previous
surface instead of adding a layer to it, so he watched ideas get traded against each other and
ended up with three demos instead of one product. His words: *"every time i feel like you listen
to my 10 ideas and not fusing into mega multilayer dashboard you build 1.5 of them and said im
done."* If you continue this project, **layer onto the existing page. Do not start a fifth
version.**

## The product thesis, if this is continued

The unit is not the message, it is the **open loop** — something you owe a person, or a person
owes you. Email is where most loops arrive, not what the product is about. The board holds loops,
the agent chases the ones that need chasing, and it asks you only what it genuinely cannot decide.
It learns rules by example ("Always do that?") instead of having a settings screen, which is how
it avoids becoming a bulky CRM. Full reasoning and the assumption tests are in `BUILD-THIS.md`.

Design language: cloudy light gradients on `#F7F6FB`, Instrument Serif for display, Inter for
body, white cards with soft violet shadows, accent `#6D5CE7` to `#C86DD7`. Ilia approved this
part; do not change it.

## What was never built

No real mail. `AGENTMAIL_API_KEY` is already in `~/.claude/.env` and AgentMail gives instant
API-key inboxes with no Gmail OAuth review, which is the shortest path to making this real. The
follow-up quality is the thing to prove first — if attempt two of a chase does not beat attempt
one on a real human, none of the UI matters.

## Files

- `index.html` — canonical demo (v1)
- `v2/`, `v3/`, `v4/` — the other three versions
- `BUILD-THIS.md` — market analysis, Ilia's assumptions tested one by one, the fused product spec
- `PLAN.md` — earlier plan plus ten open questions for Ilia
- `DEMO.md` — the sixty-second stage script for v1
- `HANDOFF.md` — this file

## Related knowledge notes

- `LIFEOS/MEMORY/KNOWLEDGE/Ideas/voice-context-extraction-mcp-interview-before-you-build.md`
- `LIFEOS/MEMORY/KNOWLEDGE/Ideas/open-loop-agent-the-crm-that-fills-itself.md`
- `LIFEOS/MEMORY/KNOWLEDGE/Ideas/in-music-embedded-advertising-context-matched.md`
