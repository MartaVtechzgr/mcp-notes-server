# mcp-notes-server

A small MCP server exposing my notes to Claude Desktop

## How to use

```bash
# claude_desktop_config.json
# {
#   "mcpServers": {
#     "notes-box": {"command": "python", "args": ["server.py"]}
#   }
# }
python server.py
```

## Install

```bash
pip install -r requirements.txt
```

## What it does

- State persisted to a JSON file in the home dir
- Three tools: add / get / list notes
- FastMCP style: decorators, zero boilerplate
- Includes Claude Desktop config snippet

## Project structure

```text
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── Makefile
├── requirements.txt
└── server.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## Known issues

- none reported yet (surprisingly)
