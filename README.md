# OpNote-AE: Automated Detection of Intraoperative Adverse Events from Spine Operative Notes

## Overview

This repository contains code for automated detection of intraoperative adverse events from spine surgery operative reports using a large language model (GPT-4).

The system identifies:

- Incidental (unplanned) durotomy  
- Non-durotomy intraoperative adverse events  

This code accompanies the manuscript:

**"GPT-4-Assisted Detection of Intraoperative Adverse Events from Spine Surgery Operative Reports: A Comparison with Human Reviewers"**

---

## Requirements

Python 3.9 or higher

Install dependencies:

pip install -r requirements.txt

---

## API Access

This project requires access to the OpenAI or Azure OpenAI API.

Set your API key:

export OPENAI_API_KEY=YOUR_API_KEY

---

## Data

Real operative notes cannot be shared due to patient privacy restrictions.

A synthetic example dataset is provided:

data/sample_notes.csv

Users may substitute their own dataset in the same format.

---

## Running the Pipeline

python src/run_pipeline.py --input data/sample_notes.csv --output results/predictions.csv

---

## Output

The pipeline outputs:

- Durotomy classification (0/1)
- Adverse event classification (text descriptor)

---

## License

MIT License
