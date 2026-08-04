#  Multi-Dimensional Experiment Comparison Report

*Generated: 2026-08-04 08:46*

##  Dataset Overview

- **Total evaluations**: 144
- **Experiments**: 8 unique
- **Models**: gpt-4.1
- **Schema modes**: small, ner, full, reasoning_path
- **Query types**: standard, error, skipped, count

- **Answer-overlap metric rows**: 105/144
- **Note**: answer-overlap is reported separately and does not change the legacy weighted overall score.

- **LLM evaluation decisions**: yes=5, no=106, other=33

## LLM Evaluation Decisions by Experiment

*Normalized values are shown as rates in [0, 1]. `yes_rate_decided` uses only decided rows (`yes` + `no`).*

| Experiment | Yes | No | Other | yes_rate_total | no_rate_total | yes_rate_decided |
|------------|-----|----|-------|----------------|---------------|------------------|
| ca_ia_ic | 2 | 12 | 4 | 0.111 | 0.667 | 0.143 |
| ca_cb_ia_ic | 2 | 14 | 2 | 0.111 | 0.778 | 0.125 |
| ca_ib | 1 | 14 | 3 | 0.056 | 0.778 | 0.067 |
| ca_ia | 0 | 9 | 9 | 0.000 | 0.500 | 0.000 |
| ca | 0 | 12 | 6 | 0.000 | 0.667 | 0.000 |
| c01 | 0 | 14 | 4 | 0.000 | 0.778 | 0.000 |
| ca_ic | 0 | 14 | 4 | 0.000 | 0.778 | 0.000 |
| c02_ia | 0 | 17 | 1 | 0.000 | 0.944 | 0.000 |

## 🏆 Overall Rankings (Weighted Multi-Metric Score)

| Rank | Experiment | Score | Samples |
|------|------------|-------|---------|
| 1 | ca_cb_ia_ic | 0.578 | 18 |
| 2 | ca_ia | 0.543 | 18 |
| 3 | ca | 0.542 | 18 |
| 4 | ca_ia_ic | 0.538 | 18 |
| 5 | ca_ic | 0.504 | 18 |
| 6 | c02_ia | 0.487 | 18 |
| 7 | ca_ib | 0.468 | 18 |
| 8 | c01 | 0.450 | 18 |

## Rankings by SYNTAX Dimension

*Higher score = better performance on syntax metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | c02_ia | 0.963 |
| 2 | ca_ib | 0.870 |
| 3 | c01 | 0.852 |
| 5 | ca_cb_ia_ic | 0.833 |
| 5 | ca_ic | 0.833 |

## Rankings by STRUCTURE Dimension

*Higher score = better performance on structure metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_ic | 0.661 |
| 2 | ca_cb_ia_ic | 0.657 |
| 3 | c01 | 0.652 |
| 4 | c02_ia | 0.640 |
| 5 | ca | 0.625 |

## Rankings by RESULTS Dimension

*Higher score = better performance on results metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.250 |
| 1 | ca_ia | 0.250 |
| 3 | ca_ia_ic | 0.231 |
| 4 | ca | 0.167 |
| 5 | ca_ic | 0.077 |

## Rankings by ANSWER_OVERLAP Dimension

*Higher score = better performance on answer_overlap metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | ca_cb_ia_ic | 0.624 |
| 2 | ca_ia_ic | 0.529 |
| 3 | ca | 0.462 |
| 4 | ca_ia | 0.458 |
| 5 | ca_ic | 0.414 |

## Rankings by EFFICIENCY Dimension

*Higher score = better performance on efficiency metrics*

| Rank | Experiment | Score |
|------|------------|-------|
| 1 | c02_ia | 0.793 |
| 2 | ca_ia | 0.751 |
| 3 | c01 | 0.717 |
| 4 | ca_ia_ic | 0.686 |
| 5 | ca_ib | 0.657 |

## 🔬 Statistical Significance Testing

 Found 7 metrics with significant differences across experiments (p < 0.05)

- **String Similarity** (structure): p=0.0294, η²=0.119
  → Best: `ca_cb_ia_ic` (0.657)

- **Answer Overlap F1** (answer_overlap): p=0.0105, η²=0.193
  → Best: `ca_cb_ia_ic` (0.626)

- **Answer Overlap Precision** (answer_overlap): p=0.0077, η²=0.201
  → Best: `ca_cb_ia_ic` (0.675)

- **Answer Overlap Recall** (answer_overlap): p=0.0089, η²=0.198
  → Best: `ca_cb_ia_ic` (0.604)

- **Answer Overlap Jaccard** (answer_overlap): p=0.0105, η²=0.193
  → Best: `ca_cb_ia_ic` (0.592)

## Recommendations by Use Case

### Highest Result Accuracy (Standard Queries)

**Winner**: `ca_cb_ia_ic`

- Expected F1: ~0.250

### Highest Answer Overlap Accuracy (Standard Queries)

**Winner**: `ca_cb_ia_ic`

- Expected answer-overlap F1: ~0.626

- This metric compares shared answer variables when result tables have different columns.

### Fastest Execution

**Winner**: `c02_ia`

- Avg time: ~1.44s

###  Most Syntactically Valid Queries

**Winner**: `c02_ia`

- Grammar validity: 100.0%

### Best Balanced Configuration

**Recommended**: `ca_cb_ia_ic`

- Good tradeoff across validity, similarity, correctness, and efficiency
