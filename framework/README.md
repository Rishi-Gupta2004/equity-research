# How I Research

Research is run like a small sell-side desk, with written rules that sit above any single note. The rules matter more than any one call: they are what make a call checkable after the fact.

## The pipeline

| Stage | Output | Published? |
|---|---|---|
| 1. Business model analysis | A long-form teardown of how the company makes money: revenue architecture, unit economics, margin and working capital mechanics, moat, failure modes, and what the price implies | No, private workpaper |
| 2. Earnings memos | A ten-point memo on each quarter: reported against consensus, KPI dashboard, guidance credibility tracker, what changed in the debate | No, private workpaper |
| 3. Three statements and model | Historical statements pulled from filings, then a forecast, DCF, reverse DCF and Monte Carlo in [Model RG](../models/model-rg/) | Screenshots only |
| 4. Initiation of coverage | About 24 pages in one PDF, built to a fixed [structure](initiation-structure.md) and passed through four gates | Yes |
| 5. Monitoring | Falsifier status each quarter, thesis update notes, and the [track record](../research/README.md) | Yes |

## Standing rules

1. **The reverse DCF leads.** Every valuation section opens with what the current price already requires (growth, margin, reinvestment, return on capital), then argues why that path is wrong. The target price follows from that argument.
2. **The method fits the business.** A forward DCF for a single business with steady cash flows; sum of the parts where segments have different economics; multiples on a named comp set where a DCF is unreliable. The choice and the reason are stated in the note.
3. **Three falsifiers, committed before publication.** Each one is specific, observable and dated. "Organic SaaS growth below 18% for two consecutive quarters" counts. "Macro deteriorates" does not. A falsifier can't simply be a share price fall.
4. **Every note argues against itself.** The Red Team section makes the strongest available case against the rating. It must attack at least one pivotal question directly and test whether the falsifiers can fire at all.
5. **Primary sources first.** Filings, then terminal data, then secondary sources for context only, labelled as such.
6. **Evidence is tagged in workpapers.** Every claim is marked as reported, a management claim, an inference or a proxy. A guess must never read like a disclosure.
7. **Numbers are computed, not typed.** Every table total, ratio and page budget is recalculated in Python and the check is kept. Errors cluster in tables, because prose gets reread and tables get pasted.
8. **One reference price per note,** stated once and used everywhere.
9. **A call is never edited after publication.** Changes go into a dated thesis update.

## Documents

| Document | What it covers |
|---|---|
| [Initiation structure](initiation-structure.md) | Section map, page budget, the four gates, how pivotal questions are tested |
| [Quality control](quality-control.md) | The pre-publication tie-out, and errors found in published broker notes that shaped it |
| [Investment policy](investment-policy.md) | The notional portfolio's mandate, benchmark, sizing, entry and exit rules |
| [House style](house-style.md) | Layout, type, colour and exhibit rules for published notes |
| [How I use AI](ai-workflow.md) | Who does what, and the rules that keep the thesis mine |
