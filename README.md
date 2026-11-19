# BPIC 2017 Process Analysis

This repository contains a reproducible process-mining analysis of the BPIC 2017 event log. All analysis and executable project code are in [`src/bpic2017_analysis.ipynb`](src/bpic2017_analysis.ipynb).

## Setup

Use Python 3.11 or 3.12. Install Graphviz separately and make sure its `dot` executable is on `PATH` so PM4Py can render Petri nets.

```powershell
cd assigment-1
py -3.12 -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
jupyter lab
```

Open `src/bpic2017_analysis.ipynb` and run all cells. Place the original event log at `data/BPI2017.xes`. On the first run, the notebook creates `data/BPI2017.parquet`; later runs use this cache when it is newer than the XES file. Put user-provided BPMN models in `data/bpmn/external/`.

## AI Assistance Disclosure

AI assistance was used to refactor and format the analysis notebook, organize the repository, and document the workflow.