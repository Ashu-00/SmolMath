# SmolMath
Full Finetuning of SmolLM2 to increase performance on Math Benchmarks

## Results
### Comparision with Base Model
| **Metrics**       | **SmolLM2-135M-8k** | **SmolMath-135M** | **Δ (Change)** |
|-------------------|---------------------|--------------------|----------------|
| HellaSwag         | 42.1                | 41.15              | −0.95          |
| PIQA              | 68.4                | 63.55              | −4.85          |
| CommonsenseQA     | 33.9                | 33.42              | −0.48          |
| TriviaQA          | 4.1                 | 0.0                | −4.10          |
| Winogrande        | 51.3                | 51.78              | +0.48          |
| OpenBookQA        | 34.6                | 30.80              | −3.80          |
| GSM8K (0-shot)*    | 0.0                 | 6.9                | +6.90          |


*This was evaluated using the lighteval script, which is favoured by the SmolLM2 creators in their evaluation and varies from the SmolMath prompt structure.
### Math Benchmarks 
    
| Model                 | AddSub* (%) | MAWPS** (%) | GSM8K* (%) |
|----------------------|------------|-----------|-----------|
| apple/OpenELM-270M-Instruct | 2.14       | 2.83      |         2.05  |
| HuggingFaceTB/SmolLM2-135M-Instruct      | 1.52       |4.04      |   0.45        |
| SmolMath-no GRPO (ours)     | 9.64       | 7.47      |  6.22         |
| SmolMath (ours)             | **12.05**  | **8.31**  |       **7.51**    |

*Evaluated only on the test set, not included in the training
**Evaluated on complete dataset, not included in the training

**Model Weights**: [Huggingface](Ashed00/SmolMath-135M)

**IMPORTANT**: Please refer to this [Blog](https://hackmd.io/@ashu-00/SmolMath) for training details and methodology overview.

