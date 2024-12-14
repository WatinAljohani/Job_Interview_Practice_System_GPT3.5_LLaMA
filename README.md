# Job Interview Practice System

This project demonstrates the fine-tuning of advanced language models, *GPT-3.5-Turbo* and *LLaMA*, on a dataset of job interview questions and answers tailored for software engineering roles. The goal is to build a conversational AI system capable of simulating realistic job interviews while evaluating technical and soft skills.

---

## Features
- *Fine-Tuning GPT-3.5 and LLaMA*: Both models are fine-tuned to generate domain-specific responses to interview questions.
- *Dataset Preparation*: Includes data cleaning, tokenization, and structuring for Natural Language Processing (NLP) tasks.
- *Performance Metrics*: Evaluates models using ROUGE and BERTScore metrics before and after optimization.
- *Model Optimization*: Implements optimization techniques to enhance performance.

---


## Installation

### Prerequisites
Ensure you have Python 3.7 or later installed. You also need `pip` to install the required packages.

### Steps
1. Clone this repository:
   ```bash
   git clone https://github.com/YourUsername/Job_Interview_Practice_System.git
   cd Job_Interview_Practice_System
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up the fine-tuning dataset in the appropriate format (e.g., JSONL).

4. Update the `openai.api_key` placeholder in the code to your own API key:
  ```python
  openai.api_key = "YOUR_API_KEY"
  ```

## Usage

1. **Fine-Tuning the Models**:
   - Fine-tune GPT-3.5 using the OpenAI API.
   - Fine-tune LLaMA using LoRA (Low-Rank Adaptation) for resource-efficient training.

2. **Running the System**:
   Execute the provided notebook or scripts to generate questions and feedback:
   ```bash
   python main.py
   ```

3. **Evaluating Performance**:
   - Metrics used include ROUGE (ROUGE-1 and ROUGE-L) and BERTScore.
   - Visualizations for performance comparison are included in the notebook.

## Dataset Description
- **Source**: The dataset was initially sourced from ([Kaggle](https://www.kaggle.com/datasets/syedmharis/software-engineering-interview-questions-dataset)) and refined to support two different conversational models, GPT and LLaMA.
- **Structure**:
  - **GPT Dataset**: Conversational flow with roles (`system`, `user`, `assistant`).
  - **LLaMA Dataset**: Instruction-response pairs.
- **Size**: 50 refined records in JSONL format.


## Workflow
1. Data Preparation:
- Load and clean the dataset.
- Tokenize and structure data for NLP tasks.
2. Model Fine-Tuning:
- Train GPT-3.5-Turbo and LLaMA on the curated dataset.
- Apply parameter-efficient fine-tuning techniques (LoRA) for LLaMA.
3. Evaluation:
- Compute performance metrics using ROUGE and BERTScore.
- Compare model performance before and after optimization.
4. Analysis:
- Visualize performance metrics and analyze trends.

  
## Key Files
1- FineTuning_GPT3.5_LLaMA_JobInterview.py:
Contains the code for data preparation, fine-tuning, evaluation, and visualization.

2- Dataset Files:
- Software_Questions_GPT.jsonl: Dataset for GPT-3.5 fine-tuning.
- Software_Questions_LLaMA.jsonl: Dataset for LLaMA fine-tuning.

## Limitations
- Performance may vary with different datasets or hyperparameters.
- LLaMA requires significant computational resources for training and fine-tuning.

## Future Work
- Explore domain-specific optimizations for additional technical fields.
- Integrate real-time evaluation capabilities for user feedback.

---

## Project Contributions
  - Watin Aljohani
  - Munirah Almutlaq
  - Joud Aldhuwaihi
  - Fatimah Albuainain
  - Mayyan Alharbi

