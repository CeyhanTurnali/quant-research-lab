# macro

Macro regime dashboard: FRED data ingestion, growth/inflation z-score
composites, 2x2 regime classification, horizon (NOW/NEXT/PIPELINE)
projections, and a positioning journal.

**Action needed:** this folder is a placeholder. Copy in the existing local
`macro/` package (`series.py`, `fetch.py`, `transform.py`, `regime.py`,
`horizon.py`, `plot.py`, `journal.py`) and `makro-playbook-H1.md` from your
Week 1 macro work — that content already exists locally, it just didn't have
a repo home until now.

Install macro-specific dependencies with:

```bash
pip install -e ".[macro,dev]"
```
