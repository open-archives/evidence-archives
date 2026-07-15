# Evidence Locker — Formatting & Methodology Guide

**Version**: 1.0  
**Last Updated**: 14 Jul 2026  
**Purpose**: This document defines the formatting standards, methodological principles, and workflow conventions for all Evidence Locker entries. It ensures consistency across the archive and provides clear guidance for future work and handoffs.

---

## Table of Contents

1. [Project Philosophy](#1-project-philosophy)
2. [Repository Structure](#2-repository-structure)
3. [Document Formatting Standards](#3-document-formatting-standards)
4. [Entry Template](#4-entry-template)
5. [Writing Methodology](#5-writing-methodology)
6. [Claim-Vs-Evidence Framework](#6-claim-vs-evidence-framework)
7. [Cross-Reference Standards](#7-cross-reference-standards)
8. [Status & Versioning](#8-status--versioning)
9. [Media Policy](#9-media-policy)
10. [Handoff Guidelines](#10-handoff-guidelines)

---

## 1. Project Philosophy

The Evidence Locker is an archive of **evidence-based, analytically balanced, and source-grounded** entries on topics of geopolitical, economic, historical, and social significance.

### Core Principles

| Principle | Description |
|-----------|-------------|
| **Truth-seeking over narrative** | Follow the evidence even when it complicates preferred stories |
| **Evidence over opinion** | Claims must be supported by data; inferences are labeled as such |
| **Balance over advocacy** | Present counter-arguments and alternative perspectives where they exist |
| **Clarity over obfuscation** | Write for a reader who wants to understand, not be persuaded |
| **Permanence over timeliness** | Entries are designed to be read years from now, not just today |
| **Sourcing over speculation** | Cite sources at the claim level; primary sources preferred |

### What This Archive Is Not

| Misconception | Reality |
|---------------|---------|
| A blog | It is a structured, permanent reference |
| Advocacy journalism | It presents evidence, not advocacy |
| A conspiracy repository | It documents documented facts, not speculation |
| A real-time news source | It is analysis, not reporting |

---

## 2. Repository Structure

### Main Repo: `evidence-archives`

```
ANALYSIS/
├── 01_geopolitics/
├── 02_infrastructure/
├── 03_finance/
├── 04_elite-networks/
├── 05_military-industrial/
├── 06_media-information/
├── 07_social-control/
├── 08_political-funding/
├── 09_conspiracy-theories/
├── 10_colonialism/
├── 11_tech-industrial-great-power/
└── README.md

INDEX/
├── BY_SOURCE.md
├── BY_THEME.md
├── BY_YEAR.md
└── SEARCH_GUIDE.md

DATA/
README.md

TOOLS/
README.md
```

---

## 3. Document Formatting Standards

### File Naming

| Element | Convention | Example |
|---------|------------|---------|
| **Entry IDs** | `EL-{CATEGORY}-{NUMBER}` | `EL-FINANCE-01` |
| **File names** | `EL-` prefix for quick identification, lowercase, hyphen-separated, descriptive | `EL-FINANCE-03-brics-energy-axis-2026.md` |
| **Series folders** | Two-digit number + topic | `03_finance/` |

### Headings

| Level | Format | Example |
|-------|--------|---------|
| H1 | # Title (only in READMEs) | `# Evidence Locker Entry: ...` |
| H2 | ## Part 1: Title | `## Part 1: The Creation (1944)` |
| H3 | ### 1.1 Subsection | `### 1.1 The Gathering` |
| H4 | #### 1.1.1 Sub-subsection | `#### 1.1.1 The Delegates` |

### Tables

Use GitHub-flavored markdown tables:

```markdown
| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Content  | Content  | Content  |
```

### Code/Diagram Blocks

Use triple backticks with language:

```text
┌─────────────────────────────────────────────┐
│           DIAGRAM / ASCII ART               │
└─────────────────────────────────────────────┘
```

### Emphasis

| Element | Format | Example |
|---------|--------|---------|
| **Bold** | `**text**` | **Key concept** |
| *Italic* | `*text*` | *source citation* |
| `Inline code` | `` `text` `` | `EL-FINANCE-01` |

---

## 4. Entry Template

All entries follow this standard structure:

```markdown
# Evidence Locker Entry: [Title]

**Archive ID**: `EL-{CATEGORY}-{NUMBER}`  
**Series**: [Series Name]  
**Compiled Date:** [Date]  
**Version:** [X.X]  
**Status:** [DRAFT / PUBLISH READY / ARCHIVED]  
**Tags:** `#tag1` `#tag2`

---

## Executive Summary

[2-4 paragraphs summarizing the entry's core argument and findings]

---

## Part 1: [Section Title]

[Content with tables, diagrams, and analysis]

---

## Part 2: [Section Title]

[Content with tables, diagrams, and analysis]

---

## Part [N]: Claim‑vs‑Evidence Table

| Claim | Supported by Data? | Source Evidence | Qualifiers |
|-------|-------------------|-----------------|------------|
| ... | ✅ Yes / ⚠️ Partially / ❌ No | ... | ... |

---

## Part [N+1]: Cross-References to Evidence Locker

| Existing Document | Connection |
|-------------------|------------|
| `EL-XXX-YYYY` | ... |

---

## Part [N+2]: Archive Metadata

| Field | Value |
|-------|-------|
| **Archive ID** | `EL-{CATEGORY}-{NUMBER}` |
| **Version** | X.X |
| **Status** | [DRAFT / PUBLISH READY] |
| **Related Entries** | `EL-XXX`, `EL-YYY` |
| **Licensing** | CC-BY-NC |

---

**Navigation**: [← Return to [Index]](./README.md) | [Evidence Locker Main →](../../README.md)
```

---

## 5. Writing Methodology

### Tone

| Do | Don't |
|----|-------|
| Write in a neutral, analytical tone | Use emotional or sensationalist language |
| Present evidence before conclusions | Lead with conclusions |
| Acknowledge uncertainty | Present speculation as fact |
| Cite sources at the claim level | Make claims without attribution |
| Use qualifiers ("likely," "suggests," "indicates") | Make absolute statements where evidence is incomplete |

### Language Guidelines

| Element | Rule | Example |
|---------|------|---------|
| **Past tense** | Use for historical events | "The Bretton Woods system was established in 1944" |
| **Present tense** | Use for analysis of current systems | "The dollar accounts for 57.13% of global reserves" |
| **Active voice** | Preferred over passive | "The U.S. closed the gold window" (not "The gold window was closed") |
| **Third person** | Avoid "I" or "we" | Use the evidence itself as the subject |

### Source Citation

| Source Type | Format | Example |
|-------------|--------|---------|
| **Academic** | Author, Year, Title | "Triffin, 1960, *Gold and the Dollar Crisis*" |
| **Primary** | Institution, Document, Year | "U.S. Treasury, TIC Data, May 2026" |
| **News** | Publication, Date | "Bloomberg, July 14, 2026" |
| **Data** | Source, Metric, Date | "IMF COFER, Q1 2026" |

---

## 6. Claim-Vs-Evidence Framework

Every entry must include a claim-vs-evidence table. It is the **core accountability mechanism** of the archive.

### Table Structure

| Column | Purpose |
|--------|---------|
| **Claim** | The assertion being evaluated |
| **Supported by Data?** | ✅ Yes / ⚠️ Partially / ❌ No |
| **Source Evidence** | Where to find the supporting evidence |
| **Qualifiers** | Limitations, caveats, or counter-arguments |

### Rating Definitions

| Rating | Meaning |
|--------|---------|
| ✅ Yes | The claim is directly supported by credible evidence |
| ⚠️ Partially | Some evidence supports the claim, but it has caveats or limitations |
| ❌ No | The claim is contradicted by available evidence |
| **Contextual** | The claim is true but requires historical/political context |

---

## 7. Cross-Reference Standards

### Cross-Reference Format

```markdown
| `EL-XXX-YYYY` (Description) | Connection |
```

### When to Cross-Reference

- The entry builds on another entry
- The entry provides evidence for another entry's claims
- The entry contradicts or complicates another entry's findings
- The entry is part of the same series

### Cross-Reference Maintenance

- Keep cross-references up to date when files are moved or renamed
- Do not reference files that do not yet exist (unless planned)
- Use the `planned` note for future entries: `EL-XXX-YYYY` (Planned)

---

## 8. Status & Versioning

### Status Definitions

| Status | Meaning |
|--------|---------|
| **DRAFT** | Work in progress; not yet ready for public viewing |
| **PUBLISH READY** | Complete; ready for publication |
| **ARCHIVED** | Superseded or no longer maintained |

### Versioning

| Version | Change |
|---------|--------|
| **1.0** | Initial publication |
| **1.1** | Minor edits & data refreshes |
| **2.0** | Significant revision or expansion |

---

## 9. Media Policy

**No media placeholders in entries.**

| Rule | Explanation |
|------|-------------|
| **No "Pending" visual asset lists** | They create an expectation of incompleteness |
| **Embed images only if you have them** | If the image exists, embed it inline |
| **No external link maintenance** | Links break; text does not |
| **Media is a separate project** | If you want to add media later, do it as a separate pass |

**Why**: Maintaining media links, sourcing images, and archiving content is time-consuming and diverts energy from the core work: analysis and writing.

---

## 10. Handoff Guidelines

### For the Next Agent

When handing off work to another agent or AI, include:

1. **Current status**: What's complete and what's in progress
2. **Priority queue**: What needs to be done next
3. **File locations**: Where to find active work
4. **Style reference**: Point to this document
5. **Open questions**: What's unresolved or pending

### Handoff Template

```markdown
## Handoff: [Date]

### Current Status
- [Series/Entry] — [Status]
- [Series/Entry] — [Status]

### Priority Queue
1. [Next task]
2. [Next task]
3. [Next task]

### File Locations
- [File path] — [Description]
- [File path] — [Description]

### Open Questions
- [Question]
- [Question]

### Notes for Next Agent
[Any additional context]
```

### Example Handoff

```markdown
## Handoff: 14 Jul 2026

### Current Status
- EL-FINANCE-01 (Bretton Woods) — PUBLISH READY
- EL-FINANCE-02 (Dollar Reserve) — PUBLISH READY
- EL-FINANCE-03 (BRICS Energy Axis) — PUBLISH READY

### Priority Queue
1. Create 03_finance/README.md linking the three entries
2. Begin EL-GEOPOLITICS-01 (Russia-China Axis)

### File Locations
- ANALYSIS/03_finance/EL-FINANCE-01.md
- ANALYSIS/03_finance/EL-FINANCE-02.md
- ANALYSIS/03_finance/EL-FINANCE-03.md

### Open Questions
- Whether to create a separate README for the finance series
- Priority of MIC vs. Russia-China series

### Notes for Next Agent
- No media placeholders in entries
- Follow the template in this document
- Cross-reference existing entries where relevant
```

---

## Appendix: Quick Reference Card

### Document Checklist

- [ ] Archive ID assigned
- [ ] Series identified
- [ ] Compiled Date set
- [ ] Version number assigned
- [ ] Status set (DRAFT / PUBLISH READY)
- [ ] Executive Summary complete
- [ ] All parts complete
- [ ] Claim-vs-Evidence table included
- [ ] Cross-references included
- [ ] Archive Metadata section complete
- [ ] Navigation links included
- [ ] No visual asset placeholders

### File Naming Quick Reference

| Element | Convention |
|---------|------------|
| Entry ID | `EL-{CATEGORY}-{NUMBER}` |
| File name | `EL-{CATEGORY}-{NUMBER}-topic.md` |
| Series folder | `{NUMBER}_{topic}/` |

---

**This document is a living standard. Update it when conventions change.**
