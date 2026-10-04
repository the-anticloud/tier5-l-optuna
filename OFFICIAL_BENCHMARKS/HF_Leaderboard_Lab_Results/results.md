# HF_Leaderboard_Lab_Results

**Project:** `L_OPTUNA`  
**Tier:** `TIER_5_WORLD_NEURO_EMBODIED`  
**Slug:** `optuna/optuna`  
**Commit:** `0684fbd74793`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **46.41 ms** |
| Min latency | 42.02 ms |
| Max latency | 50.54 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **33** |
| Tokenization latency | 1.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5901 |
| Classification latency | 94.99 ms |
| Status | **PASS** |

**Input text tokenized:**
```
L_OPTUNA (optuna/optuna) — 472 files, 72054 source lines, licence MIT, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'l', '_', 'opt', '##una', '(', 'opt', '##una', '/', 'opt', '##una', ')', '—', '47', '##2', 'files', ',', '720', '##54', 'source']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_