#  Multi-Dimensional Experiment Comparison Report

*Generated: 2026-08-04 08:36*

##  Dataset Overview

- **Total evaluations**: 144
- **Experiments**: 8 unique
- **Models**: gpt-5.4-nano
- **Schema modes**: small, ner, full, reasoning_path
- **Query types**: skipped, standard, error, count

- **Answer-overlap metric rows**: 93/144
- **Note**: answer-overlap is reported separately and does not change the legacy weighted overall score.

- **LLM evaluation decisions**: yes=1, no=97, other=46

## LLM Evaluation Decisions by Experiment

*Normalized values are shown as rates in [0, 1]. `yes_rate_decided` uses only decided rows (`yes` + `no`).*

| Experiment | Yes | No | Other | yes_rate_total | no_rate_total | yes_rate_decided |
|------------|-----|----|-------|----------------|---------------|------------------|
| ca_ic | 1 | 12 | 5 | 0.056 | 0.667 | 0.077 |
| c01 | 0 | 6 | 12 | 0.000 | 0.333 | 0.000 |
| ca_ia | 0 | 11 | 7 | 0.000 | 0.611 | 0.000 |
| ca_ia_ic | 0 | 12 | 6 | 0.000 | 0.667 | 0.000 |
| ca | 0 | 13 | 5 | 0.000 | 0.722 | 0.000 |
| c02_ia | 0 | 14 | 4 | 0.000 | 0.778 | 0.000 |
| ca_ib | 0 | 14 | 4 | 0.000 | 0.778 | 0.000 |
| ca_cb_ia_ic | 0 | 15 | 3 | 0.000 | 0.833 | 0.000 |

## 🏆 Overall Rankings (Weighted Multi-Metric Score)

| Rank | Experiment | Score | Samples |
|------|------------|-------|---------|
| 1 | ca_ic | 0.470 | 18 |
| 2 | ca_ib | 0.457 | 18 |
| 3 | ca_cb_ia_ic | 0.452 | 18 |
| 4 | ca_ia_ic | 0.447 | 18 |
| 5 | ca | 0.435 | 18 |
| 6 | ca_ia | 0.430 | 18 |
| 7 | c02_ia | 0.394 | 18 |
| 8 | c01 | 0.353 | 18 |

## Rankings by SYNTAX Dimension

*Higher score = better performance on syntax metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ib | 0.926 |
| 2 | ca_ic | 0.833 |
| 3 | ca_cb_ia_ic | 0.815 |
| 3 | ca | 0.815 |
| 5 | ca_ia_ic | 0.815 |

## Rankings by STRUCTURE Dimension

*Higher score = better performance on structure metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca | 0.619 |
| 2 | c01 | 0.609 |
| 3 | ca_ia | 0.592 |
| 4 | ca_ib | 0.525 |
| 5 | ca_cb_ia_ic | 0.504 |

## Rankings by RESULTS Dimension

*Higher score = better performance on results metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia_ic | 0.091 |
| 2 | ca | 0.083 |
| 5 | c02_ia | 0.000 |
| 5 | c01 | 0.000 |
| 5 | ca_cb_ia_ic | 0.000 |

## Rankings by ANSWER_OVERLAP Dimension

*Higher score = better performance on answer_overlap metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia_ic | 0.273 |
| 2 | ca_ic | 0.264 |
| 3 | ca | 0.167 |
| 4 | ca_ib | 0.154 |
| 5 | ca_ia | 0.100 |

## Rankings by EFFICIENCY Dimension

*Higher score = better performance on efficiency metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ic | 0.721 |
| 2 | ca_ib | 0.673 |
| 3 | ca_ia_ic | 0.669 |
| 4 | ca_ia | 0.649 |
| 5 | c01 | 0.602 |

## 🔬 Statistical Significance Testing

 Found 6 metrics with significant differences across experiments (p < 0.05)

- **Grammar Validity** (syntax): p=0.0037, η²=0.157
  → Best: `ca_ib` (1.000)

- **Preparation Validity** (syntax): p=0.0054, η²=0.150
  → Best: `ca_ib` (1.000)

## Recommendations by Use Case

### Highest Result Accuracy (Standard Queries)

**Winner**: `ca_ia_ic`

- Expected F1: ~0.091

### Highest Answer Overlap Accuracy (Standard Queries)

**Winner**: `ca_ia_ic`

- Expected answer-overlap F1: ~0.273

- This metric compares shared answer variables when result tables have different columns.

### Fastest Execution

**Winner**: `ca_ic`

- Avg time: ~4.32s

###  Most Syntactically Valid Queries

**Winner**: `ca_ib`

- Grammar validity: 100.0%

### Best Balanced Configuration

**Recommended**: `ca_ic`

- Good tradeoff across validity, similarity, correctness, and efficiency
