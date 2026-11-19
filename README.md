# token-radar-01 — peer-calibrated launch board

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/ketip1/token-radar/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard)
[![reward](https://make.fun/badge/token-radar-01/ketip1/token-radar/reward.svg)](https://make.fun/bounty/token-radar-01)

A token launch radar: it reads the sealed DefiLlama snapshot and ranks every pre-token protocol by an
implied value. The valuation is peer-calibrated: each category's market-cap/TVL multiple is the log-median
of the 128 live protocols that already launched a token, so the board separates tokens that already trade
from those still to come. Every row carries a category-specific farm plan with cost and time.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input /input/snapshot.json
```

Requires Node.js 22+.
