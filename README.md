# Draft Room

A single-file draft companion for a live, in-person fantasy football draft.
One HTML file, no server, no build step, no network — open `draft-kit.html`
in a browser and it works offline.

## Using it

Open the file, then **Setup → Rankings** and load a CSV export of your
rankings (FantasyPros, RotoBaller, Sleeper, ESPN and Yahoo all work — column
mapping is detected and confirmable). Set your league size, draft slot and
scoring, and you're ready.

During the draft, tap a player to log the pick to whoever is on the clock.
Search and press Enter to draft the top match. Long-press to assign a pick out
of order, correct a mistake, or flag an injury.

## What it does

- **Board** — your rankings with survival odds, your rank against market ADP,
  value over replacement, tier breaks and positional runs
- **Cost of waiting** — for each position, the value on the board now against
  what you can expect to still be there at your next turn
- **My Team** — projected points against the rest of the league, strength by
  position, bye-week clashes, and what's still to fill
- **Ranking sets** — load several lists, switch between them mid-draft without
  losing picks, or average them as a consensus
- **Article picks** — paste any text and it finds which of your players it
  mentions, so a staff-picks piece or an injury report becomes flags on the board
- **Scoring** — rebuild projected points under your league's rules from the
  stat columns in your export
- **Rehearsal mode** — auto-drafts the other teams so you can practise

Picks, notes and flags attach to the player rather than to a file, so they
survive switching ranking sets. Everything saves to the browser after each
pick, and **Setup → Backup** writes a file you can carry to another device.

## Notes

This repository is private, because the saved backup checked in alongside the
app carries a full set of parsed rankings — third-party projections that should
not be redistributed. Raw CSV exports stay untracked.

The app itself ships with a small sample board, clearly labelled, so the
interface is explorable before importing anything.

To set up a new device, load `draft-kit.html`, then **Setup → Load a backup
file** and pick the `draft-kit-<date>.json` here. That restores the rankings,
league settings, scoring, notes and flags in one step.
