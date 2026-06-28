# LLM Inference Playground using GPT-2

A hands-on notebook that explores how decoder-only Large Language Models (LLMs) generate text. This project walks through the complete inference pipeline—from raw logits to different decoding strategies—and concludes with an interactive Streamlit playground for experimenting with generation parameters.

---

# What You'll Learn

This notebook covers the core concepts behind LLM inference:

- GPT-2 inference pipeline
- Next-token prediction
- Logits and probability distributions
- Softmax implementation
- Greedy decoding
- Beam Search
- Temperature Sampling
- Top-K Sampling
- Top-P (Nucleus) Sampling
- Interactive LLM inference using Streamlit

---

# Notebook Contents

## 1. GPT-2 Model Loading

Load the GPT-2 Medium model and tokenizer using Hugging Face Transformers.

Topics covered:

- Decoder-only Transformers
- Tokenization
- Model loading
- Text generation

---

## 2. Next Token Prediction

Inspect how GPT-2 predicts the next token by:

- Computing logits
- Applying Softmax
- Displaying the Top-5 predicted tokens and their probabilities

Example:

```
Prompt:
Narendra Modi is the prime

Top Predictions:

minister
ministerial
...
```

---

## 3. Softmax Implementation

A manual implementation of the Softmax function to understand how raw logits are converted into probabilities.

Topics:

- Logits
- Exponentiation
- Probability normalization
- Why probabilities sum to 1

---

## 4. Decoding Strategies

Explore different decoding algorithms used during text generation.

### Greedy Search

Always selects the highest-probability token.

### Beam Search

Maintains multiple candidate sequences to improve overall generation quality.

### Temperature Sampling

Controls randomness during generation.

- Low Temperature → More deterministic
- High Temperature → More diverse

### Top-K Sampling

Samples only from the K most probable tokens.

### Top-P (Nucleus) Sampling

Samples from the smallest set of tokens whose cumulative probability exceeds a threshold **P**.

---

# LLM Inference Playground

The notebook also includes a Streamlit application (`app.py`) for interactively experimenting with GPT-2 inference.

## Features

- Prompt input
- GPT-2 model selection
- Temperature control
- Top-K control
- Top-P control
- Maximum New Tokens
- KV Cache toggle
- Input token count
- Output token count
- Total token count
- Inference latency
- Side-by-side temperature comparison
- Top-5 next-token probability visualization

---

# Concepts Covered

- Decoder-only Transformers
- Tokenization
- Next-token prediction
- Logits
- Softmax
- Probability distributions
- Greedy Search
- Beam Search
- Temperature Sampling
- Top-K Sampling
- Top-P Sampling
- Autoregressive Generation
- KV Cache
- Inference latency

---

# Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- Streamlit
- NumPy

---

# Running the Notebook

Install the required packages:

```bash
pip install torch transformers streamlit numpy
```

Open:

```
llm-inference-playground.ipynb
```

Run the notebook sequentially to explore each concept.
---

# Learning Outcomes

After completing this notebook, you will understand:

- How GPT models generate text token-by-token
- How logits become probabilities using Softmax
- The differences between Greedy Search, Beam Search, Temperature, Top-K, and Top-P Sampling
- How decoding parameters influence generated text
- How to inspect next-token probabilities
- How to build an interactive LLM inference application with Streamlit

---

# Author

**Sukumaran S.**

AI/ML Engineer | Generative AI | LLM Engineering | RAG Systems

---

⭐ If you found this notebook useful, consider giving the repository a star.
