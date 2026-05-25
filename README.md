# Topic_Modeling
Advanced Data Analysis Project (DLBDSEDA02)

## Project Description
...

### Repository Structure
There are four Jupyter notebooks, one containing the preprocessing code and 3 containing a topic modeling method each.
The repository contains the following folders:

```bash
.
├── notebooks    # Notebooks containing analysis code
├── data         # Raw data (input) and cleaned data (file too big for Github upload)
├── topics       # CSV files containing the top words for each topic
├── viz          # Visualizations of topic space/ distribution and evaluation metrics
└── README.md
```

## Setup & Execution
Run the following commands in the terminal to setup the virtual environment and install necessary dependencies:

### Create & Activate Virtual Environment (Windows)
```
.venv/
.venv\Scripts\activate
```
### Install Jupyter Kernel & Depedencies
```
python -m pip install jupyter ipykernel
pip install -r requirements.txt
python -m spacy download en_core_web_sm
```
### Run Notebooks
First run the preprocessing notebook: [Preprocessing.ipynb](Preprocessing.ipynb).

The order of the other notebooks does not matter. Each notebook includes a standalone analysis with a different topic modeling method:
* [LDA with BoW vectorization](Topic_Modeling_LDA.ipynb)
* [NMF with TFIDF vectorization](Topic_Modeling_NMF.ipynb)
* [BERTopic with BoW vectorization](Topic_Modeling_BERTopic.ipynb)