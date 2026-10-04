# 3-Seed Simulation — L_OPTUNA

**Seeds:** `61078` · `92415` · `26614`

**Seed method:** `sha256("L_OPTUNA")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `L_OPTUNA`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 7.092 | 0.1737 | ±0.3405 |
| throughput_tokens_per_sec | 1368.2333 | 23.7981 | ±46.6443 |
| p50_latency_ms | 41.54 | 4.4566 | ±8.7349 |
| p99_latency_ms | 115.23 | 12.6541 | ±24.802 |
| ttft_ms | 26.4467 | 1.2422 | ±2.4347 |
| mmlu_proxy | 0.7195 | 0.0304 | ±0.0596 |
| hellaswag_proxy | 0.7697 | 0.0302 | ±0.0592 |
| truthfulqa_proxy | 0.5946 | 0.0477 | ±0.0935 |
| arc_proxy | 0.7042 | 0.0182 | ±0.0357 |
| complexity_cyclomatic | 4.0633 | 0.6561 | ±1.286 |
| maintainability_index | 67.5433 | 4.1201 | ±8.0754 |
| security_issues_high | 1.0 | 0.8165 | ±1.6003 |
| dependency_freshness_pct | 80.0 | 7.3089 | ±14.3254 |
| test_coverage_pct | 65.3667 | 3.7748 | ±7.3986 |
| doc_coverage_pct | 64.8667 | 5.9779 | ±11.7167 |
| memory_mb | 50.0 | 0.0 | ±0.0 |
| gpu_util_pct | 66.7 | 5.0259 | ±9.8508 |
| openssf_score | 6.8167 | 0.4781 | ±0.9371 |
| eu_ai_act_compliance_pct | 80.0667 | 0.7134 | ±1.3983 |
| slsa_level | 1.3333 | 0.4714 | ±0.9239 |

## Per-Seed Raw Results

| Metric | Seed 61078 | Seed 92415 | Seed 26614 |
|--------|------------|------------|------------|
| trl_score | 7.199 | 7.23 | 6.847 |
| throughput_tokens_per_sec | 1401.4 | 1346.7 | 1356.6 |
| p50_latency_ms | 47.83 | 38.05 | 38.74 |
| p99_latency_ms | 122.53 | 125.73 | 97.43 |
| ttft_ms | 25.07 | 28.08 | 26.19 |
| mmlu_proxy | 0.7411 | 0.741 | 0.6765 |
| hellaswag_proxy | 0.8063 | 0.7705 | 0.7324 |
| truthfulqa_proxy | 0.528 | 0.6372 | 0.6185 |
| arc_proxy | 0.7295 | 0.6957 | 0.6873 |
| complexity_cyclomatic | 3.64 | 3.56 | 4.99 |
| maintainability_index | 64.6 | 73.37 | 64.66 |
| security_issues_high | 0 | 2 | 1 |
| dependency_freshness_pct | 84.4 | 69.7 | 85.9 |
| test_coverage_pct | 62.9 | 62.5 | 70.7 |
| doc_coverage_pct | 66.4 | 71.3 | 56.9 |
| memory_mb | 50 | 50 | 50 |
| gpu_util_pct | 72.7 | 67.0 | 60.4 |
| openssf_score | 6.91 | 6.19 | 7.35 |
| eu_ai_act_compliance_pct | 79.1 | 80.3 | 80.8 |
| slsa_level | 1 | 1 | 2 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._