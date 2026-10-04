# Developer Cookbook — L_OPTUNA
**Stack:** Python 3.11, optuna 3.6+, PAX 27B, PyTorch 2.10+, AIOSS_FORMAT
**Domain:** Optuna: hyperparameter optimization for PAX 27B training and Anticloud model tuning

## Hyperparameter optimization study
```python
import optuna
from l_optuna import AnticloudStudy

study = AnticloudStudy(
    pax_model="./pax-27b-fp16.safetensors",
    objective_dataset="./anticloud_eval.jsonl",
    aioss_chain="./optuna.aioss"
)

def objective(trial):
    lr = trial.suggest_float("learning_rate", 1e-6, 1e-4, log=True)
    lora_rank = trial.suggest_int("lora_rank", 4, 64)
    batch_size = trial.suggest_categorical("batch_size", [4, 8, 16])
    return study.evaluate(lr=lr, lora_rank=lora_rank, batch_size=batch_size)

result = study.optimize(objective, n_trials=50, n_jobs=2)
print(f"Best params: {result.best_params}")
print(f"Best value: {result.best_value:.4f}")
print(f"Chain: {result.chain_hash}")
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
