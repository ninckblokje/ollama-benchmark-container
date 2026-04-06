# ollama-llm-benchmark

Docker container for benchmaring ollama with [LLM:Benchmark](https://llm.aidatatools.com/).

Available tags for `linux/amd64` and `linux/arm64`:
- `cpu`: Runs ollama on the CPU

## Prompts

1. Summarize the key differences between classical and operant conditioning in psychology.
2. Translate the following English paragraph into Chinese and elaborate more -> Artificial intelligence is transforming various industries by enhancing efficiency and enabling new capabilities.
3. What are the main causes of the American Civil War?
4. How does photosynthesis contribute to the carbon cycle?
5. Develop a python function that solves the following problem, sudoku game.

## Results

| Platform | Tag | Model | Average TOPS | Prompt 1 TOPS | Prompt 2 TOPS | Prompt 3 TOPS | Prompt 4 TOPS | Prompt 5 TOPS |
|--|--|--|--|--|--|--|--|--|
| Raspberry Pi 5 8 GB RAM | cpu | qwen2:1.5b | 10.892 | 11.82 | 9.70 | 11.06 | 11.13 | 10.75 |
| Raspberry Pi 5 8 GB RAM | cpu | llama3.2:3b | 4.246 | 4.28 | 4.25 | 4.33 | 4.11 | 4.26 |
| Intel® Core™ i7-8550U × 8 24 GB RAM | cpu | qwen2:1.5b | 16.2 | 15.90 | 17.60 | 15.78 | 15.94 | 15.78 |
| Intel® Core™ i7-8550U × 8 24 GB RAM | cpu | llama3.2:3b | 7.896 | 8.08 | 8.11 | 7.63 | 7.92 | 7.74 |