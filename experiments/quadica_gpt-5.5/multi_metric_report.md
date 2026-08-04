#  Multi-Dimensional Experiment Comparison Report

*Generated: 2026-08-04 08:44*

##  Dataset Overview

- **Total evaluations**: 144
- **Experiments**: 8 unique
- **Models**: gpt-5.5
- **Schema modes**: small, ner, full, reasoning_path
- **Query types**: standard, error, count

- **Answer-overlap metric rows**: 123/144
- **Note**: answer-overlap is reported separately and does not change the legacy weighted overall score.

- **LLM evaluation decisions**: yes=7, no=123, other=14

## LLM Evaluation Decisions by Experiment

*Normalized values are shown as rates in [0, 1]. `yes_rate_decided` uses only decided rows (`yes` + `no`).*

| Experiment | Yes | No | Other | yes_rate_total | no_rate_total | yes_rate_decided |
|------------|-----|----|-------|----------------|---------------|------------------|
| ca_ic | 2 | 14 | 2 | 0.111 | 0.778 | 0.125 |
| ca_cb_ia_ic | 2 | 15 | 1 | 0.111 | 0.833 | 0.118 |
| ca_ia_ic | 2 | 15 | 1 | 0.111 | 0.833 | 0.118 |
| ca_ia | 1 | 16 | 1 | 0.056 | 0.889 | 0.059 |
| c01 | 0 | 13 | 5 | 0.000 | 0.722 | 0.000 |
| ca | 0 | 16 | 2 | 0.000 | 0.889 | 0.000 |
| ca_ib | 0 | 16 | 2 | 0.000 | 0.889 | 0.000 |
| c02_ia | 0 | 18 | 0 | 0.000 | 1.000 | 0.000 |

## 🏆 Overall Rankings (Weighted Multi-Metric Score)

| Rank | Experiment | Score | Samples |
|------|------------|-------|---------|
| 1 | ca_cb_ia_ic | 0.636 | 18 |
| 2 | ca_ia_ic | 0.585 | 18 |
| 3 | ca | 0.582 | 18 |
| 4 | ca_ia | 0.569 | 18 |
| 5 | ca_ic | 0.557 | 18 |
| 6 | ca_ib | 0.522 | 18 |
| 7 | c02_ia | 0.487 | 18 |
| 8 | c01 | 0.468 | 18 |

## Rankings by SYNTAX Dimension

*Higher score = better performance on syntax metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | c02_ia | 1.000 |
| 3 | ca_cb_ia_ic | 0.981 |
| 3 | ca_ia_ic | 0.981 |
| 3 | ca_ia | 0.981 |
| 6 | ca_ib | 0.963 |

## Rankings by STRUCTURE Dimension

*Higher score = better performance on structure metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.671 |
| 2 | ca | 0.663 |
| 3 | ca_ia | 0.662 |
| 4 | c02_ia | 0.606 |
| 5 | ca_ia_ic | 0.595 |

## Rankings by RESULTS Dimension

*Higher score = better performance on results metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia | 0.212 |
| 2 | ca_ic | 0.200 |
| 3 | ca_cb_ia_ic | 0.188 |
| 4 | ca | 0.133 |
| 4 | ca_ib | 0.133 |

## Rankings by ANSWER_OVERLAP Dimension

*Higher score = better performance on answer_overlap metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.620 |
| 2 | ca_ic | 0.471 |
| 3 | ca_ib | 0.458 |
| 4 | ca_ia_ic | 0.441 |
| 5 | ca_ia | 0.406 |

## Rankings by EFFICIENCY Dimension

*Higher score = better performance on efficiency metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.881 |
| 2 | ca_ic | 0.838 |
| 3 | ca_ia_ic | 0.818 |
| 4 | ca_ia | 0.786 |
| 5 | ca | 0.778 |

## 🔬 Statistical Significance Testing

 Found 4 metrics with significant differences across experiments (p < 0.05)

## Recommendations by Use Case

### Highest Result Accuracy (Standard Queries)

**Winner**: `ca_ia`

- Expected F1: ~0.205

### Highest Answer Overlap Accuracy (Standard Queries)

**Winner**: `ca_cb_ia_ic`

- Expected answer-overlap F1: ~0.614

- This metric compares shared answer variables when result tables have different columns.

### Fastest Execution

**Winner**: `ca_cb_ia_ic`

- Avg time: ~13.66s

###  Most Syntactically Valid Queries

**Winner**: `c02_ia`

- Grammar validity: 100.0%

### Best Balanced Configuration

**Recommended**: `ca_cb_ia_ic`

- Good tradeoff across validity, similarity, correctness, and efficiency
