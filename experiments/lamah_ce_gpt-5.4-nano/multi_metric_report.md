#  Multi-Dimensional Experiment Comparison Report

*Generated: 2026-08-04 08:35*

##  Dataset Overview

- **Total evaluations**: 144
- **Experiments**: 8 unique
- **Models**: gpt-5.4-nano
- **Schema modes**: small, ner, full, reasoning_path
- **Query types**: standard, skipped, error, count, mismatch

- **Answer-overlap metric rows**: 88/144
- **Note**: answer-overlap is reported separately and does not change the legacy weighted overall score.

- **LLM evaluation decisions**: yes=3, no=90, other=51

## LLM Evaluation Decisions by Experiment

*Normalized values are shown as rates in [0, 1]. `yes_rate_decided` uses only decided rows (`yes` + `no`).*

| Experiment | Yes | No | Other | yes_rate_total | no_rate_total | yes_rate_decided |
|------------|-----|----|-------|----------------|---------------|------------------|
| ca_ib | 1 | 12 | 5 | 0.056 | 0.667 | 0.077 |
| ca_ic | 1 | 12 | 5 | 0.056 | 0.667 | 0.077 |
| c02_ia | 1 | 14 | 3 | 0.056 | 0.778 | 0.067 |
| c01 | 0 | 6 | 12 | 0.000 | 0.333 | 0.000 |
| ca_ia | 0 | 10 | 8 | 0.000 | 0.556 | 0.000 |
| ca_cb_ia_ic | 0 | 11 | 7 | 0.000 | 0.611 | 0.000 |
| ca | 0 | 12 | 6 | 0.000 | 0.667 | 0.000 |
| ca_ia_ic | 0 | 13 | 5 | 0.000 | 0.722 | 0.000 |

## 🏆 Overall Rankings (Weighted Multi-Metric Score)

| Rank | Experiment | Score | Samples |
|------|------------|-------|---------|
| 1 | ca_ic | 0.470 | 18 |
| 2 | ca_ib | 0.464 | 18 |
| 3 | ca_ia | 0.439 | 18 |
| 4 | ca | 0.425 | 18 |
| 5 | ca_cb_ia_ic | 0.404 | 18 |
| 6 | c01 | 0.399 | 18 |
| 7 | ca_ia_ic | 0.385 | 18 |
| 8 | c02_ia | 0.358 | 18 |

## Rankings by SYNTAX Dimension

*Higher score = better performance on syntax metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | c02_ia | 0.907 |
| 2 | ca_ic | 0.870 |
| 3 | ca_ia_ic | 0.833 |
| 4 | ca_ib | 0.796 |
| 5 | ca | 0.759 |

## Rankings by STRUCTURE Dimension

*Higher score = better performance on structure metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia | 0.598 |
| 2 | c01 | 0.597 |
| 3 | ca | 0.568 |
| 4 | ca_ic | 0.556 |
| 5 | ca_ia_ic | 0.537 |

## Rankings by RESULTS Dimension

*Higher score = better performance on results metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia | 0.100 |
| 2 | ca | 0.091 |
| 3 | ca_ib | 0.077 |
| 3 | ca_ic | 0.077 |
| 6 | ca_cb_ia_ic | 0.000 |

## Rankings by ANSWER_OVERLAP Dimension

*Higher score = better performance on answer_overlap metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.300 |
| 2 | ca_ic | 0.226 |
| 3 | ca_ia | 0.167 |
| 4 | c01 | 0.164 |
| 5 | ca_ia_ic | 0.106 |

## Rankings by EFFICIENCY Dimension

*Higher score = better performance on efficiency metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ib | 0.901 |
| 2 | c01 | 0.655 |
| 3 | ca_ic | 0.619 |
| 4 | ca_ia | 0.612 |
| 5 | ca | 0.456 |

## 🔬 Statistical Significance Testing

 Found 5 metrics with significant differences across experiments (p < 0.05)

- **Grammar Validity** (syntax): p=0.0448, η²=0.112
  → Best: `c02_ia` (0.944)

- **Preparation Validity** (syntax): p=0.0244, η²=0.123
  → Best: `c02_ia` (0.944)

- **Structural Similarity (Combined)** (structure): p=0.0020, η²=0.167
  → Best: `ca` (0.809)

- **Semantic Similarity** (structure): p=0.0002, η²=0.204
  → Best: `ca` (0.654)

## Recommendations by Use Case

### Highest Result Accuracy (Standard Queries)

**Winner**: `ca_ia`

- Expected F1: ~0.100

### Highest Answer Overlap Accuracy (Standard Queries)

**Winner**: `ca_cb_ia_ic`

- Expected answer-overlap F1: ~0.300

- This metric compares shared answer variables when result tables have different columns.

### Fastest Execution

**Winner**: `ca_ib`

- Avg time: ~4.79s

###  Most Syntactically Valid Queries

**Winner**: `c02_ia`

- Grammar validity: 94.4%

### Best Balanced Configuration

**Recommended**: `ca_ic`

- Good tradeoff across validity, similarity, correctness, and efficiency
