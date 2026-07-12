# Search Guide

As this repository scales, manual navigation may become slower. Use these techniques to locate documents rapidly.

## Local Search (Grep/Ripgrep)

If you have cloned the repository locally, the fastest way to search is using terminal tools like `grep` or `rg` (ripgrep).

**Find all mentions of "WEF" in the ANALYSIS folder:**
```bash
grep -rnw 'ANALYSIS/' -e 'WEF'
```

**Find all documents citing "Reuters":**
```bash
grep -rnw 'ANALYSIS/' -e 'Reuters'
```

## GitHub Search

If viewing on GitHub, use the repository search bar with specific filters:

- `"keyword" in:file` – Searches within the contents of the files.
- `path:ANALYSIS/03_finance` – Restricts search to a specific directory.
