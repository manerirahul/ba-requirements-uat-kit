# Acceptance Criteria Checklist (pre-sign-off)

Run through this list before asking a business owner to sign off. Every box
must be checked or explicitly waived in writing.

## Requirements

- [ ] Every in-scope BRD requirement has at least one user story.
- [ ] Every user story has acceptance criteria in Given / When / Then form.
- [ ] Every acceptance criterion is testable by someone other than the author.
- [ ] Edge cases and exceptions are written down, not assumed.
- [ ] Out-of-scope items are listed explicitly (no "we'll see").

## Traceability

- [ ] Every requirement appears in the RTM.
- [ ] Every requirement maps to a design/build reference.
- [ ] Every requirement maps to at least one UAT script.
- [ ] Every UAT script maps back to a requirement (no orphan tests).

## Testing

- [ ] UAT scripts cover happy path, negative path, and edge cases.
- [ ] Test data and environment are documented per script.
- [ ] Every script has a recorded Pass / Fail, not a verbal "looks good".
- [ ] Every defect is logged with severity and status.
- [ ] Failed scripts have a retest recorded after the fix.

## Sign-off

- [ ] Business owner has reviewed the RTM, not just the demo.
- [ ] Known limitations are listed in the sign-off, not discovered later.
- [ ] Sign-off is dated and attributed to a named approver.
