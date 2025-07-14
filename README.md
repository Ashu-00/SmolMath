# SmolMath
Full Finetuning of SmolLM2 to increase performance on Math Benchmarks

## Results
| Model                 | AddSub* (%) | MAWPS** (%) | GSM8K* (%) |
|----------------------|------------|-----------|-----------|
| apple/OpenELM-270M-Instruct | 2.14       | 2.83      |           |
| HuggingFaceTB/SmolLM2-135M-Instruct      | 1.52       | 4.04      |           |
| SmolMath-no GRPO (ours)     | 9.64       | 7.47      |           |
| SmolMath (ours)             | **12.05**  | **8.31**  |           |

*Evaluated only on the test set, not included in the training
**Evaluated on complete dataset

**IMPORTANT**: Please refer to this [Blog](https://hackmd.io/@ashu-00/SmolMath) for training details and methodology overview.
