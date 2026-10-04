# Designing for Trust

**A Community-Centered Approach to Aging in Place Among Immigrant Elders in Faith-Based and Public Civic Spaces**

Graduate Research Fellowship, AmeriCorps / Arizona State University, 2025.

## The question

Why do churches function as more trusted civic spaces for immigrant elders than public
libraries or recreation centers, and what emotional, informational, or social barriers prevent
engagement with formal resources?

The premise is simple and easy to miss: people do not access what they do not know exists, and
age, isolation, and language barriers each make that worse. So the study treated awareness as a
measurable condition rather than an assumption.

## Role

Sole evaluator. I built the logic model, the evaluation plan, the IRB protocol, and every
instrument in both English and Spanish; recruited participants; collected all the data; ran the
analysis; and wrote the deliverable.

## Methods

| | |
|---|---|
| Design | Mixed-methods needs and access-barriers evaluation |
| Sample | 26 surveys, 16 semi-structured interviews |
| Population | Older immigrant men of color, age 55+, in Arizona |
| Instruments | Survey, interview guide, and consent forms developed in English and Spanish; administered in the participant's preferred language |
| Quantitative | Descriptive and correlation analysis in R |
| Qualitative | Thematic coding of interview transcripts |
| Participatory component | Neighborhood mapping activity (see below) |
| Approvals | IRB-approved; IRB Human Subjects Research certification held |

### The mapping activity

Rather than asking participants to rate a list of facilities I had written, I gave them a map of
their own neighborhood and asked them to mark three things: places they go often, places they
avoid, and places they wish they could go but do not. Each mark opened a conversation about why.
Participants who preferred not to talk could use simple marks instead. The design intent was to
let the categories come from participants rather than from me — a place I had not thought to ask
about could still show up on the map.

### Interview focus

The guide worked outward from comfort rather than inward from institutions: where do you feel
comfortable asking for help, and what makes it feel that way; where did you actually go the last
time you needed housing, food, or paperwork help; what makes libraries and recreation centers
hard to walk into; what would change that. One question asked directly whether a familiar face
from their church working at a library would make a difference.

## Findings

- Four barriers were operative: **awareness, language, privacy, and trust**.
- <!-- FILL: one sentence per barrier, with the supporting number or the theme it came from -->
- <!-- FILL: what libraries and rec centers were actually doing wrong, in participants' terms -->

<!-- FILL: the brief's headline recommendation, one sentence -->

## Deliverables

Policy brief with outreach and facility-design recommendations for municipal libraries and
recreation centers, presented to the ASU Watts College board and reported to AmeriCorps and
community partners. The brief was selected for publication in an edited volume.

## What's in this repo

| File | What it is |
|---|---|
| `design/proposal.pdf` | Study proposal: question, rationale, methods |
| `design/logic_model.pdf` | Logic model |
| `design/evaluation_plan.md` | Evaluation plan |
| `instruments/survey_en.pdf`, `survey_es.pdf` | Survey instrument, both languages |
| `instruments/interview_guide_en.md`, `_es.md` | Semi-structured interview guides |
| `instruments/consent_en.pdf`, `consent_es.pdf` | Informed consent forms, both languages |
| `instruments/mapping_activity.md` | Mapping activity protocol and instructions |
| `analysis/codebook.md` | Qualitative coding scheme |
| `analysis/*.R` | Analysis scripts, run against synthetic data (see below) |
| `data/synthetic_responses.csv` | Synthetic dataset matching the real column structure |

## What is deliberately not in this repo

No survey responses, interview transcripts, audio, field notes, completed maps, or attributed
participant quotes. With 26 surveys and 16 interviews drawn from one community, a narrow age
band, and a named set of neighborhood facilities, those records are re-identifiable even with
names removed. The analysis scripts here run against a synthetic dataset matching the real one's
structure, so the code is reviewable without exposing participants.

This follows the IRB protocol under which the study was approved. It is not a stylistic choice.

## Status

Complete. Brief selected for publication in an edited volume.

<!-- FILL: link the brief once you confirm the publisher permits self-archiving. Many allow the
     accepted version but not the published PDF. Check the agreement before posting it. -->
