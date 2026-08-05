#  Multi-Dimensional Experiment Comparison Report

*Generated: 2026-08-04 11:09*

##  Dataset Overview

- **Total evaluations**: 144
- **Experiments**: 8 unique
- **Models**: gpt-5.4-mini
- **Schema modes**: reasoning_path, small, full, ner
- **Query types**: standard, skipped, error, count

- **Answer-overlap metric rows**: 103/144
- **Note**: answer-overlap is reported separately and does not change the legacy weighted overall score.

- **LLM evaluation decisions**: yes=0, no=109, other=35

## LLM Evaluation Decisions by Experiment

*Normalized values are shown as rates in [0, 1]. `yes_rate_decided` uses only decided rows (`yes` + `no`).*

| Experiment | Yes | No | Other | yes_rate_total | no_rate_total | yes_rate_decided |
|------------|-----|----|-------|----------------|---------------|------------------|
| ca | 0 | 10 | 8 | 0.000 | 0.556 | 0.000 |
| ca_ia | 0 | 12 | 6 | 0.000 | 0.667 | 0.000 |
| c01 | 0 | 13 | 5 | 0.000 | 0.722 | 0.000 |
| ca_ia_ic | 0 | 13 | 5 | 0.000 | 0.722 | 0.000 |
| c02_ia | 0 | 15 | 3 | 0.000 | 0.833 | 0.000 |
| ca_cb_ia_ic | 0 | 15 | 3 | 0.000 | 0.833 | 0.000 |
| ca_ic | 0 | 15 | 3 | 0.000 | 0.833 | 0.000 |
| ca_ib | 0 | 16 | 2 | 0.000 | 0.889 | 0.000 |

## 🏆 Overall Rankings (Weighted Multi-Metric Score)

| Rank | Experiment | Score | Samples |
|------|------------|-------|---------|
| 1 | ca_ib | 0.500 | 18 |
| 2 | ca_cb_ia_ic | 0.500 | 18 |
| 3 | ca_ia_ic | 0.494 | 18 |
| 4 | ca_ic | 0.492 | 18 |
| 5 | ca_ia | 0.474 | 18 |
| 6 | ca | 0.467 | 18 |
| 7 | c02_ia | 0.446 | 18 |
| 8 | c01 | 0.441 | 18 |

## Rankings by SYNTAX Dimension

*Higher score = better performance on syntax metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ib | 0.963 |
| 2 | c02_ia | 0.870 |
| 4 | ca_ia_ic | 0.852 |
| 4 | ca_cb_ia_ic | 0.852 |
| 4 | ca_ic | 0.852 |

## Rankings by STRUCTURE Dimension

*Higher score = better performance on structure metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia | 0.717 |
| 2 | ca | 0.670 |
| 3 | ca_ib | 0.613 |
| 4 | ca_ic | 0.589 |
| 5 | ca_ia_ic | 0.585 |

## Rankings by RESULTS Dimension

*Higher score = better performance on results metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia_ic | 0.167 |
| 2 | ca_cb_ia_ic | 0.143 |
| 3 | ca | 0.100 |
| 4 | ca_ia | 0.091 |
| 5 | ca_ib | 0.067 |

## Rankings by ANSWER_OVERLAP Dimension

*Higher score = better performance on answer_overlap metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia_ic | 0.250 |
| 2 | ca_ic | 0.244 |
| 3 | ca_ia | 0.218 |
| 4 | ca_ib | 0.217 |
| 5 | ca_cb_ia_ic | 0.205 |

## Rankings by EFFICIENCY Dimension

*Higher score = better performance on efficiency metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ic | 0.828 |
| 2 | ca_cb_ia_ic | 0.785 |
| 3 | c01 | 0.775 |
| 4 | ca | 0.640 |
| 5 | c02_ia | 0.634 |

## 🔬 Statistical Significance Testing

 Found 1 metrics with significant differences across experiments (p < 0.05)

## Recommendations by Use Case

### Highest Result Accuracy (Standard Queries)

**Winner**: `ca_ia_ic`

- Expected F1: ~0.167

### Highest Answer Overlap Accuracy (Standard Queries)

**Winner**: `ca_ia_ic`

- Expected answer-overlap F1: ~0.250

- This metric compares shared answer variables when result tables have different columns.

### Fastest Execution

**Winner**: `ca_ic`

- Avg time: ~2.11s

###  Most Syntactically Valid Queries

**Winner**: `ca_ib`

- Grammar validity: 100.0%

### Best Balanced Configuration

**Recommended**: `ca_ib`

- Good tradeoff across validity, similarity, correctness, and efficiency
