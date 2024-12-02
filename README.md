# Binary Classification of Populist Speech

## Project Overview
This project focuses on the classification of speeches as either populist or non-populist using fine-tuned pre-trained language models. We evaluated four models—BERT-tiny, BERT-large, GPT-2, and RoBERTa-large—on a dataset of 500 manually labeled speeches. The best performing model, **RoBERTa-large**, achieved an accuracy of **88%**, demonstrating its effectiveness for this task.

## Models Evaluated
- **BERT-tiny** (Google)
- **BERT-large** (Google)
- **GPT-2** (OpenAI)
- **RoBERTa-large** (Facebook AI)

Each model was fine-tuned using pre-processed speeches, tokenized to fit the input structure of the model, and evaluated based on accuracy and loss metrics.

## Dataset
The dataset contains **500 speeches**, equally split between populist and non-populist categories, manually labeled by the contributors. The speeches were collected via web scraping and include translated texts from various languages, further enriching the diversity of the data.

## Running the Code
The project code was primarily run on **Google Colab** using a high-RAM **A100 GPU**, which allowed for:
- Batch size of 128 for **BERT-tiny**
- Batch size of 20 for the larger models

The code can be run all together with no issues given the right GPU and Database path. Replicating these results on Colab is straightforward, though smaller GPUs or CPUs will require a reduction in batch size:
- Batch size of 8 for single-model runs
- Batch size of 2-4 for running all models simultaneously

## Results
- **RoBERTa-large**: Best model with an accuracy of **88%**.
- **BERT-large**: Accuracy of **71%**.
- **GPT-2**: Accuracy of **61%**.
- **BERT-tiny**: Accuracy of **59%**.

For more details on the performance and methodology, please refer to the **Experiments and Results** section in the report.



## How to Use the Code
1. Clone this repository.
2. Ensure that you have **PyTorch**, **transformers**, and the necessary libraries installed.
3. Set up your environment with a **high-memory GPU** for best performance, or adjust the batch size as outlined above.
4. Run the code using the provided scripts, ensuring you specify the correct **database path**.

For further details on implementation, refer to the documentation within the scripts.

## Contributors
- **Alessandro Pala**
- **Lorenzo Cino**
- **Greta Grelli**
- **Alberto Calabrese**
- **Giacomo Filippin**

<p>
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white&style=plastic" height="25"/>
  <img alt="Jupyter" src="https://img.shields.io/badge/Jupyter-F37626?logo=Jupyter&logoColor=white&style=plastic" height="25"/>
  <img alt="Visual Studio Code" src="https://img.shields.io/badge/Visual Studio Code-007ACC?logo=VisualStudioCode&logoColor=white&style=plastic" height="25"/>
</p>
