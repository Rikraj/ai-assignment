GENERAL-PURPOSE AI REASONING SYSTEM - README

1. PROJECT OVERVIEW
This repository contains a General-Purpose AI Reasoning System designed 
to seamlessly handle heterogeneous logical and causal modalities across 
multiple public benchmarks, including CounterBench (causal counterfactuals), 
RuleTaker (monotonic first-order logic rules), and FOLIO (first-order logic 
inference).

2. FILE STRUCTURE
* reasoning_agent.ipynb: Core General-Purpose Reasoning Engine implementation
	                 Main execution and benchmarking script that runs 
                         evaluations across datasets and outputs metrics.
* submission.csv   :     Generated prediction output file containing IDs and 
                         predicted labels.
* report.md        :     Comprehensive project report detailing representations,
                         algorithms, experiments, and reasoning traces.

3. PREREQUISITES & DEPENDENCIES
Ensure you have Python 3.8+ installed along with the required packages:
    pip install datasets z3-solver

4. HOW TO RUN
Execute the evaluation and benchmarking script:
    python evaluate.py

This script will automatically load the datasets, evaluate samples across 
the respective reasoners, print accuracy and inference times, and generate 
the `submission.csv` file.