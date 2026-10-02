# vecnotes-v2

Semantic search over local notes with embeddings

Built for my own use; public in case it helps someone.

## How to use

```bash
python search.py ./notes
>> how do I back up my database?
```

## Install

```bash
pip install -r requirements.txt
```

## What it does

- sentence-transformers when available, TF-IDF fallback
- Interactive REPL and one-shot modes
- Reranks by recency when scores tie
- Vectors cached to .npy so re-runs are instant

## Project structure

```text
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   └── pull_request_template.md
├── docs/
│   ├── development.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── requirements.txt
└── search.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## Notes

- mostly stable, edge cases remain

## License

MIT. Do whatever you want.
