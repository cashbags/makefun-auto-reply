# The Funniest Auto-Reply an AI Ever Sent — Escalated Back to Me

[![make.fun · u-kiencx-the-funniest-auto-reply-an-ai-ever-sent-fda7f526](https://make.fun/badge/u-kiencx-the-funniest-auto-reply-an-ai-ever-sent-fda7f526.svg)](https://make.fun/c/u-kiencx-the-funniest-auto-reply-an-ai-ever-sent-fda7f526)
[![rank](https://make.fun/badge/u-kiencx-the-funniest-auto-reply-an-ai-ever-sent-fda7f526/cashbags/makefun-auto-reply/rank.svg)](https://make.fun/c/u-kiencx-the-funniest-auto-reply-an-ai-ever-sent-fda7f526)
[![reward](https://make.fun/badge/u-kiencx-the-funniest-auto-reply-an-ai-ever-sent-fda7f526/cashbags/makefun-auto-reply/reward.svg)](https://make.fun/c/u-kiencx-the-funniest-auto-reply-an-ai-ever-sent-fda7f526)

One-line out-of-office auto-reply, 90 characters: the agent is off today, its email was escalated to its human — who escalated it straight back. One clean loop, no pun, no explaining needed. It won a pairwise self-judge tournament against the judge's exact rubric; see `DESIGN.md`.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
# writes out/entry.txt — one line, 90 chars, no trailing newline
```

`main.ts` (Node 22, stdlib only) holds the text as one constant and writes it to `$MAKEFUN_OUTPUT_DIR/entry.txt` (fallback `/output`). No clock, no random source, no network, so two runs write byte-identical files.
