#  Multi-Dimensional Experiment Comparison Report

*Generated: 2026-08-04 04:19*

##  Dataset Overview

- **Total evaluations**: 144
- **Experiments**: 8 unique
- **Models**: gpt-5.4-mini
- **Schema modes**: reasoning_path, full, small, ner
- **Query types**: error, standard, mismatch, count, skipped

- **Answer-overlap metric rows**: 84/144
- **Note**: answer-overlap is reported separately and does not change the legacy weighted overall score.

- **LLM evaluation decisions**: yes=7, no=82, other=55

## LLM Evaluation Decisions by Experiment

*Normalized values are shown as rates in [0, 1]. `yes_rate_decided` uses only decided rows (`yes` + `no`).*

| Experiment | Yes | No | Other | yes_rate_total | no_rate_total | yes_rate_decided |
|------------|-----|----|-------|----------------|---------------|------------------|
| ca_cb_ia_ic | 2 | 7 | 9 | 0.111 | 0.389 | 0.222 |
| c01 | 2 | 11 | 5 | 0.111 | 0.611 | 0.154 |
| ca_ia_ic | 2 | 12 | 4 | 0.111 | 0.667 | 0.143 |
| ca | 1 | 6 | 11 | 0.056 | 0.333 | 0.143 |
| ca_ia | 0 | 10 | 8 | 0.000 | 0.556 | 0.000 |
| c02_ia | 0 | 11 | 7 | 0.000 | 0.611 | 0.000 |
| ca_ib | 0 | 12 | 6 | 0.000 | 0.667 | 0.000 |
| ca_ic | 0 | 13 | 5 | 0.000 | 0.722 | 0.000 |

## 🏆 Overall Rankings (Weighted Multi-Metric Score)

| Rank | Experiment | Score | Samples |
|------|------------|-------|---------|
| 1 | ca_ia_ic | 0.563 | 18 |
| 2 | ca_cb_ia_ic | 0.559 | 18 |
| 3 | ca_ic | 0.476 | 18 |
| 4 | c01 | 0.466 | 18 |
| 5 | ca_ib | 0.454 | 18 |
| 6 | ca_ia | 0.443 | 18 |
| 7 | ca | 0.437 | 18 |
| 8 | c02_ia | 0.433 | 18 |

## Rankings by SYNTAX Dimension

*Higher score = better performance on syntax metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia_ic | 0.907 |
| 3 | c01 | 0.889 |
| 3 | ca_ib | 0.889 |
| 3 | ca_ic | 0.889 |
| 5 | ca_ia | 0.796 |

## Rankings by STRUCTURE Dimension

*Higher score = better performance on structure metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.702 |
| 2 | c02_ia | 0.673 |
| 3 | ca_ic | 0.583 |
| 4 | ca_ia_ic | 0.582 |
| 5 | ca_ib | 0.572 |

## Rankings by RESULTS Dimension

*Higher score = better performance on results metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia_ic | 0.231 |
| 2 | ca_cb_ia_ic | 0.222 |
| 3 | c01 | 0.182 |
| 4 | ca | 0.143 |
| 5 | ca_ic | 0.139 |

## Rankings by ANSWER_OVERLAP Dimension

*Higher score = better performance on answer_overlap metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.362 |
| 2 | ca_ia_ic | 0.231 |
| 3 | c01 | 0.182 |
| 4 | ca_ic | 0.167 |
| 5 | ca | 0.143 |

## Rankings by EFFICIENCY Dimension

*Higher score = better performance on efficiency metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia_ic | 0.913 |
| 2 | c02_ia | 0.627 |
| 3 | ca_ia | 0.615 |
| 4 | ca_ib | 0.601 |
| 5 | ca_ic | 0.599 |

## 🔬 Statistical Significance Testing

 No metrics showed statistically significant differences across experiments at α=0.05 (after multiple comparison correction)

## Recommendations by Use Case

### Highest Result Accuracy (Standard Queries)

**Winner**: `ca_ia_ic`

- Expected F1: ~0.231

### Highest Answer Overlap Accuracy (Standard Queries)

**Winner**: `ca_cb_ia_ic`

- Expected answer-overlap F1: ~0.340

- This metric compares shared answer variables when result tables have different columns.

### Fastest Execution

**Winner**: `ca_ia_ic`

- Avg time: ~2.78s

###  Most Syntactically Valid Queries

**Winner**: `ca_ia_ic`

- Grammar validity: 100.0%

### Best Balanced Configuration

**Recommended**: `ca_ia_ic`

- Good tradeoff across validity, similarity, correctness, and efficiency
