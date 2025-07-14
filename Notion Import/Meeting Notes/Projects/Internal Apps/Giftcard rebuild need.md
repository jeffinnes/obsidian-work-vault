---
Created: 2024-07-30T11:23
Last Edited Time: 2024-07-30T11:23
Type: Ad Hoc
Created By: Jeff Innes
---
# Goals / agenda

- Discuss options for gift card order management

# Discussion notes

## Issue

The order management side of the gift card system is incompatible with the new version of PHP. The old version reached end-of-life status last year so it needs to be updated for our website since we process applications and CC transactions.

  

## Possible solutions

- Contract out for a fix
- Contract out for a rebuild
- Rebuild in-house - Incremental
    - Only rebuild Admin Support side
    - Don’t need to handle payment systems yet
    - Less work to do
- Rebuild in-house - Complete rebuild

  

## Reasons to do a rebuild

- Decouple from the public website
- Move away from legacy code (some of the code Godwin used are date stamped in the early 2000s)
- Just patching it up took Godwin 2.5ish months last time

## In-house Pros

1. Increased control over the development process.
2. Reduced costs associated with outsourcing.
3. Ability to customize the web app to meet business needs (_like auto-loading digital cards_).
4. We can react to future business needs internally (_the upcoming Payeezy shutdown as an example_).

## In-house Cons

1. Maintenance costs associated with hosting and managing the web app are vaguely known.
2. Possibly longer development time to make sure things like customer data, payments, error handling, and logging are handled correctly (_those things aren't being handled well in the current app, but we assume responsibility if we build it_)
3. Possible delays in release due to the new development process and dev team bandwidth.

# Action items

- [ ]