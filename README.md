# ml-experiments

Notebooks and training runs from my ML experiments. Mostly NLP, plus a lot of poking at quantized models on hardware that doesn't have much memory.

## Notebooks

| Notebook | What it does |
|---|---|
| `bert_text_classification.ipynb` | Fine-tunes bert-base on SST-2 |
| `gpt2_text_generation.ipynb` | GPT-2 generation with top-k and nucleus sampling |
| `quantization_benchmark.ipynb` | fp32 vs fp16 vs int8, speed and memory |
| `lora_vs_full_finetune.ipynb` | LoRA vs full fine-tuning on a small classification task |

## Heads up

These are experiments, so the code is rough in places, and I haven't checked that the results come out the same on other machines.

## Setup

```bash
pip install -r requirements.txt
jupyter notebook
```

## What I ran it on

- RTX 3080 (10GB)
- Colab T4
- CPU, which works but is slow for anything big
