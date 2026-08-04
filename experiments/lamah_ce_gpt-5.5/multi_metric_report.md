#  Multi-Dimensional Experiment Comparison Report

*Generated: 2026-08-04 08:41*

##  Dataset Overview

- **Total evaluations**: 144
- **Experiments**: 8 unique
- **Models**: gpt-5.5
- **Schema modes**: small, ner, full, reasoning_path
- **Query types**: standard, error, count

- **Answer-overlap metric rows**: 108/144
- **Note**: answer-overlap is reported separately and does not change the legacy weighted overall score.

- **LLM evaluation decisions**: yes=10, no=113, other=21

## LLM Evaluation Decisions by Experiment

*Normalized values are shown as rates in [0, 1]. `yes_rate_decided` uses only decided rows (`yes` + `no`).*

| Experiment | Yes | No | Other | yes_rate_total | no_rate_total | yes_rate_decided |
|------------|-----|----|-------|----------------|---------------|------------------|
| ca_cb_ia_ic | 4 | 10 | 4 | 0.222 | 0.556 | 0.286 |
| ca_ia_ic | 2 | 13 | 3 | 0.111 | 0.722 | 0.133 |
| ca | 2 | 14 | 2 | 0.111 | 0.778 | 0.125 |
| c02_ia | 1 | 15 | 2 | 0.056 | 0.833 | 0.062 |
| ca_ic | 1 | 15 | 2 | 0.056 | 0.833 | 0.062 |
| ca_ia | 0 | 14 | 4 | 0.000 | 0.778 | 0.000 |
| c01 | 0 | 16 | 2 | 0.000 | 0.889 | 0.000 |
| ca_ib | 0 | 16 | 2 | 0.000 | 0.889 | 0.000 |

## 🏆 Overall Rankings (Weighted Multi-Metric Score)

| Rank | Experiment | Score | Samples |
|------|------------|-------|---------|
| 1 | ca_cb_ia_ic | 0.658 | 18 |
| 2 | ca_ic | 0.540 | 18 |
| 3 | ca_ia | 0.529 | 18 |
| 4 | ca | 0.526 | 18 |
| 5 | ca_ia_ic | 0.525 | 18 |
| 6 | c02_ia | 0.489 | 18 |
| 7 | ca_ib | 0.486 | 18 |
| 8 | c01 | 0.457 | 18 |

## Rankings by SYNTAX Dimension

*Higher score = better performance on syntax metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 3 | c01 | 0.963 |
| 3 | c02_ia | 0.963 |
| 3 | ca | 0.963 |
| 3 | ca_ic | 0.963 |
| 3 | ca_ib | 0.963 |

## Rankings by STRUCTURE Dimension

*Higher score = better performance on structure metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia | 0.639 |
| 2 | ca_cb_ia_ic | 0.635 |
| 3 | ca_ib | 0.590 |
| 4 | ca | 0.563 |
| 5 | ca_ic | 0.556 |

## Rankings by RESULTS Dimension

*Higher score = better performance on results metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.231 |
| 2 | ca_ia_ic | 0.154 |
| 3 | ca_ic | 0.143 |
| 4 | ca_ia | 0.083 |
| 5 | ca | 0.071 |

## Rankings by ANSWER_OVERLAP Dimension

*Higher score = better performance on answer_overlap metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.932 |
| 2 | ca | 0.340 |
| 3 | ca_ia_ic | 0.329 |
| 4 | ca_ia | 0.258 |
| 5 | ca_ic | 0.245 |

## Rankings by EFFICIENCY Dimension

*Higher score = better performance on efficiency metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia | 0.775 |
| 2 | ca_ic | 0.772 |
| 3 | c01 | 0.747 |
| 4 | ca | 0.709 |
| 5 | c02_ia | 0.704 |

## 🔬 Statistical Significance Testing

 Found 7 metrics with significant differences across experiments (p < 0.05)

- **Answer Overlap F1** (answer_overlap): p=0.0002, η²=0.277
  → Best: `ca_cb_ia_ic` (0.933)

- **Answer Overlap Precision** (answer_overlap): p=0.0001, η²=0.297
  → Best: `ca_cb_ia_ic` (1.000)

- **Answer Overlap Recall** (answer_overlap): p=0.0005, η²=0.260
  → Best: `ca_cb_ia_ic` (0.897)

- **Answer Overlap Jaccard** (answer_overlap): p=0.0002, η²=0.279
  → Best: `ca_cb_ia_ic` (0.897)

## Recommendations by Use Case

### Highest Result Accuracy (Standard Queries)

**Winner**: `ca_cb_ia_ic`

- Expected F1: ~0.231

### Highest Answer Overlap Accuracy (Standard Queries)

**Winner**: `ca_cb_ia_ic`

- Expected answer-overlap F1: ~0.933

- This metric compares shared answer variables when result tables have different columns.

### Fastest Execution

**Winner**: `ca_ia`

- Avg time: ~17.18s

###  Most Syntactically Valid Queries

**Winner**: `c01`

- Grammar validity: 100.0%

### Best Balanced Configuration

**Recommended**: `ca_cb_ia_ic`

- Good tradeoff across validity, similarity, correctness, and efficiency
