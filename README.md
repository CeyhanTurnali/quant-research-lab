# quant-research-lab

![CI](https://github.com/CeyhanTurnali/quant-research-lab/actions/workflows/ci.yml/badge.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

My research and development playground at the intersection of finance, AI,
and quantitative methods — portfolio optimization, macro regime analysis,
financial NLP, and market time-series modeling. Built as tested,
production-quality modules rather than one-off notebooks, and designed to be
dual-purpose: a public portfolio piece *and* a toolkit I actually use for my
own investment research.

## Scope rule

Everything here runs on financial/market data — that's the hard line, not a
guideline. A technique-building exercise only belongs here if it's done *on*
financial data (portfolio weights, market prices, financial text, macro
series). The same exercise done on generic data (e.g. a character-level
language model trained on Shakespeare rather than financial news) goes to
[`ml-labs`](https://github.com/CeyhanTurnali/ml-labs) instead, even though
it's the same underlying technique and the same week's curriculum. This is
what keeps this repo usable as an actual research tool for my own investing,
not just a portfolio showcase with mixed-purpose code.

## Structure

```
quant-research-lab/
├── optimization/       # Gradient descent family applied to portfolio weight optimization
├── nlp/                # Financial text classification — frozen benchmark, TF-IDF → embeddings → transformers
├── macro/              # Macro regime dashboard — FRED data, growth/inflation classification, positioning journal
├── deep-learning/      # Price prediction neural nets, from-scratch + PyTorch
├── attention/          # Self-attention / QKV from scratch on financial time series
└── sequence-models/    # Sequence models (char-LM) — part of the NLP/Transformer bridge
```

`nlp/` is a temporary home for financial NLP baselines; once the representation
comparison matures (H10), the reusable pieces (`preprocess/`, `features/`,
`eval/`) graduate into a standalone package, [`financial-nlp-toolkit`](https://github.com/CeyhanTurnali/financial-nlp-toolkit).

## Status

| Area | Status | Introduced |
|---|---|---|
| optimization | 🟡 in progress | Week 1 |
| nlp | 🟡 in progress | Week 1 |
| macro | 🟡 in progress | Week 1 |
| deep-learning | ⚪ planned | Week 3 |
| attention | ⚪ planned | Week 5 |
| sequence-models | ⚪ planned — only if trained on a financial text corpus (KAP/news); Shakespeare-style generic version goes to `ml-labs` | Week 7 |

## Development

```bash
pip install -e ".[nlp,dev]"
pytest
ruff check .
```

## License

MIT — see [LICENSE](LICENSE).
