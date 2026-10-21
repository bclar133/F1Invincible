# F1 Invincible — Development Preview

This repository is **for testing and development**. It is separate from `www.brent-clark.com`, and changes here do **not** publish to the Brent Clark Games homepage.

## Open the game on a phone or desktop

To enable the dedicated preview site (one-time setup):

1. In this GitHub repository, open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch `main`, folder **/(root)**, then click **Save**.
4. After GitHub finishes deploying, open **https://bclar133.github.io/F1Invincible/** on mobile or desktop.

The preview link will update when new commits are pushed to `main` (deployment may take a minute). The repo and preview are publicly accessible to people who know the link; they are not private or password-protected.

## Auto setup (editable recommendations)

- **Auto Budget** suggests engineering spending in $0.5 million steps based on the historical car, drivers and season circuit mix. Before the season it replaces the current budget split; at halfway it only allocates remaining upgrade funds.
- **Auto Strategies** configures each driver's racing style, pit approach, qualifying and overtake mode independently.
- **Auto Tyres** is available after qualifying in Full Race and Highlights. It suggests compounds, pit laps and stop count based on conditions and stint life and avoids double-stacking when possible.

All suggestions can be manually changed before starting the race. They are gameplay recommendations, not guaranteed best outcomes.

## Mobile design

The single-page game includes responsive cards, two-row touch-friendly engineering allocation controls, stacked racing and qualifying views, and mobile tyre-planning controls. Test at common phone widths and report any clipping/overflow you see. Browser progress uses `localStorage` per device, so a phone and computer do **not** share the same championship save.

## Notes

- The 2026 and historic standings load from Jolpica where available, with offline demonstration data where supported.
- Images and circuit outlines are served by third-party services; some may fail without internet access.
- This is an unofficial fan-made project, not affiliated with Formula 1.
- Do not add a link to the public Brent Clark Games website until publication is specifically approved.

### Circuit asset credit

Monaco circuit SVG adapted from [F1DB](https://github.com/f1db/f1db/blob/main/src/assets/circuits/white/monaco-1.svg), licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). The source SVG is bundled as `assets/tracks/monaco.svg`. No track geometry modifications were made.
