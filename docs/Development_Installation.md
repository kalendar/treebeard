[⬅Back](/README.md)
## Development Installation
Prerequisite: [Groq](https://console.groq.com/keys) API Key.
This application currently relies on Groq for rapid LLM responses, which is planned to be optional. Ideally, the LLM would run on device.

### [uv](https://github.com/astral-sh/uv) (Recommended)
1. Clone this repo and enter the root directory.
2. Run `uv sync` in the root directory.
3. Enter the python venv with either `.venv\Scripts\activate` on Windows, or `source .venv/bin/activate` on Unix.
4. Set environment variables, either in the terminal or in a `.env` file in the root directory. Example env:
```sh
treebeard_sqlite_database_path = "ab\path\to\db.db"
treebeard_grok_api_key = "groq_key"
treebeard_groq_model = "llama-3.3-70b-versatile"
```
5. Run `fastapi dev .\src\treebeard\`.

### pip (Alternative)
Prerequisite - Python 3.13
1. Clone this repo and enter the root directory.
2. Run `python -m venv .venv` in the root directory.
3. Enter the python venv with either `.venv\Scripts\activate` on Windows, or `source .venv/bin/activate` on Unix.
4. Run `pip install -r requirements.txt`.
5. Set environment variables, either in the terminal or in a `.env` file in the root directory. Example env:
```sh
treebeard_sqlite_database_path = "ab\path\to\db.db"
treebeard_grok_api_key = "groq_key"
treebeard_groq_model = "llama-3.3-70b-versatile"
```
6. Run `fastapi dev .\src\treebeard\`.