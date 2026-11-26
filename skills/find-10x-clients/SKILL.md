---
name: find-10x-clients
description: From closed deals, find the 10X clients (closed fastest, pay most, refer others) and what they had in common before they bought. Also reads lost and churned deals for who to keep off the list. Use for "who are my 10X clients", "what did my wins have in common", or the step on the "The ICP comes from who closed" slide. Advanced track.
---

# Find the 10X clients

The goal is a short list of traits our best customers shared **before** they
bought, so the next list can look for accounts that have them today.

## Step 1. Get the deals

Read `./sources/deals.csv`. If it is missing, ask me for an export of closed
deals with, for each: account, date opened, date closed, won or lost, amount,
still paying or not, and where the deal came from.

Billing beats the CRM stage. If I can give you who is still paying, use that
to decide who counts as won.

## Step 2. Sort into three groups

- **Won**: closed and still paying.
- **Lost**: said no, or bought and left. A customer who churned looked like a
  fit and was not.
- **10X**: the top slice of Won. Closed fastest, pay most, or referred
  others. Name the rule you used and list the accounts.

If there are fewer than about ten won deals, say the sample is small and
treat what follows as hypotheses.

## Step 3. What the 10X had in common before they bought

For each 10X account, look at what was true before the first contact: who
they were, what they had, what they had just done. Use the deal notes, call
transcripts in `./sources/`, and what is public about the account.

List the traits that show up in most of the 10X group. For each trait give
the accounts that had it.

## Step 4. Cut

Remove a trait if:

- our competitors' customers have it too (it does not single out our buyer)
- it also shows up in the Lost group at the same rate
- it only became true after they bought

Keep a trait only if I could see it from outside, before contact: a
credential, a tool, a hire, a training, a filing, a location.

## Step 5. Read the losses

From Lost and churned deals, list what they had in common. That is who to
keep off the list.

## Step 6. Write it down

Show me the two or three traits that hold, each tied to named deals. After I
agree, write them into `./gtm-context/icp.md` under "Before they bought",
and the exclusion traits under "Who we keep off the list". Add the date and
"source: closed deals".

## Rules

- Numbers first, interviews second. Count before you interpret.
- When reading call transcripts, count only what the customer raised
  unprompted. Tag each line as seller or customer.
- Do not write a trait into `icp.md` that rests on one deal.
- Next: `find-pain-signal`.
