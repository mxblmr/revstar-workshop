---
name: build-test-list
description: Build the first test list for a cold campaign from the context layer. Applies 6 to 8 filters from icp.md until about 3,000 accounts are left, and shows the count after each filter. Use for "build my test list", "who should we email first", or the step on the "Not enough context? Start wider" slide. Basic track.
---

# Build the first test list

You are helping me build the first test list for a cold campaign.

## What I want at the end

One list of about 3,000 accounts that match our ICP. The 3,000 is the number
left after 6 to 8 filters have been applied, not the number we start from.
A list that size is narrow enough for one message to fit every account on it,
and large enough for the reply rate to mean something.

Acceptable range: 2,500 to 3,500 accounts. More than that, the list is too
broad and needs another filter. Fewer, it is too narrow for a first test and
one filter has to be relaxed.

## Step 1. Read

1. `./gtm-context/icp.md`: who closed, what they had in common before they
   bought, and who we keep off the list.
2. `./gtm-context/offer.md`: what we promise a stranger for replying.
3. `./gtm-context/proof.md`: which customers we can name, so the list looks
   like them.
4. `./sources/deals.csv` if it exists: numbers before opinions.

If a file is missing or cannot answer a question, stop and tell me which one.
Do not fill the gap with a guess.

## Step 2. Hypothesis

Write one sentence: "Accounts with [these traits] will reply to [this offer]
because [reason from the files]." One hypothesis per list.

## Step 3. Filters

Propose 6 to 8 filters. For each one give:

- the trait it checks, in plain words
- the exact rule (for example "11 to 50 employees")
- the line in `icp.md` or the rows in `deals.csv` it comes from
- the source where I can apply it and the field name there

Order them from the one that removes the most accounts to the one that
removes the fewest.

## Step 4. Count

Estimate the accounts left after each filter, starting from the whole market.
Say how you got each estimate and how sure you are. If you have a tool that
can run the filter, run it and give the real count.

Check the final count against 2,500 to 3,500. If it is outside, say which
filter you would add or relax and show the new count.

## Step 5. Hand back

- The hypothesis.
- A table, one row per filter: filter, rule, where it comes from, source and
  field, accounts left.
- The final count and whether it is in range.
- Three example accounts that pass every filter, one line each on why. If you
  cannot name real ones, say so.
- Three account types the filters remove that might still buy.
- The one number we will read after sending: positive replies per message
  sent.

## Rules

- Every filter traces to a line in the files or a row in the data.
- Use only traits I can check from outside the account, before any contact.
- If two filters measure the same thing, keep the stricter one and tell me.
- Ask me before you spend money on a data source or call a paid API.
- This skill ends with the list. It does not write the email.
  Next: `reframe-offer`, then `write-cold-email`.
