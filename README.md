# Reasoning Model from Scratch

This project is a hands-on exploration of reasoning models built from first principles, with a focus on Qwen3-style small language models and mathematical reasoning tasks. It includes notebooks for model loading, evaluation, inference-time scaling, self-refinement, distillation, and reinforcement-learning-inspired training experiments.

## Overview

The repository is designed for learning how reasoning models work in practice:
- loading a pretrained small model
- running generation with different sampling strategies
- evaluating model performance on math problems
- experimenting with inference-time scaling and reasoning traces
- testing training-time scaling and distillation ideas

## Repository structure

- `notebooks/` — Jupyter notebooks for experiments and training/evaluation workflows
  - `generating_text_qwen_3.ipynb`
  - `evaluating_model_math.ipynb`
  - `inference_time_scaling.ipynb`
  - `inference_self_refinement.ipynb`
  - `training_time_scaling.ipynb`
  - `distillation.ipynb`
- `data/` — example datasets and evaluation outputs
- `qwen3/` — downloaded tokenizer/model files (created when notebooks run)
- `main.py` — minimal entry point
- `requirements.txt` — Python dependencies
- `pyproject.toml` — project metadata and dependencies

## Technologies used

- Python 3.11+
- PyTorch
- tokenizers
- Qwen3 model/tokenizer utilities from the `reasoning-from-scratch` ecosystem
- SymPy and math-focused evaluation workflows
- Jupyter notebooks for experimentation

## Getting started

### 1. Create a virtual environment

```bash
python -m venv .venv
```

On Windows:
```bash
.venv\Scripts\activate
```

On macOS/Linux:
```bash
source .venv/bin/activate
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

Or, if you want to install the project as a package:

```bash
pip install -e .
```

### 3. Open the notebooks

Open the notebooks in VS Code, Jupyter Lab, or Jupyter Notebook and run them in order as needed.

## Typical workflow

Most experiments follow this pattern:

1. Load the tokenizer and model
2. Prepare a prompt or dataset
3. Generate model output
4. Evaluate the result using mathematical checking or a custom verifier
5. Compare different reasoning strategies

## Data and model notes

Some notebooks may download model checkpoints and datasets during execution. This can take time depending on your internet connection and machine resources.

The project is intentionally educational and research-oriented; it is useful for understanding the implementation and behavior of small reasoning-capable language models.

## Notes

This repository is best used as a learning project or experimental playground for:
- reasoning models
- math problem solving with LLMs
- generation and evaluation pipelines
- inference-time reasoning strategies
- model training and distillation experiments

## Project status

This is an experimental research/code-learning project rather than a production application.

```
Note: All the code and material is from Reasoning Model from Scratch by Sebastian Raschka.
