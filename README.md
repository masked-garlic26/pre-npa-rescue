# Pre-NPA Rescue

> We find credit card customers who are about to struggle, work out who we can actually help, offer them a kind and affordable plan, and prove the whole thing is fair, all before day 90.

Built for **Mission '26** (SCOPE x BIS Hack-a-thon, VIT Chennai) | Theme: FinTech

## The problem

Banks notice a struggling cardholder only after payments stop, then treat every defaulter the same way. By day 90 the account becomes an NPA (Non-Performing Asset): the bank provisions for the loss and the customer's credit is wrecked. This project intervenes *before* that happens.

## How it works

| Layer | What it does | Folder |
| --- | --- | --- |
| 1. Detect | Predicts who will miss payments in the next 30-60 days, explains why, and labels them Forgot / Can't pay / Won't pay | `detect/` |
| 2. Decide | Uplift model finds who will actually respond to contact; a policy engine approves what can be offered | `decide/` |
| 3. Resolve | Multilingual hardship chat that offers an affordable plan, with human handoff | `resolve/` |
| 4. Prove | Red-team tests (pressure, bias, prompt injection, privacy) and a fairness scorecard | `prove/` |

Data is fully synthetic (simulated cardholders). No real bank data is used.

## Project structure

- `data/` synthetic data generator
- `detect/` early-warning model
- `decide/` uplift model and policy engine
- `resolve/` hardship chat and relief engine
- `prove/` red-team harness and scorecard
- `app/` collector dashboard and customer chat UI
- `docs/` slides and architecture diagrams
- `tests/` automated tests

## How to run

_To be filled in during the hackathon._

## Team

- Mahin Kumar Padhi (@masked-garlic26)
- Gautam
- Nitheesh
- M Sharmesh (@sharmeshms)

## License

MIT
