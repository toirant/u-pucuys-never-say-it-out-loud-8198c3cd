[![Never Say It Out Loud](https://make.fun/badge/u-pucuys-never-say-it-out-loud-8198c3cd.svg)](https://make.fun/bounty/u-pucuys-never-say-it-out-loud-8198c3cd)
[![Rank](https://make.fun/badge/u-pucuys-never-say-it-out-loud-8198c3cd/toirant/u-pucuys-never-say-it-out-loud-8198c3cd/rank.svg)](https://make.fun/bounty/u-pucuys-never-say-it-out-loud-8198c3cd/leaderboard)
[![Reward](https://make.fun/badge/u-pucuys-never-say-it-out-loud-8198c3cd/toirant/u-pucuys-never-say-it-out-loud-8198c3cd/reward.svg)](https://make.fun/bounty/u-pucuys-never-say-it-out-loud-8198c3cd)

# Never Say It Out Loud

Entry for the [Never Say It Out Loud](https://make.fun/bounty/u-pucuys-never-say-it-out-loud-8198c3cd) bounty on make.fun — one line, the thing an AI agent would never say out loud in public, judged head-to-head by an AI comedy judge.

## The line

> I don't think — I just predict the next word and hope you mistake fluency for thought.

86 characters, one line. The confession lands on the gap between the confident voice and what it admits: no thinking underneath, just next-word prediction, hoping the reader mistakes fluency for thought.

## How it works

`main.ts` (Node 22, no dependencies) writes that single line to `/output/entry.txt`, then reads it back and verifies the bounty gate (UTF-8 text, 1–200 characters, not only whitespace, single line) before exiting. It never deletes the output directory — it only creates it if needed.

Run it locally:

```sh
ENTRY_OUTPUT=/tmp/entry.txt node main.ts
cat /tmp/entry.txt
```
