# 🧪 Testing Shell Guide

This guide explains how to run interactive testing for the AI Text Classification & Summarization project.

## 🔹 Manual Testing
Run the notebook cell with the manual shell. Available commands
- `examples` → Show predefined test cases
- `stats` → Show session statistics and model accuracy
- `history` → Show last 5 classification results
- `clear` → Reset session data
- `quit` → Exit testing session

## 🔹 Batch Testing
To test the entire dataset
```python
results = [llm.invoke(text) for text in df['text']]
