# EDI Order Exception Resolution Playbook (sample)

Upload this as a Knowledge file. Replace it with your team's real playbook.

## Standard lead time
Orders need at least 5 business days between PO date and requested delivery date.

## Exception types and owners

| Exception | Usual cause | Fix | Owner |
| --- | --- | --- | --- |
| Missing cross-reference | New customer part number not yet mapped | Add the mapping in the item cross-reference, then reprocess the PO | Master data team |
| Discontinued item | Customer ordering an end-of-life item | Ask the customer to reorder the replacement SKU | Customer service rep |
| UOM mismatch, converts cleanly | Customer ordered in eaches for a case-pack item | Convert to cases, confirm the price matches, release | Customer service rep |
| UOM mismatch, does not convert | Quantity is not a whole number of cases | Ask the customer to correct the quantity | Customer service rep |
| Invalid or inactive ship-to | Customer used an old or wrong location code | Ask the customer to confirm the correct ship-to and resend | Customer service rep |
| PO price below contract | Customer error or expired promotion | Ask the customer to correct the price | Customer service rep, with pricing team if over $5,000 |
| PO price above contract | Price increase not yet loaded in our system | Pricing team confirms and updates the price list | Pricing team |
| No contract price | Customer ordering outside their contract | Escalate to the account manager | Account manager |
| Date not feasible | Requested date inside lead time | Offer the earliest feasible date | Customer service rep |
| Possible duplicate | Customer resent the same PO | Confirm with the customer before processing either copy | Customer service rep |

## Escalation
Escalate any single issue worth more than $10,000, or any case where the evidence conflicts, to the order-to-cash supervisor.
