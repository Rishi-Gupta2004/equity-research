# How I Use AI

I use Claude (Anthropic) as a research associate. The rules below decide what it does and what it never does. They were written before the first note, and every note is built to them.

## Division of labour

| I write | AI does |
|---|---|
| The thesis and the variant view | Pulls and reconciles data from filings, transcripts and data terminals |
| The pivotal questions and my answer to each | Proposes candidate pivotal questions, each tested against the four criteria |
| The rating, conviction and target price decision | Builds exhibits, tables and the three-statement history |
| Scenario probabilities | Drafts descriptive sections (industry, business, peers) at my direction |
| The three falsifiers (AI may propose candidates) | Writes the Red Team: the strongest case against my rating |
| The conclusion | Recomputes every number in Python and runs the Gate 4 tie-out |
| The decision journal | Runs an independent check of each draft against the sources |

## The rules that keep the thesis mine

- **AI never writes the thesis sentence, the variant view, the rating rationale or the conclusion.** If asked, it declines and asks the questions that help me write it myself.
- **No placeholders.** It doesn't draft a "rough version to react to" in any of my sections. A placeholder is a first draft with deniability, and editing one isn't the same as writing my own.
- **Gates are hard stops.** At each of the four gates in the [initiation structure](initiation-structure.md), drafting stops until my judgement goes in. A gate is never passed on an assumption.
- **The Red Team is labelled.** In the TYL initiation it is titled "Claude's Dissection" and written in an external voice, so the reader can see which argument is mine and which is the challenge to it.

## Why work this way

Used without rules, AI makes a note faster and less yours. Used with them, it does the work a junior associate would do: data, exhibits, checking, and an adversary who has read everything. The judgement stays with the analyst, and every judgement call can be traced to the person who made it.

## Tooling

Repeatable workflows are packaged as custom Claude skills I designed and maintain:

| Skill | What it produces |
|---|---|
| Business model analysis | The stage-one private workpaper |
| Top 10 must-knows | The quarterly earnings memo |
| Three-statement builder | An audit-ready Excel pull of historical statements, a peer multiples page and a GAAP-to-adjusted bridge |
| Model reset | Clears and repopulates Model RG for a new ticker from primary sources, with a sector hard-block and tie-outs |
| Sell-side initiation | Drives the 20-section structure and enforces the four gates |
| Exhibit | Print-quality charts in the house style |
| Thesis review | Restates the falsifiers verbatim and tests each against the latest filings |
