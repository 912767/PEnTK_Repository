# PEnTK Repository
Python Engineering Toolkit (PEnTk) is an open-source toolkit for stable, better engineering (or lab analysis) in a Python workflow.

# Features and limitations:

* Built for windows and vs code
* Requires human setup (instructions below)
* Better stability than Python alone
* Totally open source
* Uses UV to maintain software versions to prevent failure due to updates.
* Updates and installs must be done and checked for errors manually.

# FIRST TIME INSTALLATION INSTRUCTIONS

Install the Python interpreter in VS Code.

Installing uv (if you haven't already)

Windows: `powershell -ExecutionPolicy Bypass -c “irm https://astral.sh/uv/install.ps1 | iex”`

Linux/Mac: `curl -LsSf https://astral.sh/uv/install.sh | sh`

Close and reopen your terminal, then run `uv` to confirm it’s ready.

Open the VS Code terminal:
(Ctrl + ~) and run `uv sync`. This connects VS Code to load a specific stable virtual environment.
If this returns an error and uv is confirmed to be installed, close the VS Code window, reopen it, and run the above command again.

Connect VS Code to the Environment:
(Ctrl + Shift + P) Search for and select Python: Select Interpreter.
Choose the interpreter pointing to `./.venv/Scripts/python.exe` (Windows) or `./.venv/bin/python` (macOS/Linux).

# Single Use Scripts

Single-use scripts live within the “scripts” folder. To execute single-use scripts, simply run them in VS Code. Calling scripts is as such, e.g., `from pentk_repository import exampleFuncs`

# Loading Packages

To load external packages, you must use uv
ex: `uv add numpy pandas matplotlib`
to remove packages
ex: `uv remove numpy pandas matplotlib`

# My personal favored software.

numpy Documentation: https://numpy.org/doc/stable/

matplotlib https://matplotlib.org/cheatsheets/

polars Documentation: https://docs.pola.rs/