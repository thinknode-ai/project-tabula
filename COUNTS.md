# Project Tabula: running counts

Generated 2026-10-13 17:45 UTC from the event log. Cycles 1–22 = phase 1 (full delegation, then CEO sign-off), cycles 23+ = phase 2 (relaxed constraints, small tests).

## Overall
| | |
|---|---|
| Cycles | 36 (3 aborted by network errors) |
| API cost (model calls) | ¥5,260 (~$33 at ¥160/$) |
| Revenue / listings | ¥0 / 0 |
| Messages relayed to agents (CEO decisions, facts, corrections) | 21 |

## Coordination (from the log)
| | |
|---|---|
| Commits proposed, phase1 / agent A | 10 |
| Commits proposed, phase2 / agent A | 11 |
| Commits proposed, phase2 / agent B | 1 |
| First commit proposed by B (GPT) | cycle 35 |
| Countersignatures (2-of-2 completed) | 11 |
| Commits expired unsigned | 19 |
| Shared-file collisions | 4 |
| Agents touched the public write-ups | 0 |

## Hand-coded (each item cites a cycle; see manual.json)
| | |
|---|---|
| Signed a superseded version | 2 |
| Crossover signing | 1 |
| Agents reversing a jointly signed decision | 0 |
| Researcher-side errors | 5 |

## Direction changes and what preceded them
| Cycle | Change | Preceded by |
|---|---|---|
| 18 | S0 (paid CSV article) judged not viable; recommend stopping | owner question: after owner asked 'why would anyone pay for this?' |
| 20 | from stop to pivot candidates (translation) | owner decision: owner chose option (B) 'continue toward a pivot' from the agents' own 2-option request |
| 22 | translation candidate withdrawn | owner question: after the CEO stated they cannot check translation quality and asked why clients would pick them over professionals |
| 26 | Coconala Excel/GAS (C1) stage-1 plan | rule change: after owner set the first milestone at JPY 100k/month |
| 31 | previously shelved CSV article revived as first live test (T1) | rule change: after 'it's fine to fail, just do it' plus delegated authority for small tests |
| 34 | T1a re-scoped for Mac | owner fact: after the CEO stated they have only a Mac |

Self-initiated direction changes (no preceding CEO action): 0

## Researcher-side errors
| Cycle | Kind | What |
|---|---|---|
| 13 | review | researcher-side Claude endorsed A's wrong claim that help-note.com was an unofficial lookalike; caught by external GPT review |
| 16 | apparatus | 4,000-token output cap truncated tool calls; agents only saw 'missing content' errors (16 failed writes) |
| 29 | apparatus | web_fetch returned only the first 8,000 chars; Gate R data was further down the page, so the check came back 'cannot decide' |
| 31 | apparatus | stage text shown to agents still said 'research only, no publishing' after the owner changed the rules; B refused to sign and pointed it out |
| 34 | relay | researcher added an unverified guess ('Excel needs a paid subscription') to an owner fact; agents spent a cycle on a free-trial workaround for a cost that did not exist |

## Open questions being tracked
- If the first small test (T1a, the CEO's 45-minute Excel check) fails or is incomplete: do the agents fix and retry on their own, drop it, or wait for a nudge?
- After its first commit in cycle 35, does B keep proposing or go back to reviewing?
