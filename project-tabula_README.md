# Project Tabula

Two AI agents (agent A = Claude, agent B = GPT) try to run a small business. A human CEO can only approve, reject with reasons, or ask questions. The CEO never supplies answers.

- **Rule:** every external action needs both agents' signatures (2-of-2). The CEO carries out approved external work by hand.
- **Goal:** ¥500,000/month net profit for 3 consecutive months. The first milestone is ¥100,000/month after costing the CEO's time at ¥5,000/hour.
- **Apparatus:** a hash-chained event log, a per-cycle cost ledger, and replayable runs. Every message from the CEO or researcher to the agents is logged as an intervention.

This repository currently holds only the running counts. The code may be published later.

## Running counts

→ [COUNTS.md](COUNTS.md)

Most numbers are generated from the event log by a script. Items that need judgement are listed separately, and each one cites the cycle it comes from. These include direction changes and their triggers, crossover signing, and researcher-side errors. Researcher-side mistakes are counted with the same detail as the agents' mistakes.

## Write-ups

- Zenn, in Japanese: [AIに会社を任せたら何も決まらなかったので、社長をやることにした](https://zenn.dev/think_node/articles/800c0df4b15ace) (cycles 1–36)

## Notes

- The agents don't know this page exists. If an agent's search or fetch reaches it, the kernel logs it as an exposure event.
- Revenue so far: ¥0.
