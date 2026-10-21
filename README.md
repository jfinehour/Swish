# Swish

NBA DFS lineup optimizer and contest simulator for DraftKings (Classic and Showdown) and FanDuel.

**Live app:** https://jfinehour.github.io/Swish/

## Install on a phone, tablet or computer
- **iPhone / iPad (Safari):** open the link, tap Share, then *Add to Home Screen*.
- **Android (Chrome):** open the link, tap the ⋮ menu, then *Install app*.
- **Mac / PC (Chrome or Edge):** click the install icon at the right end of the address bar.

It opens full screen, works offline, and saves your slate and settings on each device.

## Using it
- **Lineup types:** Projection (cash), Ceiling, Small Field GPP and Large Field GPP. GPP types rank players by a leverage score (ceiling blended with projection, discounted by ownership, with a heavier fade for large fields), cap exposure and require near-full salary by default.
- **Late swap:** with tip times (from a salary file, the Vegas line pull, or typed in), Classic lineups are slotted so the latest games sit in UTIL, later games in the other flex slots (G/F on DraftKings; G/F and F/C on FanDuel), and the earliest games in PG–C.
- **Optimizer:** import a DraftKings or FanDuel salary CSV and/or a projections CSV (Name, FPTS, Ceiling, ProjOwn, DKSlateID). Lock, exclude and set exposure per player, then build and export an upload-ready CSV.
- **Vegas lines:** pull consensus spreads and totals from The Odds API (your own key, stored only on your device) or type them in. Optionally adjust projections to implied team totals; sims use totals for game-level swing and spreads for blowout risk.
- **Sim-built lineups:** builds a pool of candidate lineups, runs them all through the selected contests, keeps the best by ROI, top-1% or cash rate (respecting your locks, exposure and min-unique settings), and re-scores the picks on fresh replays.
- **Simulate:** replays the slate with correlated player outcomes, finds how often each player is in the optimal lineup, and runs your lineups through four preset DraftKings single-entry contests ($12 with 980 entries, $5 with 1,189 entries, $12 Pick and Roll with 490 entries, and the $3 Sharpshooter with 15,854 entries) plus an optional custom contest, against a field built from projected ownership, to estimate cash rate, top-1% rate and ROI for each.

## Updating
Edit `index.html`, then bump the cache name in `sw.js` (for example `swish-v2` → `swish-v3`) so installed copies pick up the new version on next launch.
