# Deploy Guide — L_OPTUNA
**Tier:** TIER_5_WORLD_NEURO_EMBODIED | **Stack:** Python 3.11, optuna 3.6+, PAX 27B, PyTorch 2.10+, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, optuna 3.6+, PyTorch 2.10+, PAX 27B weights. A100 for fast trial evaluation.

## Environment
A100 for fast HPO trials. T4 for slower but feasible trials. 32GB RAM.

## AIOSS Integration
```bash
aioss init --module L_OPTUNA --output ./l_optuna.aioss
aioss append --chain ./l_optuna.aioss --payload ./output.bin --module L_OPTUNA
aioss verify --chain ./l_optuna.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="L_OPTUNA",
    aioss_chain="./L_OPTUNA.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./L_OPTUNA.aioss --verbose
python -m L_OPTUNA.tests.smoke
```
