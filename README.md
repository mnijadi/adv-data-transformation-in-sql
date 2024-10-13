# Advanced SQL Data Transformations

## Setup

You have two options to run the exercises in this repo

### Option 1: Github codespaces (Recommended)

Steps:

1. Create [Github codespaces with this link](https://github.com/codespaces/new?skip_quickstart=true&machine=basicLinux32gb&repo=833339774&ref=main&geo=UsEast).
2. Wait for Github to install the [requirements.txt](./requirements.txt). This step can take about 5minutes.
        ![installation](./images/inst.png)
3. In the terminal run `python setup.py` to create the tables and data necessary for the exercises.
4. Now open the `0-basics.ipynb` (or any ipynb) and it will open in a Jupyter notebook interface. You will be asked for your kernel choice, choose `Python Environments` and then `python3.10.13 Global`.
        ![Jupyter notebook in VScode](./images/vsjupy.png)

### Option 2: Run locally

Steps:

1. Clone this repo, cd into the cloned repo
2. Start a virtual env and install requirements.
3. In the terminal run `python setup.py` to create the tables and data necessary for the exercises.
4. Start Jupyter lab and run the `ipynb` notebooks.

```bash
# clone repo then cd to repo folder
python -m venv ./env # create a virtual env
source env/bin/activate # use virtual environment
pip install -r requirements.txt
python setup.py
jupyter lab
```

## Data Model

The TPC-H data represents a car parts seller’s data warehouse, where we record orders, items that make up that order (lineitem), supplier, customer, part (parts sold), region, nation, and partsupp (parts supplier). 

Note: Have a copy of the data model as you follow along; this will help in understanding the examples provided and in answering exercise questions.

![](./tpch_erd.png)

## Topics covered in the workshop

1. Window functions
2. CTEs
3. Common query templates for common data processing problems
