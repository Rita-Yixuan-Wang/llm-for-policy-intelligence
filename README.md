# Few-Shot LLM-Based Policy Text Classifier

This project demonstrates how to use GPT-4 with few-shot prompting to classify U.S. policy statements by their relevant industry sectors. It is designed to be a lightweight, no-training-required prototype for consulting, research, and regulatory analysis tasks.

![OpenAI](https://img.shields.io/badge/LLM-GPT--4-blue)
![Python](https://img.shields.io/badge/Python-3.8+-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Status](https://img.shields.io/badge/Project-Demo--Ready-blueviolet)

---

## 🚀 Overview

**Goal:**  
Automatically assign industry labels (e.g., Energy, Finance, Education) to policy texts using GPT-4.

**Method:**  
Few-shot learning (in-context classification using prompt examples)

**Tools:**  
Python, OpenAI API, Pandas

**Dataset:**  
10 synthetic U.S. policy statements covering multiple federal agencies and industries

---

## 🧠 Why This Matters

Policy analysts, consultants, and business strategists often need to monitor large volumes of policy updates. Manual classification is time-consuming.  
This project shows how LLMs can be used out-of-the-box to:

- Identify regulatory risks and opportunities by industry  
- Route policy updates to relevant internal teams (e.g., Energy, Labor)  
- Quickly prototype NLP pipelines without labeled datasets or ML training

---

## 🛠️ How It Works

1. A small number of labeled examples are written in the prompt  
2. The model is prompted with new policy statements  
3. GPT-4 predicts the most relevant industry  
4. Results are stored in a CSV file

---

## 🧾 Example Output

| Policy Snippet                                      | Predicted Industry       |
|-----------------------------------------------------|--------------------------|
| FAA increases drone cybersecurity standards         | Transportation           |
| DOE funds small nuclear reactor projects            | Energy                   |
| USDA subsidizes organic agriculture                 | Agriculture              |
| Labor Dept proposes warehouse worker protections    | Labor & Employment       |

✅ *Accuracy: 100% in a 10-sample test set (manually reviewed)*

---

## 📁 Project Structure

```text
llm-policy-classifier/
├── data/
│   └── classified_policies.csv     # Output predictions
├── src/
│   └── classify_with_gpt.py        # Main classification script
├── reports/
│   └── final_report.pdf            # Full analysis and results
├── README.md                       # Project overview (this file)
```

---

## 📈 Possible Extensions

This project can be extended in several ways:

- 🧠 Fine-tune BERT or LLaMA for more robust domain-specific classification  
- 📚 Use RAG (Retrieval-Augmented Generation) to enhance prediction quality on ambiguous or long policy texts  
- 📊 Build a Streamlit UI for interactive input/output and result visualization  
- 🧮 Scale to real datasets with 1,000+ policies from public government or regulatory sources

