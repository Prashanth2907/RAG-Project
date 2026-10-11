# RAG-Based Question Answering with Chunking and Vector Search

## Project Overview

This project explores a Retrieval-Augmented Generation (RAG) system for answering questions using structured problem-and-solution data. It compares different chunking strategies and vector search techniques to retrieve relevant information and generate context-based answers.

## Objectives

- Implement and compare multiple chunking strategies.
- Retrieve relevant records using vector similarity search.
- Generate answers using a Large Language Model (LLM).
- Evaluate retrieval performance using Recall@K and Mean Reciprocal Rank (MRR).
- Assess generated answer quality using correctness and faithfulness scores.

## Technologies Used

- Python
- Pandas and NumPy
- Sentence Transformers
- FAISS
- Groq API
- Jupyter Notebook
- CSV and Excel

## Chunking and Retrieval Methods

The project compares five retrieval methods:

1. Fixed Chunking
2. Semantic Chunking
3. Recursive Chunking
4. Documentation-Based Chunking
5. Agentic Retrieval

## Dataset

The project uses an Excel dataset containing two main columns:

- `Problem`
- `Solution`

The dataset contains 86 records used for indexing, retrieval, and evaluation.

## Evaluation

The retrieval evaluation uses 10 dataset problem titles as test queries and compares the five retrieval methods.

Reported results:

- Recall@5: 100% for all five methods
- MRR: 1.00 for all five methods

**Note:** These results are based on queries matching existing dataset problem titles. They demonstrate retrieval performance for this test setup but do not establish generalization to independently phrased questions.

Answer quality is evaluated separately using reference solutions and correctness and faithfulness scores.

## Project Structure

```text
RAG-Chunking-Project/
├── RAG_Chunking_Project_Clean_Notebook.ipynb
├── Data.xml.xlsx
├── retrieval_evaluation_details.csv
├── retrieval_evaluation_summary.csv
├── answer_quality_evaluation.csv
├── requirements.txt
└── README.md
```

*The filenames above are examples; update them to match the files in your repository.*

## Setup and Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
   cd YOUR_REPOSITORY
   ```

2. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Configure your Groq API key as an environment variable. Do not publish API keys in the notebook or repository.

4. Open the Jupyter Notebook and run the cells in order.

## Future Improvements

- Expand the dataset and test questions.
- Evaluate retrieval using independently phrased questions.
- Improve answer-quality evaluation with additional metrics.
- Explore LLM-driven retrieval refinement.

## Author

Developed as a project on Retrieval-Augmented Generation, chunking strategies, and vector search.
