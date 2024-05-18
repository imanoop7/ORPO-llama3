# Fine-Tuning Llama 3 with ORPO

Welcome to the **Fine-Tuning Llama 3 with ORPO** repository! In this project, we explore a novel fine-tuning technique called ORPO (Odds Ratio Preference Optimization) for adapting the Llama 3 language model to specific tasks. ORPO combines supervised fine-tuning and preference alignment into a single training process, reducing computational resources and training time.

## What is ORPO?

- **ORPO (Odds Ratio Preference Optimization)**: ORPO modifies the standard language modeling objective by adding an odds ratio (OR) term to the loss function. It weakly penalizes rejected responses while strongly rewarding preferred ones, allowing the model to learn the target task and align with human preferences in a single step.

## Article- https://medium.com/@mauryaanoop3/fine-tuning-llama-3-with-orpo-a-deep-dive-1452bc1b1838
## Repository Structure

- `ORPO_finetuning.ipynb`: A Jupyter Notebook demonstrating how to fine-tune Llama 3 using ORPO. The notebook covers environment setup, model training, evaluation, and deployment.
- `benchmark_results/`: Detailed results of benchmark evaluations (e.g., eqbench and truthfulqa). Note that we used a small dataset (1000 samples) for demonstration purposes.
- `LICENSE.md`: MIT license information for this repository.

## Getting Started

1. Clone this repository.
2. Set up the required compute environment (Nvidia GPU with >=24GB VRAM).
3. Run the `ORPO_finetuning.ipynb` notebook to fine-tune Llama 3 with ORPO.
4. Evaluate the model's performance using benchmark metrics.
5. Deploy the fine-tuned model for your specific use case.

## Model Details

- **Llama 3**: The latest family of large language models developed by Meta. Two model sizes are available: a 70 billion parameter model and a smaller 8 billion parameter model.
- **Performance**: The 70B model achieved impressive scores on benchmarks (e.g., 82 on MMLU and 81.7 on HumanEval).
- **Context Length**: Llama 3 models support up to 8,192 tokens context length (potentially scaling up to 32k with RoPE).
- **Tokenizer**: Uses a new tokenizer with a 128K-token vocabulary, reducing the number of tokens required for encoding text.

Feel free to explore and adapt this repository based on your specific tasks. Happy fine-tuning! 🚀🤖

