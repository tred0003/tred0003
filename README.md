### Derik Treuel, AI Engineer

I spent 13 years advising clients at Merrill Lynch and Empower. Now I build AI systems on Google Cloud.
I'm a Google Cloud Certified Professional Machine Learning Engineer and Generative AI Leader.

How I work: I write the spec, the baseline to beat and the eval gate. Claude Code writes most of the
code, I review the changes, and the evals decide what ships. That's why my commits are co-authored with Claude.

[LinkedIn](https://www.linkedin.com/in/derik-treuel-495b2673/) · [rygiene.app](https://rygiene.app)

#### [sec-10k-document-intelligence](https://github.com/tred0003/sec-10k-document-intelligence)

Pulls financial-statement numbers out of SEC 10-K PDFs with Document AI and Gemini, then checks them
against the SEC's own XBRL data. On 20 companies it never saw, it got 87.8% right, compared with 62.2%
for a keyword baseline. Banks are still the weak spot. It also answers questions with page citations:
re-ranking took MRR@10 from 0.29 to 0.71, and a LlamaIndex rebuild got 93% of 271 held-out questions right.

#### [nfl-dfs-gameday-agent](https://github.com/tred0003/nfl-dfs-gameday-agent)

A Gemini agent on Google Cloud that writes a daily report on each user's fantasy lineup. Tests run
on every push, and the agent can't deploy until it passes an eval gate. I built the Q&A feature both
as an agent and as a fixed pipeline, graded 680 answers, and the pipeline won, so that's what shipped.
I also found the cost meter was missing most of the bill, fixed it, and cut cost per report 68%.

#### Rygiene (live app, private code)

An e-bike safety app for parents. Phones upload rides, workers score them for speeding, phone use and
night riding, and parents get notified. It's been live on iOS and Android since mid-2026. The code is
private because it's a business, but I'm happy to walk through it.
