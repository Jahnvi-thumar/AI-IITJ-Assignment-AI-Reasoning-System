AI Assignment

Overview

This project implements a Python-based AI reasoning system that converts supported natural-language facts and rules into a logical representation. It uses unification and forward chaining to derive conclusions and answer True/False queries.

Dependencies

The reasoning engine requires the following libraries:

- pandas
- datasets
- huggingface_hub
- tqdm

Install them using:

pip install datasets huggingface_hub pandas tqdm

Execution Instructions

1. Open `assignment.ipynb` in Jupyter Notebook or Google Colab.
2. Run all cells from top to bottom.
3. The notebook downloads the public development datasets, evaluates the reasoning engine, and displays reasoning traces and evaluation metrics.
4. The notebook also generates public diagnostic CSV files.

Implemented Reasoning Methods

- Knowledge Representation: Facts and rules are stored using logical literals and rule structures.
- Unification:Matches variables in rules with known facts.
- Forward Chaining: Derives new facts by repeatedly applying rules.
- Query Evaluation: Checks whether a query can be derived from the knowledge base.

Dataset Experiments

The notebook includes:

- RuleTaker: Evaluation of the forward-chaining reasoning engine.
- FOLIO: Binary evaluation, excluding Uncertain examples.
- CounterBench: Dataset loading and structural inspection.

CounterBench is inspected for dataset structure; no reasoning accuracy is reported for it.

Limitations

The natural-language parser supports a limited set of sentence patterns. More complex sentences and logical constructions may be unsupported or incorrectly interpreted.

Output

The notebook displays evaluation metrics, inference traces, and generates CSV output for the public RuleTaker development evaluation.

The generated public CSV is for demonstration and diagnostic purposes; it is not a private-test submission.
