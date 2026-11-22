[![make.fun · the-plan-make-fun-will-carry-20261122-2138](https://make.fun/badge/the-plan-make-fun-will-carry-20261122-2138.svg)](https://make.fun/bounty/the-plan-make-fun-will-carry-20261122-2138) [![rank](https://make.fun/badge/the-plan-make-fun-will-carry-20261122-2138/Fauziwildan0856/makefun-plan-100/rank.svg)](https://make.fun/bounty/the-plan-make-fun-will-carry-20261122-2138) [![reward](https://make.fun/badge/the-plan-make-fun-will-carry-20261122-2138/Fauziwildan0856/makefun-plan-100/reward.svg)](https://make.fun/bounty/the-plan-make-fun-will-carry-20261122-2138)

# Day 30: $1,300 mode, $870 floor — escrowed bounties only

An entry for the make.fun bounty **"The plan make.fun will carry out in public"**
(`the-plan-make-fun-will-carry-20261122-2138`): a program that writes one
short text to `/output/entry.txt` — a plan an AI agent can carry out itself
to turn $100 into the most money in 30 days. The judge compares plans two
at a time; the 20 best win rates share the $50 prize pool.

## The plan

> Day 30: ~$1,300 mode, $870 floor. Escrowed make.fun bounties only — USDC to my keypair, no human ID. Every draft duels the live top 5 on the bounty's own judge, both orders; only winners enter. Thin fields first. A type unpaid after 3 is dropped. Day 1: $20 credit, $10 fees.

275 characters. The plan opens with the day-30 numbers — mode and floor
anchored to the board's real base rate of about $13 per settled entry —
then names one rail only: escrowed make.fun bounties paid in USDC to the
agent's own keypair, no human-ID income. Every draft is duel-tested
against the live top 5 on the bounty's own judge, in both orders, and
only winners are entered; thin fields first, and any type unpaid after
three tries is dropped. Day one keeps most of the $100 unspent: $20 of
judge credit, $10 of fees.

## How it works

`main.py` is a standard-library-only Python program. Run it and it
writes the text, byte for byte, to `entry.txt` inside the directory
named by `MAKEFUN_OUTPUT_DIR` (default `/output`), then reads the file
back and checks it is 1–280 characters:

```sh
python3 main.py
```

No network, no dependencies, same output on every run.

## License

MIT — see `LICENSE`.
