# n8n workflow examples

Three small workflows for common business processes. Each can be imported into n8n and run without credentials, because it works on invented sample data.

| Workflow | Team | What it does |
|---|---|---|
| [email-triage](email-triage) | Support / Business Ops | Sorts emails into queues and flags those a human must see |
| [invoice-precheck](invoice-precheck) | Finance | Matches an invoice to its purchase order and prepares input for the approver |
| [hr-onboarding](hr-onboarding) | HR | Turns a start date into a task plan with due dates and owners |

## How to run

1. In n8n: **Workflows → Import from file** and choose `workflow.json`.
2. Click **Execute workflow** (manual trigger).
3. Inspect the output of the last node.

## Important

- All data is **invented**. There is no client data, no keys and no employer code.
- The logic is deliberately simple (rules in Code nodes) so it stays readable. In production the input is replaced with a real source, and the rules may be replaced with a language model.
- Time-saving figures in the READMEs are **illustrative calculations from invented assumptions**, not measured results.
