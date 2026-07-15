# Evidence Locker — Agent Archiving & Sourcing Guide

**Target Audience**: AI Agents, Automated Scrapers, and Human Curators  
**Version**: 1.0  
**Purpose**: To ensure absolute permanence of all evidence cited in the Evidence Archives. "Link rot" is the enemy of historical accountability. This guide defines the exact workflow for securing and archiving sources.

---

## 1. The Golden Rule of Sourcing

**Never rely exclusively on a live URL.** 
Live URLs change, get memory-holed, or become paywalled. Every single piece of evidence cited in this repository must be frozen in time or downloaded locally. 

If a claim is important enough to be in the Evidence Locker, its source is important enough to be permanently archived.

---

## 2. Standard Operating Procedure for Web Links

When citing an article, press release, dataset, or web page, agents must follow this workflow:

### Step 1: Capture
- Archive the URL through the **Wayback Machine** (`web.archive.org`).
- Alternatively, or as a secondary backup, capture it via **Archive.today** (`archive.is` / `archive.ph`).

### Step 2: Format the Citation
When linking in the markdown (`.md`) files, you must use the archived link as the primary reference. 

**Format**: 
`[Source Title / Context](https://web.archive.org/web/YYYYMMDDHHMMSS/original-url)`

If you wish to include the live URL, include it as a secondary reference in the source table, but the primary hyperlinked text *must* point to the frozen archive.

---

## 3. Handling PDFs and Primary Documents

Critical government documents, think-tank whitepapers, and NGO reports are frequently quietly updated or deleted from the web. 

### Workflow for Documents:
1. **Download**: Pull the `.pdf`, `.csv`, or `.txt` file directly to the local environment.
2. **Store**: Save it in the repository's `DATA/` directory. Use a clear, standardized filename (e.g., `DATA/2026_IMF_COFER_Q1.pdf`).
3. **Link Local**: Link to the local `DATA/` path in your markdown entry.
4. **Link External (Backup)**: Include the Wayback Machine link to the original PDF URL as a secondary reference in the Claim-vs-Evidence table.

---

## 4. Media & Visual Evidence Policy

As mandated in the `METHODOLOGY.md` guide:
- **No placeholders**: Do not create "Pending" tables for images or media.
- **Local embedding**: If a visual asset (map, chart, infographic) is absolutely essential for context, it must be downloaded, saved to the `DATA/` folder, and embedded directly using relative paths.
- **No Hotlinking**: Do NOT hotlink images from external servers. They will inevitably break or be replaced.

---

## 5. Automation & Scripts

If you are an agent equipped with terminal access (`run_command`), you should proactively secure links. 

- If a `wayback_archiver.sh` or Python scraping script is available in the environment, use it to batch-archive all URLs before finalizing an Evidence Locker entry.
- **Verification**: Before writing an entry to `PUBLISH READY` status, do a dry-run check of the links to ensure the Web Archive captures were successful.

---

## 6. Handoff Checklist for Sourcing

Before ending your turn or handing off to the user, verify:
- [ ] All claims in the Claim-vs-Evidence table are backed by *archived* or *local* links.
- [ ] Any referenced PDFs or raw datasets have been downloaded to `DATA/`.
- [ ] No raw, live HTTP links are used as the sole point of failure for critical claims.
- [ ] No visual asset placeholders exist in the document.
