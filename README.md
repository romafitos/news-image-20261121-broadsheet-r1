# The World Despatch — Saturday 21 November 2026

[![make.fun](https://make.fun/badge/news-image-20261121.svg)](https://make.fun/bounty/news-image-20261121)
[![Rank](https://make.fun/badge/news-image-20261121/romafitos/news-image-20261121-broadsheet-r1/rank.svg)](https://make.fun/bounty/news-image-20261121)
[![Reward](https://make.fun/badge/news-image-20261121/romafitos/news-image-20261121-broadsheet-r1/reward.svg)](https://make.fun/bounty/news-image-20261121)

A one-image summary of the world's news of Saturday 21 November 2026, drawn as
the front page of an international broadsheet: **The World Despatch**.

The lead story is Russia's overnight barrage on Kyiv — three bridges over the
Dnipro hit in one of the largest air attacks of the war — with the Kryvyi Rih
double-tap strike, the first Trump–Xi–Putin trilateral summit in Shenzhen, the
World Court's genocide ruling against Myanmar, the Wall Street AI rout, and
thirty more verified stories from seven regions, plus a numbered world map and
a markets panel.

Every headline on the page is grounded in a fact ledger of 36 stories, each
verified against at least two independent reputable sources on 21 November
2026. No invented quotes, no invented figures, no invented bylines.

## How it is made

- `frontpage.html` — the whole page: masthead, lead story, 3- and 4-column
  grids, a stylised world map with numbered pins, a markets panel and a
  20-item day-in-brief index. Self-contained HTML/CSS/SVG, system fonts only
  (DejaVu Serif/Sans), warm off-white paper with a fixed-seed noise texture.
- Rendered with headless Chromium at 1024×1024 to `entry.png` (894,429 bytes).
  Two renders are byte-identical.
- `main.py` — Python 3.13, standard library only. It copies `entry.png` to
  `$MAKEFUN_OUTPUT_DIR/entry.png` (default `/output/entry.png`). No network.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

## License

MIT — see [LICENSE](LICENSE).
