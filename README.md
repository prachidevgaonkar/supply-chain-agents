# Supply chain agents

No-code agent designs for supply chain teams, with ready-to-paste instructions for a main agent and its subagents, sample data, and an answer key for testing.

Each agent is designed as a one-week proof of concept: build it without code, test it against cases your team has already resolved, and decide whether it's worth a pilot.

| Agent | Process | Problem it solves |
| --- | --- | --- |
| [EDI Order Exception Triage](edi-order-exceptions/) | Order-to-cash | Diagnoses EDI purchase orders on hold, recommends the fix, and drafts customer emails |

## Ideas for more agents

- **Deductions and chargeback triage** (order-to-cash): classify retailer short-payments as valid or disputable, and draft disputes.
- **Three-way match exceptions** (procure-to-pay): explain why an invoice doesn't match the PO and goods receipt.
- **Supplier delay early warning** (procure-to-pay): flag supplier orders that will arrive after production needs them.
- **Freight invoice audit** (logistics): check carrier invoices against contracted rates and actual shipments.
- **Stockout and excess risk review** (planning): explain at-risk SKUs ahead of the weekly planning meeting.

## License

MIT
