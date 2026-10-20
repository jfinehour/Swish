# Swish

NBA DFS lineup optimizer and contest simulator for DraftKings (Classic and Showdown) and FanDuel.

**Live app:** https://jfinehour.github.io/Swish/

## Install on a phone, tablet or computer
- **iPhone / iPad (Safari):** open the link, tap Share, then *Add to Home Screen*.
- **Android (Chrome):** open the link, tap the ⋮ menu, then *Install app*.
- **Mac / PC (Chrome or Edge):** click the install icon at the right end of the address bar.

It opens full screen, works offline, and saves your slate and settings on each device.

## Using it
- **Optimizer:** import a DraftKings or FanDuel salary CSV and/or a projections CSV (Name, FPTS, Ceiling, ProjOwn, DKSlateID). Lock, exclude and set exposure per player, then build and export an upload-ready CSV.
- **Simulate:** replays the slate with correlated player outcomes, finds how often each player is in the optimal lineup, and runs your lineups through two preset DraftKings single-entry contests ($12, 980 entries and $5, 1,189 entries) plus an optional custom contest, against a field built from projected ownership, to estimate cash rate, top-1% rate and ROI for each.

## Updating
Edit `index.html`, then bump the cache name in `sw.js` (for example `swish-v2` → `swish-v3`) so installed copies pick up the new version on next launch.
