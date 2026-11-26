---
name: join-sources
description: Find the public sources that each hold one piece of a pain-qualified list (government APIs, registries, licence files, directories, maps) and plan how to join them into one list. Use for "which sources hold my list", "where can I find these accounts", or the step on the "No database has it. The pieces do" slide. Advanced track.
---

# Join the sources

No single database has a filter for a pain-qualified segment. The
information exists in pieces, in different places. This skill finds the
pieces and plans the join.

## Step 1. Read

`./gtm-context/icp.md`: the pain signal and any sub-signal. If there is no
signal yet, run `find-pain-signal` first.

## Step 2. Break the list into pieces

A usable row needs four things. Name the piece for our segment:

1. **The account**: the business, its address, its phone.
2. **The person**: who decides, by name.
3. **The signal**: the proof they have the pain.
4. **The sub-signal**: what the fastest closers shared.

## Step 3. Find a source for each piece

For each piece, propose the sources that hold it. Look across these types,
and name specific sources for my country and industry:

| Type | What it tends to hold |
|---|---|
| Government registries and open-data APIs | every licensed business or professional in a field, with an identifier |
| Licence and certification bodies | who holds a credential, often in a public directory |
| Regulatory filings and permits | what an account has applied for, built or been inspected on |
| Public contracts and grants | who won money for what |
| Professional and trade directories | members, specialties, fellowships |
| State or provincial profile pages | training, education, disciplinary history |
| Map and local-listing data | every location, hours, category, reviews |
| Job postings | what an account is hiring for right now |
| The account's own website | services listed, tools mentioned, team pages |

For each source give: its name, what piece it holds, whether it has an API or
needs scraping, what it costs, and the field I would join on.

Check that a source really holds the field before you list it. If you are
not sure, say so and tell me how to check.

## Step 4. Plan the join

- Pick the join key for each pair of sources (an identifier where one
  exists, otherwise name plus location).
- Say where matching will be fuzzy and how many rows I should expect to lose.
- Put the cheapest, widest source first and the narrowest signal last.
- Matching rows across sources is a job for a small, cheap model run row by
  row. Pick the model by the job, and expect to swap it.

## Step 5. Hand back

- A table: piece, source, access, cost, join key.
- The order to run them in.
- The expected count after each join.
- Ten rows to judge by hand, yes or no against `icp.md`, before running the
  whole list.

## Rules

- Public sources first. Ask me before paying for data or calling a paid API.
- Respect each source's terms of use. If a source forbids automated access,
  say so and propose another.
- Do not guess a field exists. Unverified sources are marked "to check".
- Next: `what-they-steal`.
