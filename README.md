Make sure you have uv installed (suggestion: use `pipx`)
```
pipx install uv
```

Create the directory and everything you need:
```
uv init uv-demo
cd uv-demo
```

Python will already be set for you!
```
> more .python-version
3.13
```

Add the `wat` and `whenever` packages (the former to the `dev` dependency group) to the
`pyproject.toml` file.
```
uv add --dev ruff
uv add whenever
```
(Note, this will automatically add the virtual environment, too)

Activate your environment! (although, you don't even need this)
```
. .venv/bin/activate
```

Run `ruff`:
```bash
uv run ruff format .
```

