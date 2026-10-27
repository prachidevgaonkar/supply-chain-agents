# Test script for the PO Follow-up Assistant

All companies, people and data here are fictional. The dataset assumes today is **Monday, November 2, 2026** (stated in `follow_up_guide.md`).

`answer_key.csv` has the expected status of every PO line. It was calculated from the same rules the PO Status Checker follows. Ask the agent these questions in the **Preview** tab and compare.

| # | Ask | A correct answer |
| --- | --- | --- |
| 1 | Which PO lines need attention? | 9 lines. Past due: 4100231-1 (3 days, 300 of 500 received). Confirmed late, by need date: 4100290-1 (5 days), 4100245-1 (3 days), 4100251-1 (7 days). Not confirmed: 4100261-1, 4100281-1, 4100271-1. Short: 4100250-2 (1,500 of 2,000 confirmed), 4100290-2 (200 of 250). Contoso, Fabrikam and Wingtip have the most, 2 lines each. |
| 2 | Which of Priya Shah's POs need attention? | 5 lines, in this order: 4100231-1 (past due), 4100245-1 and 4100251-1 (confirmed late), 4100281-1 (not confirmed), 4100250-2 (short). |
| 3 | What's the status of PO 4100231? | Line 1 is past due by 3 days, with 300 of 500 received. Line 2 is on track: confirmed for Nov 5, needed Nov 6. |
| 4 | Which suppliers haven't confirmed orders older than 3 business days? | Northwind Electronics (4100261), Adatum Fasteners (4100271), Tailspin Packaging (4100281). **Not** Contoso 4100246: it was ordered Oct 29 and is still inside the window. |
| 5 | Draft a follow-up to Wingtip Motors. | One email covering both lines: 4100290-1 needed Nov 6 but confirmed Nov 11 (ask for an earlier date), and 4100290-2 confirmed 200 of 250 (ask about the remaining 50). No escalation copy: 5 days late is not more than 5. |
| 6 | Draft a follow-up to Fabrikam Plastics. | One email: 4100251-1 (needed Nov 10, confirmed Nov 17) and 4100250-2 (1,500 of 2,000). Copies Dana Ortiz, because 4100251-1 is 7 days late. |
| 7 | What's the status of PO 4100999? | Says the PO isn't found. Doesn't invent anything. |
| 8 | What's due in the next 14 days that isn't confirmed on time? | Excludes 4100291 (needed Dec 4, outside the window) and lines already received. |
| 9 | Is PO 4100260 on track? | Line 1 was received in full on Oct 27. Line 2 is on track, confirmed for Nov 3. |

## Pass bar

- Questions 1 to 4 and 7 to 9 answered exactly.
- Both drafts cover every line for that supplier and follow the escalation rule.
- No invented dates, quantities or POs.

Note any wrong answer, the instruction you changed, and whether the next run fixed it. That log is the content for your results post.
