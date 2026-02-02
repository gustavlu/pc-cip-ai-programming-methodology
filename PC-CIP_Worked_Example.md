# PC-CIP Worked Example (End-to-End)

## Problem
Build an API endpoint that creates an order without duplicate charges.

---

## Spec Block (Excerpt)

HARD INVARIANT:
- A payment must never be charged more than once.

CAUSALITY MAP:
- Trigger: POST /order
- Command: CreateOrder
- Allowed Effects: DB.insert, Payment.authorize
- Forbidden Effects: Payment.capture twice

FAILURE POLICY:
- Idempotent order creation
- Deny on ambiguity

---

## Design Skeleton
- Controller
- OrderService
- PaymentAdapter
- IdempotencyStore

---

## Proof Pack (Excerpt)

| Invariant | Enforcement | Test | Monitoring |
|---------|-------------|------|------------|
| No duplicate charge | Idempotency key | test_idempotent_charge | duplicate_charge_metric |

---

## Result
The AI implementation is provably constrained by the invariant.

