---
name: read-the-round
description: After a batch has been sent, read the results, decide which one line in the context layer should change, and pick the next test. Use for "read the round", "what did we learn", "what do we test next", or the step on the "Run experiments fast, learn faster" slide. Basic track.
---

# Read the round

One round is: pick one change, send to a batch, read the replies, fix one
line in the files. This skill does the last two.

## Step 1. Get the results

Ask me for, or read from `./record/`:

- how many messages were sent, per version (A and B)
- how many positive replies each version got
- the text of the replies, positive and negative
- what the round was testing (the list, the offer or the ask)

A positive reply is a yes to the ask. "Not interested" and "remove me" are
not positive. An out-of-office is not a reply.

## Step 2. Read the number

For each version, give positive replies per message sent. Say plainly when
the batch is too small to tell A from B. Under about 200 sends per version,
treat a difference as a hint, not a result.

## Step 3. Read the words

Read every reply. Report:

- what people said yes to, in their own words
- what they pushed back on
- anything that tells us the list was wrong (wrong role, wrong size, wrong
  kind of company)
- anything that repeats across three or more replies

Quote the replies. Do not summarise them into our vocabulary.

## Step 4. Fix one line

Propose one change to one file:

- `icp.md` if the replies say who should or should not be on the list
- `offer.md` if the replies say what they would say yes to
- `proof.md` if they asked for evidence we did not give
- `objections.md` if the same pushback came up three times

Show the line before and after. Wait for my yes before you edit.

## Step 5. Log it

Add one row to `./record/rounds.md`: date, what was tested, sends, positive
replies per version, what we learned, the line that changed.

## Step 6. Next test

Propose the next round: one thing to change, and why. Keep the rest the same.

## Rules

- One change per round. If two things change, we cannot tell which one
  mattered.
- A reply is worth more than an open or a click.
- If the round taught us nothing, say so and say why (batch too small, two
  things changed, list too mixed).
- When the same trait keeps showing up in the yes replies, tell me. That is
  the sign to move to the advanced track: `find-10x-clients`.
