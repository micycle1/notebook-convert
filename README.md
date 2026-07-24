# notebook-convert

Drop `.ipynb` files in, get their Python source out. Runs entirely in the browser — no upload, no build step, no dependencies. Open `notebook-to-python.html` and go.

Built for pasting notebooks into an LLM, so it optimizes for that: token counts up front, tracebacks preserved, one button to copy everything.

## Options

| Option | Effect |
|---|---|
| Markdown, as comments | Prose cells included, prefixed `#` |
| Printed output and errors | stdout/results as `#>`, stderr/tracebacks as `#!`, ANSI stripped |
| Cell separators | `# %% [code] cell N` markers |
| IPython magics | Off: `%`/`!`/`?` lines commented out. On: left as-is |
