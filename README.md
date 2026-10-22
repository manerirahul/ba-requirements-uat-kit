# BA Requirements & UAT Kit

The templates a Business Analyst actually reuses on every project: capture the
requirement once, trace it to a test, and prove it passed — without reinventing
the paperwork each time.

## Templates

| File | Use it for |
| --- | --- |
| `templates/BRD-template.md` | Business Requirements Document — the agreed scope, rules, and measures |
| `templates/user-story-template.md` | User stories with acceptance criteria that a tester can execute |
| `templates/requirements-traceability-matrix.csv` | Trace each requirement → design → test → result (RTM) |
| `templates/UAT-test-script-template.md` | Step-by-step UAT scripts with expected results and pass/fail |
| `templates/acceptance-criteria-checklist.md` | A pre-sign-off checklist so nothing ships on a verbal "looks good" |

## Worked example

`examples/fictional-order-status-workflow.md` shows all five templates filled in
for one small, **fictional** scenario (a neighborhood bakery's online order
status page). It is deliberately small and fictional so the *shape* of good
artifacts is visible without any real project data.

## How to use this kit on a real project

1. Start with the BRD: problem, in-scope / out-of-scope, stakeholders, business rules.
2. Break the BRD into user stories; every story gets acceptance criteria in
   Given / When / Then form.
3. Log every story in the RTM the day it is written — not at the end.
4. Write UAT scripts from the acceptance criteria, not from memory.
5. Sign off against the checklist, with the RTM as evidence.

## Data note

No real project, employer, or client data is used anywhere in this repo.
The example is fictional and labeled as such.
