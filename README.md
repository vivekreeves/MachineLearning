# Machine Learning and LLM Project

## Folder Structure
- `data/`: Contains datasets.
- `notebooks/`: Contains Jupyter notebooks.
- `models/`: Contains saved models.
- `llms/`: Contains LLM-specific files:
  - `prompts/`: Prompt engineering files.
  - `fine_tuning/`: Scripts for fine-tuning LLMs.
  - `inference/`: Scripts for inference using LLMs.
  - `training/`: Scripts for training LLMs.
- `src/`: Contains source code for preprocessing, utilities, etc.

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd MachineLearning
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Mac/Linux
   venv\Scripts\activate     # On Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Running the Project
1. Open Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
2. Navigate to the `notebooks/` folder and open the desired `.ipynb` file.

## LLM Workflows
### Fine-Tuning
- Use scripts in `llms/fine_tuning/` to fine-tune LLMs on your dataset.
- Example:
  ```bash
  python llms/fine_tuning/fine_tune.py --data data/your_dataset.csv --model models/base_model.bin
  ```

### Inference
- Use scripts in `llms/inference/` for inference tasks.
- Example:
  ```bash
  python llms/inference/inference.py --model models/fine_tuned_model.bin --input llms/prompts/sample_prompt.txt
  ```

## Dependencies
See `requirements.txt` for the full list of dependencies.