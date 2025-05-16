🧠 GPT-2 Prompt Engineering Evaluation with BERTScore
Motivational Text Generation in the Style of A Song of Ice and Fire

📜 Overview
This project explores prompt engineering techniques for generating motivational quotes using the GPT-2 language model, evaluated via BERTScore for semantic similarity to human-written references. The prompts and references are inspired by the lore and language of A Song of Ice and Fire, aiming to capture the tone of iconic characters like Jon Snow, Daenerys Targaryen, and Tyrion Lannister.

By comparing different prompt styles (e.g., direct, scenario-based, persona-based), this project investigates how input phrasing influences the quality of the generated text. It provides both quantitative and qualitative analysis through textual metrics, tables, and visualizations.

🚀 Features
🔁 Multiple Prompt Types: Explore how Direct, Persona-based, Conversational, and Keyword-driven prompts affect GPT-2 output.

🧠 Semantic Evaluation with BERTScore: Quantify how close GPT-2 outputs are to human-written references.

📊 Length & Word Count Metrics: Track structural differences between generated and reference texts.

📈 Data Visualization: Beautiful plots comparing prompt effectiveness.

💾 Result Export: Save raw outputs and summaries for reuse or publication.

🧪 Prompt Types Used
Prompt Type	Description
Direct	Simple, imperative style prompts
Scenario-based	Hypothetical situations to trigger narrative generation
Persona-based	Role-play style prompts imitating a character's worldview
Keyword-based	Force specific vocabulary within a character's context
Conversational	Simulated dialogue between user and assistant in-character

🛠️ Tech Stack
Language Model: GPT2LMHeadModel from Hugging Face Transformers

Tokenizer: GPT2Tokenizer

Evaluation Metric: BERTScore (Precision, Recall, F1)

Data Handling: pandas

Visualization: matplotlib, seaborn

Execution: Jupyter Notebook / Python script

📂 Project Structure
📦 gpt2-prompt-evaluation
├── 📓 notebook.ipynb                   # Jupyter Notebook version
├── 📊 gpt2_prompt_engineering_results.csv  # All generated outputs and scores
├── 📈 gpt2_prompt_type_summary.csv         # Aggregated summary by prompt type
└── 📄 README.md                        # You're reading it!
🧬 Workflow Summary
Load GPT-2 Model

Loads pretrained model and tokenizer with GPU acceleration.

Generate Text

Creates 3 variations per prompt using temperature sampling and beam constraints.

Post-Processing

Trims incomplete sentences and cleans output.

Evaluate with BERTScore

Compares generated text to human references using semantic similarity.

Compute Metrics

Includes length and word count ratios.

Visualize & Export

Bar plots, boxplots, and CSV exports of results.

📊 Sample Output Comparison
Prompt Type	Model Output (Example)	Human Reference
Persona-based	“I walked through fire and came out steel. You can too. Rise with fury, not fear.”	“I was born in a storm... know that you have the strength to rise from the ashes of failure.”

📈 Key Findings
Persona-based prompts often yield the most stylistically aligned and coherent outputs.

Keyword-based prompts offer more control but risk reducing natural fluency.

Conversational prompts increase emotional relatability.

📥 Installation
# Create a virtual environment (optional but recommended)
python -m venv env
source env/bin/activate  # or env\Scripts\activate on Windows

# Install required packages
pip install torch transformers bert_score pandas matplotlib seaborn
▶️ How to Run
Open the notebook or run as a Python script:
# Jupyter Notebook
jupyter notebook notebook.ipynb

📌 Requirements
Python 3.7+

PyTorch with CUDA support (for GPU acceleration)

Hugging Face Transformers

BERTScore

pandas, matplotlib, seaborn

🔍 Possible Extensions
🔁 Fine-tune GPT-2 on fantasy literature for even better stylistic mimicry.

🧑‍⚖️ Human Evaluation: Add human raters to assess emotional resonance.

📚 Train a classifier to predict prompt type effectiveness based on linguistic features.

🌍 Try multilingual or translated prompts with mBERTScore.

✍️ Acknowledgements
Inspired by the literary world of A Song of Ice and Fire by George R. R. Martin.

GPT-2 and evaluation tools powered by Hugging Face and BERTScore.








