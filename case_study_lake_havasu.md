# Police Staffing in a Tourist Economy

**A workload-based patrol staffing model for Lake Havasu City**

Public Affairs capstone, Arizona State University, PAF 509 (Instructor: Cynthia Seelhammer).
Client contact and second reader: Lt. Michael Terrinoni, Lake Havasu City Police Department.

## The problem

LHCPD sets patrol staffing using ratio-based reasoning against a resident population of about
62,400 — in a city the department estimates receives roughly 1.6 million annual visitors. Calls
for service reached 50,493 in 2025, up from about 47,300 in 2024.

A resident-only ratio cannot see demand that arrives with visitors, and it cannot see *when* in
the year that demand lands. Current staffing appears to rest on assumptions that predate the
city's growth.

## Role

Primary evaluator for the client: literature review, data acquisition, extraction pipeline,
analysis, and the client-facing deliverable.

## Methods

| | |
|---|---|
| Design | Quantitative comparative case study |
| Data | 44 monthly calls-for-service files, January 2023 – August 2026, obtained through a public records request |
| Record fields | Call ID, timestamp, priority level, call nature |
| Engineering | R pipeline converting 44 monthly PDFs into one analysis-ready dataset |
| Workload measure | Calls for service, aggregated monthly for seasonal pattern and broken out by priority to separate time-sensitive from low-priority activity |
| Proxy | Because month-by-month visitor counts don't exist, monthly call volume also stands in for effective service population — which lets the analysis test whether demand tracks visitor patterns more closely than resident population |
| Benchmarking | Peer municipalities with comparable seasonal swings, on staffing ratios, workload distribution, and allocation |
| Tools | R, SQL |
| Evidence base | 13-source review spanning criminology, operations research, economics, and tourism management, plus DOJ COPS Office guidance |

### Alternatives considered

A pure per-capita ratio is the baseline being evaluated, and the literature finds it a poor fit
where non-resident populations are large. A full queueing or simulation model fits large seasonal
swings better but was too data- and time-intensive for this scope. A purely qualitative approach
built on leadership interviews would not have produced the defensible recommendation the client
asked for.

## What the literature does and doesn't settle

- **Ratios are weak, but there's no consensus replacement.** The field agrees static
  officer-per-resident ratios are a poor basis for staffing; it splits on what replaces them —
  an adjustable formula versus queueing models matched to call volume. The formula is easier to
  explain to a department; queueing handles seasonality better.
- **More officers is not automatically the answer.** The workforce-size-to-outcome link is
  context-dependent, with evidence of diminishing returns past an optimal amount of patrol. The
  operative variable is deployment against demand, not headcount.
- **Tourism strains small cities, but the evidence is indirect.** The supporting studies come
  from Spain, Tobago, and local U.S. reporting, so they establish that the mismatch exists
  without showing how it resolves in a U.S. lake town.
- **Small departments struggle with data.** Inconsistent record systems and limited analytic
  capacity are documented norms — which is exactly why this project's call records arrived as 44
  PDFs.

The gap: workload methods are well developed but largely untested in small, tourism-heavy U.S.
departments.

## What's in this repo

| File | What it is |
|---|---|
| `pipeline/extract_pdfs.R` | PDF-to-dataset extraction and validation pipeline |
| `pipeline/README.md` | How extraction works and how it was validated |
| `sql/schema.sql` | <!-- FILL: SQLite schema once the load is built --> |
| `sql/*.sql` | <!-- FILL: cleaning and monthly/priority summary queries --> |
| `analysis/seasonality.R` | Monthly demand and seasonal structure |
| `analysis/benchmarking.R` | Peer-city comparison from public sources |
| `figures/` | Demand by month, by priority, and by call nature |

## What is deliberately not in this repo

The client report and its staffing recommendations. The report is a deliverable for the
department and a graded submission; recommendations reach the client before they reach anywhere
public.

The call records came through a public records request and are therefore disclosable, but what
gets posted here is cleared with the department and the course instructor first.

## Findings

<!-- FILL after analysis. Three bullets, each with a number:
     - size and timing of the seasonal peak
     - where LHCPD sits against peer cities on officers per 1,000
     - what the workload method implies for staffing vs. what the ratio method implies -->

## Status

In progress, Fall 2026. Literature review complete; extraction pipeline built; analysis and
client report underway.
