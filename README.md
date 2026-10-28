# Baseball Strategy Agent
**Ospanov Dayan | 23B030308 | CSCI3235 Midterm I**

This compact project contains:

- `baseball_agent.ipynb`: all environment, SARSA, baseline, experiment and plot code,
  with saved outputs and explanations.
- `report.pdf`: report and a one-page learning-record section.
- `README.md`: these run instructions.
- `requirements.txt`: Python dependencies.

## Run
Create an environment from the repository root and install the dependencies:

```text
python -m venv .venv
.venv\Scripts\python -m pip install -r requirements.txt
```

On macOS/Linux, use `.venv/bin/python` for the second command.
Open `baseball_agent.ipynb`. In VS Code, choose **Select Kernel > Python
Environments > .venv**, then **Run All**.

Run the notebook from top to bottom. Allow about 10-30 seconds on a typical
laptop. Python 3.11 or later is recommended; the supplied notebook was run on
Python 3.14.7. It does not read the old project's files or require any datasets.
The notebook itself produces no extra files or folders.

## Experiment
Five seeds: 42, 123, 456, 789, 2026. Each agent trains for 10,000 at-bats.
Final evaluation uses 10,000 fresh at-bats per seed and policy. SARSA uses
alpha=0.1, gamma=1 and main epsilon=0.2; sensitivity settings are 0.05 and 0.5.
The notebook reports every seed, the mean and sample standard deviation.

The code cells contain no comments; explanations are in Markdown cells.
All results and figures are saved in the notebook. The report includes your
reflection and the completed AI-assisted two-strike foul check. Its executable
assertion and passing output are saved in the notebook.

## Work and assistance
I completed the experiments, analysis, report and learning reflection. OpenAI
Codex helped with the Python implementation, testing and debugging, and provided
initial project drafts. I reviewed and revised the material and take responsibility
for the final work.
