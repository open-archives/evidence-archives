# Contributing to the Evidence Archive

This repository is designed as a living archive for verifying, documenting, and cross-referencing global events, structural strategies, and systemic operations. It is not a collection of opinions; it is an infrastructure for truth that scales.

## Architecture

Our archive follows a strict taxonomy to ensure clarity and scalability as we grow to 1,000+ documents.

- **`INDEX/`**: Contains the master table of contents and browse files (by theme, year, source).
- **`DATA/`**: Raw evidentiary files (PDFs, transcripts, datasets).
- **`ANALYSIS/`**: Curated markdown documents interpreting the data, placed into specific thematic folders (e.g., `01_geopolitics`, `03_finance`).
- **`TOOLS/`**: Scripts for scraping, backup, and indexing.

## How to Submit New Evidence

1. **Format:** All submissions must be written in Markdown (`.md`).
2. **Metadata:** Every file must begin with a Metadata block detailing:
   - Date / tracking period
   - Topic
   - Source (list of primary and secondary sources)
   - Status (Verified via [Method])
3. **Citations:** Cite primary sources. Link to original documents in the `Related Documentation` section. If possible, backup raw files to the `DATA/` folder and link them locally.
4. **Structure:** Adhere to the established format: Executive Summary, Timeline/Data tables, Notable Quotes, Related Documentation, Discrepancy Notes. Use data tables generously.
5. **No Opinions:** Present the facts, the rhetoric of key actors, and structural interconnections neutrally. 
6. **Pull Requests:** Submit a pull request to the `main` branch. A maintainer will review the submission for accuracy, citation standards, and structural compliance before merging.

*Remember: You are building infrastructure where truth accumulates faster than it can be removed.*
