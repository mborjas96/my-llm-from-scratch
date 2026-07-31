# My LLM From Scratch Build

A from-scratch implementation of a GPT-style large language model in Python and PyTorch, based on Sebastian Raschka's *Build a Large Language Model (From Scratch)*.

The purpose of this repository is to build working language models from first principles, understand each major component of the training and inference pipeline, and then use those models as a foundation for controlled experiments in realistic application scenarios.

> **Status:** In progress

## Project Goals

This project has two primary goals:

1. Build and train a GPT-style language model from scratch by implementing the core concepts presented in *Build a Large Language Model (From Scratch)*.
2. Go beyond the book by extending, evaluating, and experimenting with the resulting models across applied scenarios and original research questions.

The repository is intended to produce working implementations, reproducible experiments, and documented findings. It is not primarily a chapter-by-chapter progress journal.

## Core Implementation

The initial implementation will cover:

- Text collection and preprocessing
- Tokenization and vocabulary construction
- Input-target pair generation
- Token and positional embeddings
- Self-attention
- Causal attention
- Multi-head attention
- Layer normalization
- Feed-forward neural networks
- Transformer blocks
- GPT-style model architecture
- Pretraining
- Text generation
- Model evaluation
- Classification fine-tuning
- Instruction fine-tuning

## Project Roadmap

| Phase | Focus | Status |
|---|---|---|
| 1 | Repository, environment, and development setup | In progress |
| 2 | Text processing and tokenization | Not started |
| 3 | Attention mechanisms | Not started |
| 4 | GPT model architecture | Not started |
| 5 | Pretraining and text generation | Not started |
| 6 | Model evaluation and training analysis | Not started |
| 7 | Classification fine-tuning | Not started |
| 8 | Instruction fine-tuning | Not started |
| 9 | Applied experimentation and original research | Not started |
| 10 | Final analysis, research report, and demonstrations | Not started |

Detailed work will be tracked using GitHub Issues, Milestones, and a linked GitHub Project.

## Applied Experimentation and Original Research

After completing the core implementation, the project will use the resulting models as an experimental platform.

Potential research directions include:

- Small language models in offline or resource-constrained environments
- Local AI assistants for isolated environments
- Reliability in safety-critical or high-consequence tasks
- Effects of model size, context length, and dataset quality
- Domain adaptation using specialized datasets
- Retrieval-augmented generation with locally hosted models
- Hallucination reduction through verification prompts and structured workflows
- Uncertainty communication and confidence calibration
- Model behavior under incomplete, ambiguous, or conflicting information
- Tradeoffs among accuracy, latency, memory usage, and computational cost
- Human trust and decision-making when working with local language models

Each experiment should include:

- A clearly defined research question
- A testable hypothesis
- A baseline
- One or more experimental configurations
- Controlled variables
- Quantitative and qualitative evaluation criteria
- Reproducible training and inference settings
- Results and analysis
- Limitations and potential sources of bias
- Follow-up questions or proposed improvements

## Engineering Approach

The implementation will emphasize:

- Modular Python and PyTorch code
- Clear separation between reusable model code and experiments
- Automated tests
- Reproducible training runs
- Configuration-driven experiments
- Documented tensor shapes and model dimensions
- Meaningful version-control history
- Continuous integration
- Explicit architectural and training tradeoffs
- Honest reporting of failed experiments and limitations

## Planned Repository Structure

```text
my-llm-from-scratch-build/
├── src/
│   └── my_llm/
├── tests/
├── notebooks/
├── experiments/
├── configs/
├── scripts/
├── docs/
├── data/
├── models/
├── results/
├── .github/
│   └── workflows/
├── .gitignore
├── LICENSE
├── pyproject.toml
└── README.md
```

### Directory Responsibilities

- `src/my_llm/`: reusable model, training, inference, and evaluation code
- `tests/`: automated unit and integration tests
- `notebooks/`: exploratory analysis and visual explanations
- `experiments/`: experiment definitions and scenario-specific work
- `configs/`: reproducible model and training configurations
- `scripts/`: command-line training, evaluation, and inference scripts
- `docs/`: architecture notes, research plans, and technical documentation
- `data/`: local datasets or dataset instructions
- `models/`: locally generated model checkpoints
- `results/`: metrics, figures, tables, and experiment summaries

Large datasets and model checkpoints will generally not be committed to Git.

## Reproducibility

Each major experiment should record:

- Random seed
- Dataset and preprocessing version
- Model configuration
- Training configuration
- Hardware environment
- Dependency versions
- Evaluation procedure
- Saved metrics and outputs

Configuration files and scripts should make it possible to reproduce important results without relying on undocumented notebook state.

## Current Focus

The current phase is repository and development-environment setup.

The first implementation phase will focus on:

- Text preprocessing
- Tokenization
- Input-target generation
- PyTorch datasets and data loaders
- Tests for sequence construction and tensor shapes

## Attribution

This project is based on concepts and exercises from:

> Sebastian Raschka, *Build a Large Language Model (From Scratch)*, Manning Publications.

This is an independent educational and experimental implementation. It is not the official book repository and is not affiliated with Sebastian Raschka or Manning Publications.

Any code directly adapted from external sources will include appropriate attribution and license information.

## License

This project is licensed under the Apache License 2.0.
