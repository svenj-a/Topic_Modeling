# Topic_Modeling
This repository contains a data analysis project applying topic modeling techniques to a collection of Reddit posts from r/askScience.

## Project Description (Fictional Use Case)
Many public concerns, especially regarding science-related policies like climate change or public healthcare, are shaped by gaps in understanding or misinformation. To better address these challenges, a municipality aims to improve science communication and public engagement strategies. Since younger citizens are often underrepresented in traditional feedback and participation channels, the municipality additionally analyzes social media posts where users ask questions and express curiosity or confusion about scientific topics. By identifying trending and recurring topics, the municipality can design targeted science and education campaigns, improve public communication on policy decisions, and proactively address knowledge gaps before they turn into dissatisfaction or resistance. In this project usergenerated content from Reddit, specifically posts from r/AskScience, are analyzed as a proxy for the questions and interests of a digitally active population. By extracting and structuring insights from unstructured text data, the municipality aims to inform targeted science communication and education campaigns that align more closely with the needs and concerns of a younger audiences.

## Repository Structure
There are three Jupyter notebooks, one containing the preprocessing code and two containing topic modeling methods.
The repository contains the following items:

```bash
.
├── notebooks (files)           # Notebooks containing analysis code
├── data (folder)               # Raw data (input) and cleaned data (files too big for Github upload, added to gitignore)
├── topics (folder)             # CSV files containing the top words for each topic
├── viz (folder)                # Visualizations of topic space/ distribution and evaluation metrics
├── requirements.txt (file)     # Lists all required dependencies with the version used for development
└── README.md (file)            # You are here.
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
