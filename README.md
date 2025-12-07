Rating Prediction via Prompting

The project explores three different prompting strategies to classify Yelp reviews into 1–5 star ratings, using the Qwen/Qwen2.5-0.5B-Instruct LLM via the HuggingFace Inference API (free).
The entire workflow is implemented inside a single Jupyter notebook.

 🎯 Objective

Design and evaluate three prompting approaches for Yelp review rating prediction:
Zero-Shot Prompting
Few-Shot Prompting (with examples)
Rubric-Based Prompting (rule-driven)

Each LLM response must follow this JSON structure:
{
  "predicted_stars": <1–5>,
  "explanation": "Short reasoning"
}

🧪 Evaluation

A stratified sample of ~200 reviews from the Yelp dataset was used.
Metrics evaluated:
Accuracy
JSON validity rate
Mean Absolute Error (MAE)
Confusion matrices
Latency & consistency
Ensemble performance (bonus)

All results are stored in task1/results/.

🤖 Model Used

The project uses the Qwen/Qwen2.5-0.5B-Instruct model through the HuggingFace Inference API, which is:
Lightweight
Open-source
Fast
Free to use (no billing risk)

🚀 How to Run Locally

Install dependencies:
pip install -r requirements.txt

Set your HuggingFace API key in the notebook when prompted.
Launch the notebook:
jupyter notebook task1/notebooks/task1_notebook.ipynb

Run cells sequentially to:
Load data
Generate prompts
Call the model
Evaluate performance

📬 Contact
For issues or clarifications, feel free to open an issue on this repository.
