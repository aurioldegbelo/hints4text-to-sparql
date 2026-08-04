#  Multi-Dimensional Experiment Comparison Report

*Generated: 2026-08-04 08:43*

##  Dataset Overview

- **Total evaluations**: 144
- **Experiments**: 8 unique
- **Models**: gpt-5.5
- **Schema modes**: small, ner, full, reasoning_path
- **Query types**: standard, error, count

- **Answer-overlap metric rows**: 125/144
- **Note**: answer-overlap is reported separately and does not change the legacy weighted overall score.

- **LLM evaluation decisions**: yes=19, no=114, other=11

## LLM Evaluation Decisions by Experiment

*Normalized values are shown as rates in [0, 1]. `yes_rate_decided` uses only decided rows (`yes` + `no`).*

| Experiment | Yes | No | Other | yes_rate_total | no_rate_total | yes_rate_decided |
|------------|-----|----|-------|----------------|---------------|------------------|
| ca_ia | 6 | 10 | 2 | 0.333 | 0.556 | 0.375 |
| ca | 4 | 12 | 2 | 0.222 | 0.667 | 0.250 |
| ca_cb_ia_ic | 3 | 14 | 1 | 0.167 | 0.778 | 0.176 |
| c01 | 2 | 15 | 1 | 0.111 | 0.833 | 0.118 |
| ca_ic | 2 | 15 | 1 | 0.111 | 0.833 | 0.118 |
| ca_ia_ic | 1 | 15 | 2 | 0.056 | 0.833 | 0.062 |
| ca_ib | 1 | 16 | 1 | 0.056 | 0.889 | 0.059 |
| c02_ia | 0 | 17 | 1 | 0.000 | 0.944 | 0.000 |

## 🏆 Overall Rankings (Weighted Multi-Metric Score)

| Rank | Experiment | Score | Samples |
|------|------------|-------|---------|
| 1 | ca | 0.580 | 18 |
| 2 | ca_cb_ia_ic | 0.566 | 18 |
| 3 | ca_ib | 0.523 | 18 |
| 4 | ca_ia_ic | 0.521 | 18 |
| 5 | ca_ia | 0.521 | 18 |
| 6 | c01 | 0.509 | 18 |
| 7 | ca_ic | 0.502 | 18 |
| 8 | c02_ia | 0.486 | 18 |

## Rankings by SYNTAX Dimension

*Higher score = better performance on syntax metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 2 | c01 | 0.981 |
| 2 | c02_ia | 0.981 |
| 2 | ca_ib | 0.981 |
| 2 | ca_ic | 0.981 |
| 6 | ca_ia_ic | 0.963 |

## Rankings by STRUCTURE Dimension

*Higher score = better performance on structure metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ia | 0.643 |
| 2 | ca_ia_ic | 0.618 |
| 3 | c02_ia | 0.615 |
| 4 | ca | 0.589 |
| 5 | ca_ic | 0.576 |

## Rankings by RESULTS Dimension

*Higher score = better performance on results metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca | 0.200 |
| 2 | ca_cb_ia_ic | 0.144 |
| 3 | ca_ia | 0.133 |
| 4 | ca_ib | 0.062 |
| 6 | c01 | 0.000 |

## Rankings by ANSWER_OVERLAP Dimension

*Higher score = better performance on answer_overlap metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.603 |
| 2 | ca | 0.600 |
| 3 | ca_ia | 0.511 |
| 4 | ca_ia_ic | 0.343 |
| 5 | ca_ic | 0.322 |

## Rankings by EFFICIENCY Dimension

*Higher score = better performance on efficiency metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | c01 | 0.814 |
| 2 | ca | 0.782 |
| 3 | c02_ia | 0.721 |
| 4 | ca_ia_ic | 0.712 |
| 5 | ca_ic | 0.675 |

## 🔬 Statistical Significance Testing

 Found 5 metrics with significant differences across experiments (p < 0.05)

- **Answer Overlap F1** (answer_overlap): p=0.0282, η²=0.140
  → Best: `ca` (0.600)

- **Answer Overlap Precision** (answer_overlap): p=0.0165, η²=0.151
  → Best: `ca_cb_ia_ic` (0.771)

- **Answer Overlap Recall** (answer_overlap): p=0.0323, η²=0.137
  → Best: `ca` (0.600)

- **Answer Overlap Jaccard** (answer_overlap): p=0.0282, η²=0.140
  → Best: `ca` (0.600)

## Recommendations by Use Case

### Highest Result Accuracy (Standard Queries)

**Winner**: `ca`

- Expected F1: ~0.200

### Highest Answer Overlap Accuracy (Standard Queries)

**Winner**: `ca_cb_ia_ic`

- Expected answer-overlap F1: ~0.583

- This metric compares shared answer variables when result tables have different columns.

### Fastest Execution

**Winner**: `c01`

- Avg time: ~17.66s

###  Most Syntactically Valid Queries

**Winner**: `c01`

- Grammar validity: 100.0%

### Best Balanced Configuration

**Recommended**: `ca`

- Good tradeoff across validity, similarity, correctness, and efficiency
