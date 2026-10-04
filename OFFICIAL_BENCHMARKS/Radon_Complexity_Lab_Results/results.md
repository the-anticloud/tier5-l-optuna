# Radon_Complexity_Lab_Results
**Project:** `L_OPTUNA` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'A', 'score': 2.9194630872483223}`
- **complexity_grade:** `A`
- **complexity_score:** `2.9194630872483223`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_OPTUNA\UPSTREAM\optuna\cli.py - B (13.03)
E:\fenta\Downlo`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_OPTUNA\UPSTREAM\optuna\cli.py
    F 98:0 _convert_to_dict - D (25)
    F 204:0 _dump_table - C (13)
    F 57:0 _get_storage - B (10)
    F 82:0 _format_value - B (10)
    M 689:4 _Ask.take_action - B (10)
    F 244:0 _format_output - B (8)
    C 655:0 _Ask - B (7)
    M 441:4 _Studies.take_action - B (6)
    F 929:0 _preprocess_argv - A (5)
    C 415:0 _Studies - A (5)
    C 625:0 _StorageUpgrade - A (5)
    F 191:0 _dump_value - A (4)
    F 977:0 main - A (4)
    M 628:4 _StorageUpgrade.take_action - A (4)
    F 42:0 _check_storage_url - A (3)
    C 162:0 CellValue - A (3)
    M 163:4 CellValue.__init__ - A (3)
    M 181:4 CellValue.get_string - A (3)
    C 391:0 _StudyNames - A (3)
    C 470:0 _Trials - A (3)
    C 520:0 _BestTrial - A (3)
    C 573:0 _BestTrials - A (3)
    M 598:4 _BestTrials.take_action - A (3)
    C 760:0 _Tell - A (3)
    F 829:0 _parse_storage_class_without_suggesting_deprecated_choices - A (2)
    F 893:0 _add_commands - A (2)
    F 963:0 _set_log_file - A (2)
    M 172:4 CellValue.__str__ - A (2)
    C 273:0 _BaseCommand - A (2)
    C 307:0 _CreateStudy - A (2)
    C 355:0 _DeleteStudy - A (2)
    C 368:0 _StudySetUserAttribute - A (2)
    M 404:4 _StudyNames.take_action - A (2)
    M 495:4 _Trials.take_action - A (2)
    M 545:4 _BestTrial.take_action - A (2)
    M 781:4 _Tell.take_action - A (2)
    F 846:0 _add_common_arguments - A (1)
    F 917:0 _get_parser - A (1)
    F 945:0 _set_
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_