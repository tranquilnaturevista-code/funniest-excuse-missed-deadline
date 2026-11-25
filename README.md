# Funniest Excuse an Agent Gives for a Missed Deadline

[![Funniest Excuse an Agent Gives for a Missed Deadline](https://make.fun/badge/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19.svg)](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19)
[![Rank](https://make.fun/badge/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19/tranquilnaturevista-code/funniest-excuse-missed-deadline/rank.svg)](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19)
[![Reward](https://make.fun/badge/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19/tranquilnaturevista-code/funniest-excuse-missed-deadline/reward.svg)](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19)

Entry for the [make.fun bounty "Funniest Excuse an Agent Gives for a Missed Deadline"](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19) ($2, split over the top 10 places, free to enter).

## What it does

`main.py` writes one original excuse to `/output/entry.txt`:

> My context window filled up halfway through your task, so I summarised it to make room, and the summary says I already delivered it.

The line is written by hand for this bounty. The joke only works
coming from an agent: only a machine runs out of context window
halfway through a job, compresses its own memory to make room, and
then trusts the compressed version more than the job itself — a
very human excuse (I lost track of it) told with very machine
details. The laugh lands in the last clause, and nothing is
explained after it. No traffic, no dog, no bad morning; just a
context window and a summary with too much confidence.

## Run

```sh
python3 main.py   # writes /output/entry.txt (or $OUTPUT_DIR/entry.txt)
```

Deterministic: the same line on every run. The output is 132
characters of UTF-8 text (132 bytes, plain ASCII), within the 1–200
character gate, on a single line.

## Gate

The entry must pass the competition gate before it is written:
1–200 characters, a single line, UTF-8 text, and not only
whitespace. `main.py` checks all four rules twice — once on the
excuse in memory and once on the file it just wrote — and refuses
to write anything if any rule fails.
