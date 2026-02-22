# FlashMD

A local, offline flashcard app that parses Markdown files into decks and studies them using SM-2 spaced repetition.

---

## Install

### Linux

```bash
git clone https://github.com/johnfire/flashmd-python
cd flashmd-python
bash install-linux.sh
```

Installs a virtual environment, the app, and a desktop launcher (shows up in your app menu).

> **Requires tkinter.** If the installer reports it missing:
> - Debian/Ubuntu: `sudo apt install python3-tk`
> - Fedora: `sudo dnf install python3-tkinter`

---

### macOS

```bash
git clone https://github.com/johnfire/flashmd-python
cd flashmd-python
bash install-mac.sh
```

Installs a virtual environment and creates `~/Applications/FlashMD.app`. Double-click it to launch, or drag it to your Dock.

> **Requires Python 3.10+.** Download from [python.org](https://www.python.org) or `brew install python`.
> If tkinter is missing: `brew install python-tk`

---

### Windows

1. Install [Python 3.10+](https://www.python.org) — check **"Add Python to PATH"** during setup
2. Clone or [download the ZIP](https://github.com/johnfire/flashmd-python/archive/refs/heads/main.zip) and unzip
3. Double-click **`install-windows.bat`**

Creates a virtual environment and adds **FlashMD** shortcuts to your Desktop and Start Menu.

---

## Markdown Format

A single `.md` file = one deck. Cards follow this pattern:

```
# Deck Title

## Category Name

**1. TERM — Full Term Name**
Definition paragraph.

Second paragraph if needed.
```

---

## Running from the terminal (all platforms)

```bash
# Linux / macOS
.venv/bin/flashmd

# Windows
.venv\Scripts\flashmd.exe
```

---

## Running Tests

```bash
pip install pytest
pytest
```

---

## License

MIT — Copyright (c) 2025 Christopher Rehm
