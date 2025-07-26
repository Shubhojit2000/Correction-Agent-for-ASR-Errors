# 🔧 Correction Agent for ASR Errors

This project implements a phoneme-based correction agent to improve the outputs of Automatic Speech Recognition (ASR) systems. It uses a beam search strategy to explore possible sentence alternatives and leverages OpenAI's Whisper model to evaluate the cost (loss) of each candidate correction.

---

## 📁 Project Structure

```plaintext
Correction-Agent-for-ASR-Errors/
├── DATA/                    # Input audio and metadata
├── RESULTS/                 # Output corrections and evaluation results
├── col671-a1.ipynb          # Main Jupyter Notebook (Core logic)
```

---

## 🚀 Features

- ✅ Uses **Whisper Small (English)** model as a cost evaluator.
- ✅ Implements a **beam search** agent for error correction.
- ✅ Supports **phoneme substitution**, **insertion**, and **deletion** based on a configurable phoneme table.
- ✅ Evaluates performance based on **cost reduction** and provides visual insights.
- ✅ Outputs both summary statistics and correction results in `.json` format.

---

## 📦 Dependencies

Make sure the following Python packages are installed:

```bash
pip install torch transformers jiwer pandas seaborn matplotlib
