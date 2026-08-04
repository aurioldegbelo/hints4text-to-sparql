#  Multi-Dimensional Experiment Comparison Report

*Generated: 2026-08-04 08:45*

##  Dataset Overview

- **Total evaluations**: 144
- **Experiments**: 8 unique
- **Models**: gpt-4.1
- **Schema modes**: small, ner, full, reasoning_path
- **Query types**: standard, skipped, error, count, mismatch

- **Answer-overlap metric rows**: 76/144
- **Note**: answer-overlap is reported separately and does not change the legacy weighted overall score.

- **LLM evaluation decisions**: yes=7, no=75, other=62

## LLM Evaluation Decisions by Experiment

*Normalized values are shown as rates in [0, 1]. `yes_rate_decided` uses only decided rows (`yes` + `no`).*

| Experiment | Yes | No | Other | yes_rate_total | no_rate_total | yes_rate_decided |
|------------|-----|----|-------|----------------|---------------|------------------|
| ca_cb_ia_ic | 4 | 10 | 4 | 0.222 | 0.556 | 0.286 |
| ca_ic | 2 | 10 | 6 | 0.111 | 0.556 | 0.167 |
| ca_ia_ic | 1 | 10 | 7 | 0.056 | 0.556 | 0.091 |
| ca | 0 | 6 | 12 | 0.000 | 0.333 | 0.000 |
| ca_ia | 0 | 6 | 12 | 0.000 | 0.333 | 0.000 |
| c01 | 0 | 9 | 9 | 0.000 | 0.500 | 0.000 |
| c02_ia | 0 | 11 | 7 | 0.000 | 0.611 | 0.000 |
| ca_ib | 0 | 13 | 5 | 0.000 | 0.722 | 0.000 |

## 🏆 Overall Rankings (Weighted Multi-Metric Score)

| Rank | Experiment | Score | Samples |
|------|------------|-------|---------|
| 1 | ca_cb_ia_ic | 0.569 | 18 |
| 2 | ca_ic | 0.527 | 18 |
| 3 | ca_ia_ic | 0.483 | 18 |
| 4 | ca_ia | 0.477 | 18 |
| 5 | ca | 0.467 | 18 |
| 6 | ca_ib | 0.460 | 18 |
| 7 | c02_ia | 0.451 | 18 |
| 8 | c01 | 0.441 | 18 |

## Rankings by SYNTAX Dimension

*Higher score = better performance on syntax metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ib | 0.889 |
| 2 | ca_cb_ia_ic | 0.852 |
| 3 | ca_ic | 0.833 |
| 4 | c02_ia | 0.815 |
| 4 | ca_ia_ic | 0.815 |

## Rankings by STRUCTURE Dimension

*Higher score = better performance on structure metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca | 0.633 |
| 2 | ca_ic | 0.632 |
| 3 | c02_ia | 0.610 |
| 4 | c01 | 0.605 |
| 5 | ca_ib | 0.595 |

## Rankings by RESULTS Dimension

*Higher score = better performance on results metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ic | 0.182 |
| 2 | ca_cb_ia_ic | 0.154 |
| 3 | ca_ia_ic | 0.100 |
| 6 | c01 | 0.000 |
| 6 | ca | 0.000 |

## Rankings by ANSWER_OVERLAP Dimension

*Higher score = better performance on answer_overlap metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.701 |
| 2 | ca_ic | 0.364 |
| 3 | ca_ia_ic | 0.300 |
| 4 | ca | 0.167 |
| 4 | ca_ia | 0.167 |

## Rankings by EFFICIENCY Dimension

*Higher score = better performance on efficiency metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia | 0.814 |
| 2 | c01 | 0.798 |
| 3 | ca | 0.707 |
| 4 | c02_ia | 0.671 |
| 5 | ca_cb_ia_ic | 0.656 |

## 🔬 Statistical Significance Testing

 Found 8 metrics with significant differences across experiments (p < 0.05)

- **Grammar Validity** (syntax): p=0.0020, η²=0.167
  → Best: `c02_ia` (1.000)

- **Answer Overlap F1** (answer_overlap): p=0.0239, η²=0.246
  → Best: `ca_cb_ia_ic` (0.703)

- **Answer Overlap Precision** (answer_overlap): p=0.0098, η²=0.279
  → Best: `ca_cb_ia_ic` (0.769)

- **Answer Overlap Recall** (answer_overlap): p=0.0291, η²=0.239
  → Best: `ca_cb_ia_ic` (0.667)

- **Answer Overlap Jaccard** (answer_overlap): p=0.0239, η²=0.246
  → Best: `ca_cb_ia_ic` (0.667)

## Recommendations by Use Case

### Highest Result Accuracy (Standard Queries)

**Winner**: `ca_ic`

- Expected F1: ~0.182

### Highest Answer Overlap Accuracy (Standard Queries)

**Winner**: `ca_cb_ia_ic`

- Expected answer-overlap F1: ~0.703

- This metric compares shared answer variables when result tables have different columns.

### Fastest Execution

**Winner**: `ca_ia`

- Avg time: ~2.24s

###  Most Syntactically Valid Queries

**Winner**: `ca_ib`

- Grammar validity: 100.0%

### Best Balanced Configuration

**Recommended**: `ca_cb_ia_ic`

- Good tradeoff across validity, similarity, correctness, and efficiency
