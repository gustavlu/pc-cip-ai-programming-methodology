# PC-CIP Spec Block Linter (Pre-Prompt Checklist)

Use this checklist before prompting an AI.

## Invariants
- [ ] Each invariant is binary (true/false)
- [ ] Each invariant is testable
- [ ] No vague language ("secure", "fast")

## Interfaces
- [ ] Inputs defined
- [ ] Outputs defined
- [ ] Schemas provided

## Causality
- [ ] All side effects listed
- [ ] Forbidden effects explicitly stated

## Failure Policy
- [ ] Default behavior defined
- [ ] Retries specified
- [ ] Idempotency addressed

## Acceptance Tests
- [ ] Minimal
- [ ] Directly map to invariants

If any box is unchecked, **do not prompt the AI yet**.

