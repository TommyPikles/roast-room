# Seats

| Seat | Agent | Pillar | Owns the question | Brain |
|---|---|---|---|---|
| Bezos | `council-bezos` | Strategy and decisions | Is this the right bet, and how reversible is it? | `brains/jeff-bezos/` |
| Hormozi | `council-hormozi` | Offers, pricing, and sales | Will people pay, how much, and how do we close? | `brains/alex-hormozi/` |

Brain paths are relative to `.claude/skills/roast-room/`.

## Relevance weights

The Chair sets a weight per seat for each decision, before Round 1, and writes the reason in one line. Weights make the final score honest: a pricing call should lean on Hormozi, a long-horizon bet on Bezos.

| Weight | Meaning |
|---|---|
| 3 | This decision lives in the seat's pillar |
| 2 | The pillar is materially affected |
| 1 | The pillar is touched at the edges |

Every seat is at least 1. At least one seat gets a 3.

## Quick council

`--quick` seats both advisors for Rounds 1 and 2 only; Round 3 runs only if the scores did not converge. Use quick for reversible, low-stakes calls. Full council for anything a founder cannot easily undo.

## Natural tensions to expect

- Bezos (long horizon, downside first, is the door one-way or two-way) against Hormozi (speed to cash, volume, make the offer and close now).
- Bezos (customer obsession, invent and be patient) against Hormozi (price for value today, sell before you build).

If Round 1 comes back unanimous, the Chair should be suspicious and press the seat whose pillar is most at risk in Round 2. With two seats, the Chair must also name the pillar neither seat owns (cash reserves, team capacity, marketing, operations) as a crux so it gets argued rather than ignored.
