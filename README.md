# AI Case Study – Regulatory Compliance Prototype

## Overview

This repository contains a GenAI-based prototype for regulatory compliance checking.

The solution extracts structured constraints from a municipal construction notice, evaluates them against a simplified ruleset, and generates a machine-readable compliance assessment.

## Task Objectives

1. Extract structured constraints from an unstructured municipal letter.
2. Evaluate the extracted constraints against a simplified ruleset.
3. Produce a machine-readable compliance assessment suitable for downstream automation and agent-based workflows.

## Solution Approach

The solution follows a hybrid LLM + Python architecture:

Municipal Letter  
→ LLM Constraint Extraction
→ Validation  
→ Rule Evaluation  
→ Compliance Assessment JSON

The LLM is used for information extraction, while compliance evaluation is implemented using deterministic Python logic to ensure explainability, reproducibility, and auditability.

## Repository Structure

```text
notebook/
└── case_study.ipynb

data/
├── Municipal_Letter.docx
└── Ruleset.docx

outputs/
├── extracted_constraints.json
└── validation_result.json

requirements.txt
README.md
```

## Main Components

- Constraint extraction using GPT-4o
- Structured JSON generation
- Pydantic schema validation
- Rule-based compliance evaluation
- Machine-readable compliance assessment

## Outputs

The notebook generates the following outputs:

- `extracted_constraints.json`
- `validation_result.json`

These outputs can be consumed by downstream automation workflows or AI agents.

## Running the Notebook

1. Install the required dependencies:

```bash
pip install -r requirements.txt
```

2. Configure the provided API credentials.

3. Execute the notebook from top to bottom.

