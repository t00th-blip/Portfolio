# Power Hour: Making Minutes Count — Evaluation Design

A complete evaluation design for Boys & Girls Clubs of the Valley's Power Hour program:
theory of change, logic model, monitoring and evaluation plan, quasi-experimental outcome
design, analysis plan, reporting plan, and budget.

Arizona State University, PAF 541: Program Evaluation (Dr. Eileen Eisen-Cohen), June 2026.

> **This is a design, not an analysis.** No data was collected and no findings are reported.
> It is also an academic exercise — it was not commissioned by Boys & Girls Clubs of the Valley,
> and the program description is built from the organization's public materials.

It's in the portfolio because designing a defensible evaluation is a distinct skill from running
one, and this is the artifact that shows it end to end: what to measure, how to know whether the
program was even delivered, what the design can and cannot claim, and what it costs.

## The program and the problem

Power Hour runs across 27 BGCAZ sites in the Phoenix metro area, serving youth ages 6 to 18 with
structured daily homework time, adult tutoring, STEAM enrichment, and summer programming. The
underlying premise is that unequal access to academic support outside school hours drives the
achievement gap, and that summer learning loss hits low-income students hardest.

## Evaluation questions

1. To what extent does Power Hour improve homework completion among participants?
2. Do participants show improved academic performance over time?
3. Do participants experience less summer learning loss than comparable non-participants?
4. Do outcomes vary by age, grade level, or length of enrollment?
5. Is Power Hour being implemented consistently across all 27 sites?

Questions 1–4 are outcome questions; question 5 is implementation. Both are in scope on purpose:
outcome data from 27 sites is hard to interpret if the sites aren't running the same program.

## Design

| | |
|---|---|
| Outcome design | Quasi-experimental pre-post; participants assessed at enrollment, 60 days, and 90 days |
| Comparison | Matched non-participants, matched on school, grade level, and baseline academic performance |
| Summer component | Difference-in-differences against non-participants from the same schools, to separate program effect from general seasonal trend |
| Analysis | Descriptive statistics; paired t-tests for pre-post; difference-in-differences for summer outcomes; subgroup analysis by age, grade, and enrollment duration |
| Implementation | Quarterly fidelity checklists; % of sites meeting BGCA standards |

### What the design can't claim

Selection bias is the binding limitation: families who enroll may already differ from
non-participants in unmeasured ways that also predict better outcomes. Matching reduces that and
does not eliminate it, so findings are framed as associative, not causal. Secondary limits are
data quality in staff-maintained homework logs, which varies by site, and site-level
implementation differences that make cross-site outcome comparison imperfect.

Stating this in the design rather than discovering it in the discussion section is the point.

## Monitoring and evaluation plan

Eight tracked measures across seven program activities, each with an indicator, data source,
collection frequency, and reporting frequency — from daily session logs through quarterly site
fidelity checks. See `evaluation_plan.md`.

## Equity and ethics in the design

Many participating families are Latino and many are English language learners, so every survey,
consent form, and reporting product is produced in English and Spanish, with bilingual staff or
community reviewers checking cultural appropriateness rather than just translation accuracy.

Because the program serves immigrant families, the consent process states plainly that data
collection is unrelated to immigration enforcement and will not affect access to services.
Participation is voluntary and services are not conditioned on it.

The evaluation involves minors, so parental consent and youth assent are both required. Data is
reported only in aggregate. Where findings show disparities — weaker outcomes for older students
or late enrollees — the design commits to reporting them rather than omitting them.

## Reporting plan

Five products for five audiences: an interim implementation report for site staff, a full
technical report for leadership and funders, an executive summary, a one-page bilingual
community summary in plain language for families, and a staff presentation with actionable
recommendations.

## Budget

$13,200 in staffing across 280 hours — lead evaluator, research analyst, evaluation assistant,
and community liaison / cultural consultant.

## What's in this repo

| File | What it is |
|---|---|
| `evaluation_design.pdf` | The full design document |
| `logic_model.md` | Inputs, activities, outputs, short- and long-term outcomes |
| `theory_of_change.md` | Problem, contributing factors, program response, expected change |
| `me_plan.csv` | M&E plan: activity, measure, indicator, source, frequencies |
| `budget.csv` | Staffing budget |

## Status

Design complete; never fielded. Course assignment, June 2026.
