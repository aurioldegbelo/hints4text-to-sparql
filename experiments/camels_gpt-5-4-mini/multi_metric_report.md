#  Multi-Dimensional Experiment Comparison Report

*Generated: 2026-08-04 02:38*

##  Dataset Overview

- **Total evaluations**: 144
- **Experiments**: 8 unique
- **Models**: gpt-5.4-mini
- **Schema modes**: reasoning_path, full, small, ner
- **Query types**: error, standard, count, skipped

- **Answer-overlap metric rows**: 101/144
- **Note**: answer-overlap is reported separately and does not change the legacy weighted overall score.

- **LLM evaluation decisions**: yes=5, no=103, other=36

## LLM Evaluation Decisions by Experiment

*Normalized values are shown as rates in [0, 1]. `yes_rate_decided` uses only decided rows (`yes` + `no`).*

| Experiment | Yes | No | Other | yes_rate_total | no_rate_total | yes_rate_decided |
|------------|-----|----|-------|----------------|---------------|------------------|
| ca_cb_ia_ic | 2 | 12 | 4 | 0.111 | 0.667 | 0.143 |
| ca_ic | 1 | 13 | 4 | 0.056 | 0.722 | 0.071 |
| ca_ia_ic | 1 | 14 | 3 | 0.056 | 0.778 | 0.067 |
| ca_ib | 1 | 15 | 2 | 0.056 | 0.833 | 0.062 |
| ca | 0 | 10 | 8 | 0.000 | 0.556 | 0.000 |
| ca_ia | 0 | 11 | 7 | 0.000 | 0.611 | 0.000 |
| c01 | 0 | 13 | 5 | 0.000 | 0.722 | 0.000 |
| c02_ia | 0 | 15 | 3 | 0.000 | 0.833 | 0.000 |

## 🏆 Overall Rankings (Weighted Multi-Metric Score)

| Rank | Experiment | Score | Samples |
|------|------------|-------|---------|
| 1 | ca_cb_ia_ic | 0.523 | 18 |
| 2 | ca_ic | 0.473 | 18 |
| 3 | ca_ib | 0.468 | 18 |
| 4 | ca_ia_ic | 0.464 | 18 |
| 5 | c01 | 0.443 | 18 |
| 6 | ca_ia | 0.435 | 18 |
| 7 | c02_ia | 0.417 | 18 |
| 8 | ca | 0.395 | 18 |

## Rankings by SYNTAX Dimension

*Higher score = better performance on syntax metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ib | 0.944 |
| 2 | ca_ia_ic | 0.907 |
| 3 | c02_ia | 0.870 |
| 3 | ca_cb_ia_ic | 0.870 |
| 5 | ca_ic | 0.852 |

## Rankings by STRUCTURE Dimension

*Higher score = better performance on structure metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia | 0.630 |
| 2 | c02_ia | 0.613 |
| 3 | ca_cb_ia_ic | 0.605 |
| 4 | ca_ia_ic | 0.604 |
| 5 | c01 | 0.581 |

## Rankings by RESULTS Dimension

*Higher score = better performance on results metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ic | 0.154 |
| 2 | ca_cb_ia_ic | 0.077 |
| 3 | ca_ia_ic | 0.071 |
| 4 | ca_ib | 0.067 |
| 6 | ca | 0.000 |

## Rankings by ANSWER_OVERLAP Dimension

*Higher score = better performance on answer_overlap metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.359 |
| 2 | ca_ic | 0.231 |
| 3 | ca_ia | 0.200 |
| 4 | ca_ib | 0.178 |
| 5 | ca_ia_ic | 0.143 |

## Rankings by EFFICIENCY Dimension

*Higher score = better performance on efficiency metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.672 |
| 2 | ca_ia_ic | 0.644 |
| 3 | c01 | 0.615 |
| 4 | ca_ia | 0.609 |
| 5 | ca_ib | 0.603 |

## 🔬 Statistical Significance Testing

 Found 1 metrics with significant differences across experiments (p < 0.05)

- **Execution Time** (efficiency): p=0.0158, η²=0.164
  → Best: `ca_ia` (2.180)

## Recommendations by Use Case

### Highest Result Accuracy (Standard Queries)

**Winner**: `ca_ic`

- Expected F1: ~0.154

### Highest Answer Overlap Accuracy (Standard Queries)

**Winner**: `ca_cb_ia_ic`

- Expected answer-overlap F1: ~0.359

- This metric compares shared answer variables when result tables have different columns.

### Fastest Execution

**Winner**: `ca_cb_ia_ic`

- Avg time: ~1.95s

###  Most Syntactically Valid Queries

**Winner**: `ca_ib`

- Grammar validity: 100.0%

### Best Balanced Configuration

**Recommended**: `ca_cb_ia_ic`

- Good tradeoff across validity, similarity, correctness, and efficiency
