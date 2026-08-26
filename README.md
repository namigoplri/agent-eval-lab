# agent-eval-lab

Keyword-based eval runner with latency tracking

Started as a weekend hack, grew on me.

## Examples

```bash
python evals.py
# edit cases.json, point run() at your agent
```

## Installation

```bash
# stdlib only, nothing to install
```

## Highlights

- Keyword scoring + latency per case
- Cases defined in plain JSON
- Swap in any agent function via one line
- Exit code usable as a CI gate

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── pull_request_template.md
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
├── cases.json
└── evals.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## FAQ

**Is this production ready?**  
It works for my use case; review the code before relying on it.

**Why no framework?**  
The stdlib covers what this project needs.
