# flashmd-python

A local, offline flashcard app that parses Markdown files into decks and studies them using SM-2 spaced repetition.

## Requirements

- Python 3.10+
- tkinter (usually included with Python; on Debian/Ubuntu: `sudo apt install python3-tk`)

## Install & Run

```bash
git clone https://github.com/johnfire/flashmd-python
cd flashmd-python

python3 -m venv .venv
source .venv/bin/activate

pip install -e .
flashmd
```

Or without activating the venv:

```bash
.venv/bin/flashmd
```

## Markdown Format

A single `.md` file is one deck. Cards follow this pattern:

```
# Deck Title

## Category Name

**1. TERM — Full Term Name**
Definition paragraph.

Second paragraph if needed.
```

## Running Tests

```bash
pip install pytest
pytest
```

## License

MIT — Copyright (c) 2025 Christopher Rehm
