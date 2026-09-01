# quant-research-lab

![CI](https://github.com/CeyhanTurnali/quant-research-lab/actions/workflows/ci.yml/badge.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

My research and development playground at the intersection of finance, AI,
and quantitative methods — portfolio optimization, macro regime analysis,
financial NLP, and market time-series modeling. Built as tested,
production-quality modules rather than one-off notebooks, and designed to be
dual-purpose: a public portfolio piece *and* a toolkit I actually use for my
own investment research.

`nlp/` is a temporary home for financial NLP baselines; once the representation
comparison matures (H10), the reusable pieces (`preprocess/`, `features/`,
`eval/`) graduate into a standalone package, [`financial-nlp-toolkit`](https://github.com/CeyhanTurnali/financial-nlp-toolkit).

## Status

| Area | Status | 
|---|---|---|
| optimization | 🟡 in progress | 
| nlp | 🟡 in progress | 
| macro | 🟡 in progress | 
| deep-learning | ⚪ planned | 
| attention | ⚪ planned | 
| sequence-models | ⚪ planned 

## Development

```bash
pip install -e ".[nlp,dev]"
pytest
ruff check .
```

## License

MIT — see [LICENSE](LICENSE).
