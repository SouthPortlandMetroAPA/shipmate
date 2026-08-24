# CrewCall

South Portland Metro APA — public **player ↔ team matching** intake. Successor to CrewFinder.

Two guided paths (one question per screen):
- **I'm looking for a team** (free agent): nights, formats, willing-to-play areas (+ optional favorite), and a short "about me".
- **I need a player** (captain): which of your current teams, 8- & 9-ball skill range, and what you're looking for — **one player per request**.

Magic-link login by email or APA #. Requests are stored in Supabase `crewcall.requests` via the shared GAS apa-mailer (`crew_*` actions) and reviewed in **Slate → CrewCall**.

- **Live:** https://southportlandmetroapa.github.io/crewcall/
- **Deploy:** push to `master` (GitHub Pages serves the repo root).
- **Brief / validator:** `tools/claude/briefs/2026-08-24-player-team-requests.md` · `tools/claude/validate-crewcall.mjs`
