---
name: Rollers withdrawal policy
description: Owner-confirmed deposit qualification and withdrawal-link rules for the Rollers bot.
---

Withdrawals require a qualifying crypto deposit in the rolling previous 30 days. An owner-approved `/botdepo` credit also qualifies. Once eligible, the full balance—including tips, rains, bonuses, and winnings—is withdrawable without an unfinished wager lock. All group withdrawal links should open `@rollersgamesbot`.

**Why:** The owner confirmed the deposit and `/botdepo` rules and explicitly said to keep `@rollersgamesbot` as the withdrawal bot.

**How to apply:** Enforce the shared deposit check on every withdrawal route, including amount/address submission, withdraw-all, and saved-address callbacks. Do not add a wager-progress gate after the qualifying deposit is recorded.
