#  Multi-Dimensional Experiment Comparison Report

*Generated: 2026-08-04 08:37*

##  Dataset Overview

- **Total evaluations**: 126
- **Experiments**: 7 unique
- **Models**: gpt-4.1
- **Schema modes**: small, ner, full, reasoning_path
- **Query types**: standard, skipped, error, count

- **Answer-overlap metric rows**: 93/126
- **Note**: answer-overlap is reported separately and does not change the legacy weighted overall score.

- **LLM evaluation decisions**: yes=4, no=96, other=26

## LLM Evaluation Decisions by Experiment

*Normalized values are shown as rates in [0, 1]. `yes_rate_decided` uses only decided rows (`yes` + `no`).*

| Experiment | Yes | No | Other | yes_rate_total | no_rate_total | yes_rate_decided |
|------------|-----|----|-------|----------------|---------------|------------------|
| ca_cb_ia_ic | 2 | 12 | 4 | 0.111 | 0.667 | 0.143 |
| ca_ia | 1 | 11 | 6 | 0.056 | 0.611 | 0.083 |
| ca_ib | 1 | 14 | 3 | 0.056 | 0.778 | 0.067 |
| ca_ia_ic | 0 | 14 | 4 | 0.000 | 0.778 | 0.000 |
| c01 | 0 | 15 | 3 | 0.000 | 0.833 | 0.000 |
| c02_ia | 0 | 15 | 3 | 0.000 | 0.833 | 0.000 |
| ca_ic | 0 | 15 | 3 | 0.000 | 0.833 | 0.000 |

## 🏆 Overall Rankings (Weighted Multi-Metric Score)

| Rank | Experiment | Score | Samples |
|------|------------|-------|---------|
| 1 | ca_ia | 0.498 | 18 |
| 2 | ca_ia_ic | 0.494 | 18 |
| 3 | ca_cb_ia_ic | 0.492 | 18 |
| 4 | ca_ib | 0.479 | 18 |
| 5 | ca_ic | 0.472 | 18 |
| 6 | c01 | 0.471 | 18 |
| 7 | c02_ia | 0.455 | 18 |

## Rankings by SYNTAX Dimension

*Higher score = better performance on syntax metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ic | 0.889 |
| 1 | ca_ib | 0.889 |
| 3 | c01 | 0.870 |
| 3 | c02_ia | 0.870 |
| 5 | ca_ia_ic | 0.852 |

## Rankings by STRUCTURE Dimension

*Higher score = better performance on structure metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ib | 0.614 |
| 2 | c01 | 0.605 |
| 3 | c02_ia | 0.601 |
| 4 | ca_ia_ic | 0.593 |
| 5 | ca_cb_ia_ic | 0.565 |

## Rankings by RESULTS Dimension

*Higher score = better performance on results metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.154 |
| 2 | ca_ia | 0.091 |
| 3 | ca_ia_ic | 0.077 |
| 4 | ca_ib | 0.071 |
| 4 | ca_ic | 0.071 |

## Rankings by ANSWER_OVERLAP Dimension

*Higher score = better performance on answer_overlap metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.359 |
| 2 | ca_ia | 0.325 |
| 3 | ca_ib | 0.204 |
| 4 | ca_ia_ic | 0.154 |
| 5 | ca_ic | 0.143 |

## Rankings by EFFICIENCY Dimension

*Higher score = better performance on efficiency metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ib | 0.718 |
| 2 | ca_ia_ic | 0.691 |
| 3 | c01 | 0.677 |
| 4 | ca_ia | 0.664 |
| 5 | c02_ia | 0.634 |

## 🔬 Statistical Significance Testing

 No metrics showed statistically significant differences across experiments at α=0.05 (after multiple comparison correction)

## Recommendations by Use Case

### Highest Result Accuracy (Standard Queries)

**Winner**: `ca_cb_ia_ic`

- Expected F1: ~0.154

### Highest Answer Overlap Accuracy (Standard Queries)

**Winner**: `ca_cb_ia_ic`

- Expected answer-overlap F1: ~0.359

- This metric compares shared answer variables when result tables have different columns.

### Fastest Execution

**Winner**: `ca_ib`

- Avg time: ~3.55s

###  Most Syntactically Valid Queries

**Winner**: `ca_ic`

- Grammar validity: 100.0%

### Best Balanced Configuration

**Recommended**: `ca_ia`

- Good tradeoff across validity, similarity, correctness, and efficiency
