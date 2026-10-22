# Worked Example (FICTIONAL): Neighborhood Bakery — Online Order Status Page

> **Fictional scenario.** No real business, employer, or client is involved.
> The bakery, its staff, and its customers are invented to show how the kit's
> templates fit together on one small change.

## Problem (BRD excerpt)

Customers phone the bakery to ask "is my order ready?" Staff interrupt baking
to check and answer. Goal: let customers see live order status online, and cut
status-check calls.

**Success measure:** status-check calls drop within 4 weeks of launch.

## Requirements

| ID | Requirement | Priority |
| --- | --- | --- |
| BR-01 | Customer can view live order status using order number + phone number | Must |
| BR-02 | Staff can update an order's status (Received → Preparing → Ready → Collected) | Must |
| BR-03 | Status page shows an estimated ready time | Should |

## User story (US-01, traces to BR-01)

> As a customer,
> I want to check my order status online,
> So that I don't have to phone the bakery.

**Acceptance criteria:**

- **AC1:** Given a valid order number and phone number, when I submit them,
  then I see the current status and estimated ready time.
- **AC2:** Given a wrong phone number for the order, when I submit them,
  then I see "We couldn't find that order" and no order details.
- **AC3:** Given a collected order, when I check it, then I see "Collected"
  and no estimated ready time.

## RTM rows

| Req | Story | UAT script | Result |
| --- | --- | --- | --- |
| BR-01 | US-01 | UAT-01 | (filled at test time) |
| BR-02 | US-02 | UAT-02 | (filled at test time) |

## UAT script (UAT-01, traces to US-01)

| Step | Action | Expected result |
| --- | --- | --- |
| 1 | Enter valid order number + matching phone number | Status + estimated ready time shown |
| 2 | Enter valid order number + wrong phone number | "We couldn't find that order", no details shown |
| 3 | Enter a collected order's details | Status "Collected", no estimated ready time |

## What this example is showing

One requirement → one story → testable acceptance criteria → one UAT script
→ one RTM row. That chain, repeated at real-project scale, is the whole kit.
