# tidyfeed-hq

Small pandas pipeline that cleans messy CSV exports

Side project, maintained when I have time.

## Install

```bash
pip install -r requirements.txt
```

## Highlights

- Writes a cleaning report next to the output
- Drops duplicates, trims strings, normalizes dates
- Chunked reading for files that do not fit in memory
- Config-driven column renames and type casts

## How to use

```bash
python pipeline.py raw.csv --config config.yaml --out clean.csv
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── faq.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── LICENSE
├── config.yaml
├── pipeline.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## Acknowledgments

- README structure inspired by popular OSS templates
- Thanks to everyone opening issues with ideas
