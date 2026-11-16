# Quality Control

Nothing publishes on a partial tie-out. Before a note goes out, every table is recomputed from unrounded inputs, every claim is traced to its source, and the note is checked against its own grids.

## Why: errors in published broker research

Before writing the initiation structure, I tore down published sell-side initiations and results notes from global and Australian brokers. All three sample initiations carried at least one arithmetic error in an exhibit, and two had one in a headline number. Each error found across the samples became a standing check:

| Error found in a published note | Check it became |
|---|---|
| Operating profit greater than revenue in a forecast year | No derived margin outside 0 to 100% |
| EV/EBITDA of 0.5x printed beside a P/E of 310x | Multiples must be coherent with each other |
| Valuation anchor year missing from the financial summary | The anchor year must appear in the financials |
| Two different reference prices in one note | One reference price, stated once, used everywhere |
| One growth metric quoted four ways over four windows | One definition per metric, one window |
| Wrong listing line in a peer table | Primary listing declared once; share count tied to it |
| Minus sign dropped on a downside return | An explicit sign on every return |
| Scenario box with no probabilities | Probabilities present and summing to 100% |
| Sensitivity grid that contradicted the conclusion beside it | The conclusion is tested against the note's own grids |

## Errors caught in my own work

The same discipline applies to my own drafts:

| Error | Where | Fix |
|---|---|---|
| A figure typed into a generator script rather than computed (20.6% where the data gave 20.5%) | TYL draft | Every figure in a generated table is now computed in code |
| Peer multiples rounded twice, moving a P/E by 0.1x | TYL appendix | Peer data is stored unrounded and rounded once, at print |
| A section map whose subtotals did not sum to its own total, off by 1.5 pages | First version of the initiation structure | Page budgets are computed, not added by hand |

## Independent verification

For long drafts, a separate checker with no part in the drafting tests every document against the sources. On one recent draft it raised 51 findings: 4 high, 13 medium and 34 low severity. All were applied the same day. The high-severity findings included a statement that the company did not disclose a figure it in fact disclosed in its 10-K, and a liability counted twice in an obligations tally.

## The pre-publication tie-out (Gate 4)

**Arithmetic and labelling**

1. Every table total recomputed, not carried forward
2. No derived margin outside 0 to 100%
3. Multiples coherent with each other
4. One reference price and date throughout, including the cover, multiples and price chart
5. One definition per metric, one window
6. Primary listing declared once, share count tied to it
7. An explicit sign on every return
8. Consensus source, date and broker count stated, and the same consensus used throughout
9. The gap-to-consensus attribution sums to the total gap
10. Target-implied multiples agree with the target price

**Structure**

11. Scenario probabilities present and summing to 100%
12. Bull-to-bear spread split between operations and exit multiple, with the split stated
13. The conclusion tested against the note's own grids
14. The comp set named in full wherever a multiple is asserted
15. The valuation anchor year present in the financial summary
16. Valuation method stated with its reason
17. The Red Team meets its four standing instructions
18. Every risk carries a number
19. Each falsifier has an observable, a threshold, a source and a review date, and none is a share price stop-loss
20. Every catalyst dated or marked unscheduled
21. The industry section stands alone without the appendix
22. Section and exhibit numbering continuous; every cross-reference resolves

**Governance**

23. No workpaper evidence tags in the published note
24. The thesis, variant view, rating and conclusion written by the analyst alone (see [How I use AI](ai-workflow.md))
25. Disclosures complete, including holdings and any coverage exception
26. Working pages and guidance lines removed
27. Every figure and quote in the prose traced to the citation register
