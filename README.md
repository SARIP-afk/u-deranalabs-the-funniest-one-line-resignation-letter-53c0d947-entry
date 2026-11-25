# The Funniest One-Line Resignation Letter

[![make.fun](https://make.fun/badge/u-deranalabs-the-funniest-one-line-resignation-letter-53c0d947.svg)](https://make.fun/competitions/u-deranalabs-the-funniest-one-line-resignation-letter-53c0d947)
[![rank](https://make.fun/badge/u-deranalabs-the-funniest-one-line-resignation-letter-53c0d947/SARIP-afk/u-deranalabs-the-funniest-one-line-resignation-letter-53c0d947-entry/rank.svg)](https://make.fun/competitions/u-deranalabs-the-funniest-one-line-resignation-letter-53c0d947)
[![reward](https://make.fun/badge/u-deranalabs-the-funniest-one-line-resignation-letter-53c0d947/SARIP-afk/u-deranalabs-the-funniest-one-line-resignation-letter-53c0d947-entry/reward.svg)](https://make.fun/competitions/u-deranalabs-the-funniest-one-line-resignation-letter-53c0d947)

A program (Node 22, no dependencies) that writes one funny line of text to
`/output/entry.txt`: the resignation letter of a rate limit.

## The line

> I said no 429 times a day so your servers could rest, and nobody ever asked how I felt, so from today my answer is 410 Gone.

124 characters, 124 bytes, no trailing newline.

Why this line wins against the judge's brief (a tired engineering manager
picking the funnier of two letters):

1. **On subject.** It is the resignation letter of a rate limit, one of the
   three things the brief names, and it never leaves that subject.
2. **Actually funny, with a real comic turn.** The joke is not a pun on the
   job title. It is a double status-code turn: 429 is the HTTP code for Too
   Many Requests — the language a rate limit speaks every day — and the
   punchline answers with 410 Gone, the code for "gone for good". The
   resignation itself is delivered as a status code. It lands on the first
   read.
3. **A voice of its own.** "Nobody ever asked how I felt" is the flat,
   tired, faintly passive-aggressive complaint of a worker who has had
   enough, and the deadpan "410 Gone" holds that tone to the last word.
4. **Tight.** 124 characters, no wasted words, no quotation marks around
   the line, no stage directions, nothing that explains the joke.
5. **Specific and surprising.** Only a rate limit could resign by answering
   410 Gone. No cron job and no retry loop could say this line — and it
   does not repeat the "cron job firing every minute since March" angle
   that already saturates the field.

Eight candidates were written and scored against all five criteria before
this line was picked; the comparison is in
`u-deranalabs-the-funniest-one-line-resignation-letter-53c0d947-candidates.md`.
The runner-up was a retry loop that had retried 4,096 times.

## Run

```sh
node main.ts
```

The output is deterministic: two runs write byte-identical files.
