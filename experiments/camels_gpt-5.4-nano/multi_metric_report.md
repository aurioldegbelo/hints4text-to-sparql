#  Multi-Dimensional Experiment Comparison Report

*Generated: 2026-08-04 08:37*

##  Dataset Overview

- **Total evaluations**: 144
- **Experiments**: 8 unique
- **Models**: gpt-5.4-nano
- **Schema modes**: small, ner, full, reasoning_path
- **Query types**: standard, skipped, error, count

- **Answer-overlap metric rows**: 89/144
- **Note**: answer-overlap is reported separately and does not change the legacy weighted overall score.

- **LLM evaluation decisions**: yes=0, no=93, other=51

## LLM Evaluation Decisions by Experiment

*Normalized values are shown as rates in [0, 1]. `yes_rate_decided` uses only decided rows (`yes` + `no`).*

| Experiment | Yes | No | Other | yes_rate_total | no_rate_total | yes_rate_decided |
|------------|-----|----|-------|----------------|---------------|------------------|
| ca_ic | 0 | 10 | 8 | 0.000 | 0.556 | 0.000 |
| c01 | 0 | 11 | 7 | 0.000 | 0.611 | 0.000 |
| ca_ia | 0 | 11 | 7 | 0.000 | 0.611 | 0.000 |
| c02_ia | 0 | 12 | 6 | 0.000 | 0.667 | 0.000 |
| ca | 0 | 12 | 6 | 0.000 | 0.667 | 0.000 |
| ca_cb_ia_ic | 0 | 12 | 6 | 0.000 | 0.667 | 0.000 |
| ca_ib | 0 | 12 | 6 | 0.000 | 0.667 | 0.000 |
| ca_ia_ic | 0 | 13 | 5 | 0.000 | 0.722 | 0.000 |

## 🏆 Overall Rankings (Weighted Multi-Metric Score)

| Rank | Experiment | Score | Samples |
|------|------------|-------|---------|
| 1 | c01 | 0.438 | 18 |
| 2 | ca | 0.437 | 18 |
| 3 | ca_ia | 0.428 | 18 |
| 4 | ca_cb_ia_ic | 0.407 | 18 |
| 5 | ca_ia_ic | 0.393 | 18 |
| 6 | ca_ic | 0.380 | 18 |
| 7 | c02_ia | 0.370 | 18 |
| 8 | ca_ib | 0.363 | 18 |

## Rankings by SYNTAX Dimension

*Higher score = better performance on syntax metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia_ic | 0.796 |
| 2 | ca | 0.778 |
| 2 | ca_ib | 0.778 |
| 4 | c02_ia | 0.741 |
| 4 | ca_cb_ia_ic | 0.741 |

## Rankings by STRUCTURE Dimension

*Higher score = better performance on structure metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca | 0.608 |
| 2 | ca_ic | 0.591 |
| 3 | c01 | 0.573 |
| 4 | ca_ia | 0.554 |
| 5 | ca_cb_ia_ic | 0.532 |

## Rankings by RESULTS Dimension

*Higher score = better performance on results metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 4 | c01 | 0.000 |
| 4 | c02_ia | 0.000 |
| 4 | ca | 0.000 |
| 4 | ca_cb_ia_ic | 0.000 |
| 4 | ca_ia | 0.000 |

## Rankings by ANSWER_OVERLAP Dimension

*Higher score = better performance on answer_overlap metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | c01 | 0.200 |
| 2 | ca_ia | 0.100 |
| 3 | ca | 0.056 |
| 4 | ca_cb_ia_ic | 0.003 |
| 6 | c02_ia | 0.000 |

## Rankings by EFFICIENCY Dimension

*Higher score = better performance on efficiency metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | c01 | 0.665 |
| 2 | ca | 0.618 |
| 3 | ca_ia | 0.579 |
| 4 | ca_ia_ic | 0.542 |
| 5 | ca_cb_ia_ic | 0.508 |

## 🔬 Statistical Significance Testing

 Found 2 metrics with significant differences across experiments (p < 0.05)

## Recommendations by Use Case

### Highest Result Accuracy (Standard Queries)

**Winner**: `c01`

- Expected F1: ~0.000

### Highest Answer Overlap Accuracy (Standard Queries)

**Winner**: `c01`

- Expected answer-overlap F1: ~0.200

- This metric compares shared answer variables when result tables have different columns.

### Fastest Execution

**Winner**: `c01`

- Avg time: ~3.26s

###  Most Syntactically Valid Queries

**Winner**: `ca_ia_ic`

- Grammar validity: 83.3%

### Best Balanced Configuration

**Recommended**: `c01`

- Good tradeoff across validity, similarity, correctness, and efficiency
