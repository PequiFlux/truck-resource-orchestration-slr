# Review Audit Trail

## Search Sources

- IEEE Xplore
- Web of Science
- Scopus
- backward snowballing via Zotero

## Search Date

- February 27, 2026 for the database searches
- same review cycle for backward snowballing

## Core Boolean Query Preserved

```text
("agribusiness logistics" OR "cross-docking" OR "dock doors" OR "gates" OR "terminal logistics" OR "truck appointment system" OR "truck arrivals" OR "yard management" OR "yard trucks")
AND
("dynamic scheduling" OR "heuristic" OR "machine learning" OR "optimization" OR "predictive-reactive scheduling" OR "real-time scheduling" OR "reinforcement learning" OR "resource allocation" OR "simulation")
AND
("bottleneck reduction" OR "congestion reduction" OR "delay reduction" OR "dock utilization improvement" OR "makespan reduction" OR "operational cost reduction" OR "queue reduction" OR "waiting time reduction")
```

## Exact Scopus Query Preserved

```text
TITLE-ABS-KEY ( ( "truck scheduling" OR "truck appointment system" OR "yard management" OR "terminal logistics" OR "agribusiness logistics" ) AND ( queue* OR "resource allocation" OR bottleneck OR dock* ) AND ( optimiz* OR heuristic* OR "reinforcement learning" OR "machine learning" OR simulation ) AND ( "real-time" OR dynamic OR uncertain* ) ) AND PUBYEAR > 2020 AND PUBYEAR < 2027
```

Result preserved from the review log:

- 22 documents found in Scopus

## Exact IEEE Xplore Query Preserved

```text
( "truck scheduling" OR "truck appointment system" OR "yard management" OR "terminal logistics" OR "agribusiness logistics" ) AND ( queue* OR "resource allocation" OR bottleneck OR dock* ) AND ( optimiz* OR heuristic* OR "reinforcement learning" OR "machine learning" OR simulation ) AND ( "real-time" OR dynamic OR uncertain* )
```

Result preserved from the review log:

- IEEE Xplore showed 13 results for this query
- the preserved Parsifal import snapshot still lists 12 IEEE records

## Source-Level Execution Details Preserved

| Source | Execution date | Recoverable retrieval scope | Filters applied | Preserved count |
| --- | --- | --- | --- | --- |
| IEEE Xplore | February 27, 2026 | Exact advanced-search syntax preserved for this source; direct Boolean query with no year filter | No temporal filter | 13 results shown retrospectively; 12 imported records preserved in the archived snapshot |
| Web of Science | February 27, 2026 | Common Boolean query aligned with title/abstract/keyword retrieval; exact interface field tags not preserved | Publication year 2021-2026 | 20 imported records |
| Scopus | February 27, 2026 | Exact advanced-search syntax preserved for this source; `TITLE-ABS-KEY` query plus explicit year filter | Publication year 2021-2026 | 22 documents found and imported |
| Backward snowballing via Zotero | Same review cycle after database screening | Reference-list inspection rather than database-field syntax | Same inclusion and exclusion rules as the database search | 8 additional records |

## PRISMA Flow Preserved in the Current Package

- database-search records: 60
- duplicates removed: 18
- records after deduplication: 42
- records excluded for inaccessible full text: 13
- records added by snowballing: 8
- studies entering quality assessment: 37
- studies excluded with score `<= 7.5`: 3
- final retained corpus: 34

## Preservation Status

- Preserved: core Boolean query, exact IEEE Xplore query, exact Scopus query, source list, search date, source-level imported counts, retained-corpus list, and extraction spreadsheet.
- Preserved only in aggregate: deduplication result and count of inaccessible full-text exclusions.
- Partially preserved: database-specific field tags as typed in each interface, because the exact IEEE Xplore and Scopus syntax is archived but the Web of Science string is not.
- Not preserved: duplicate-pair log, definitive article-level list of the 13 inaccessible full-text records, and item-level quality scores.

## Full Extraction Sheet

- `../../data_extraction.xls`

## Journal-Grade Gap That Still Remains

The current package is now explicit about what is auditable and what is not. It still does not support a retrospective threshold-sensitivity analysis or a definitive appendix for the 13 inaccessible full-text records. Those two artifacts depend on recovering the original Parsifal screening workspace.
