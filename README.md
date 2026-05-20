# Supplementary Materials for the Agent-Readable Advertising Survey

Created: 2026-05-14

This repository contains the supplementary materials for the manuscript on agent-readable representations of legacy display advertising.
It is intended to support reviewer and reader inspection of the survey registry, public coding summaries and traceability tables, corpus-construction trace, standards/protocol crosswalks, AARS schema, and benchmark template.

## Contents

| Supplement item | Files |
|---|---|
| S1 registry and related surveys | 4 CSV files |
| S2 core coding summaries and traceability tables | 6 CSV files, 2 Markdown files |
| S3 background role mapping | 2 CSV files |
| S4 out-of-scope exclusions | 1 CSV file |
| S5 search/screening trace | 1 CSV file, 1 Mermaid corpus-construction flow, 1 Markdown trace |
| S6 C7 ad-tech standards | 1 CSV file |
| S7 C8 agentic protocols | 1 CSV file |
| S8 AARS reference schema | 1 JSON schema, 1 synthetic example Markdown file |
| S9 G5 benchmark task template | 1 Markdown template |

## Boundary

- This package uses only previously verified local project sources.
- The 149-paper research-corpus registry is provided as `S1_registry_related_surveys/S1_research_corpus_registry_149_english.csv`, derived from the S2 core, S3 background, and S4 out-of-scope tables.
- No new literature, standard, venue, DOI, author list, or current web update was added during assembly.
- S5 is a corpus-construction trace for a structured systematic mapping; unavailable database-hit and screening counts are not inferred.
- S2 includes public paper-level coding summaries, coding responsibility and completion records, row-level coder responsibility fields, high-risk coding-field definitions, a claim-to-citation traceability matrix for the main corpus-bounded negative claims, and descriptive targeted-verification tables for selected high-risk records. These materials derive from the internal coding process and record distributed literature identification/coding by cluster or subset, claim traceability, and label-visible targeted verification; they are not presented as an exhaustive row-level dump of every internal coding field and do not claim independent double coding, inter-rater reliability, Cohen's kappa, Jaccard agreement, agreement rates, independent audit, non-core validation, or adjudicated reliability statistics.
- AARS is a survey-derived reference schema, not an industry standard.
- S8 is synthetic and is not empirical evidence.
- S9 is a survey agenda template and is not executed experimental data.

## Exclusions

- This repository does not include copyrighted paper PDFs.
- This repository does not include manuscript source files.
- This repository does not claim that the corpus-construction trace is a complete formal review flow diagram.
