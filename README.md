# tokencost

Quick token/cost estimates for prompt budgeting

Built for my own use; public in case it helps someone.

## How to use

```bash
python cost.py prompt.txt --model gpt-4o-mini --expect-out 500
```

## Highlights

- Per-model pricing table in JSON
- Reports input/output tokens and USD estimate
- Zero dependencies
- Heuristic token estimate (~4 chars/token)

## Install

```bash
# stdlib only
```

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── SECURITY.md
├── cost.py
└── pricing.json
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```
