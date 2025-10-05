# Python Fundamentals — Zero to Mastery Notebook

This Jupyter notebook covers all topics taught during the exclusive IEEEXTREME 19.0 training session "Python: Zero to Mastery", delivered as part of Informatyka 5.0 by IEEE CS SBC RIT and IEEE CS SBC CE Kidangoor in collaboration with the IEEE Computer Society Kerala Section. The workshop was conducted online on 4th and 5th October 2025 from 7:00 PM to 9:00 PM.

## What this notebook is

This notebook is a day-by-day walkthrough of core Python fundamentals. It mixes explanatory markdown with runnable Python code cells that demonstrate concepts and print example outputs. The content includes examples you can run and modify directly in a Jupyter environment or VS Code.

## Table of contents

All links point to headings inside the Jupyter notebook `ZerotoMastery_PythonFundamentals.ipynb` (open the notebook and click the links below to jump to that section):

| Section                                                                                                                                  |
| ---------------------------------------------------------------------------------------------------------------------------------------- |
| [Structure of a Python Program](ZerotoMastery_PythonFundamentals.ipynb#structure-of-a-python-program)                                    |
| [Variables and Data Types](ZerotoMastery_PythonFundamentals.ipynb#variables-and-data-types)                                              |
| [Keywords](ZerotoMastery_PythonFundamentals.ipynb#keywords)                                                                              |
| [Mutable vs Immutable types](ZerotoMastery_PythonFundamentals.ipynb#mutable-and-immutable-data-types)                                    |
| [Operators](ZerotoMastery_PythonFundamentals.ipynb#operators-and-operands)                                                               |
| [Input and Output](ZerotoMastery_PythonFundamentals.ipynb#input-and-output)                                                              |
| [Comments and docstrings (Single-line / Multi-line)](ZerotoMastery_PythonFundamentals.ipynb#comments-in-python)                          |
| [Flow of execution (Sequential / Conditional Statements / Looping Constructs)](ZerotoMastery_PythonFundamentals.ipynb#flow-of-execution) |
| [Strings (Operations / Slicing / Methods)](ZerotoMastery_PythonFundamentals.ipynb#strings)                                               |
| [Lists (Operations / Slicing / Methods)](ZerotoMastery_PythonFundamentals.ipynb#lists)                                                   |

## How to clone the repository and run

To run the notebook inside Visual Studio Code, follow these steps. This guide assumes you have Git and Python installed; if not, install them first:

- Git for Windows: https://git-scm.com/download/win
- Python (3.8+): https://www.python.org/downloads/

1. Clone the repository (HTTPS) and open it in VS Code:

```powershell
git clone https://github.com/ellen-rose-james/python-fundamentals-course.git
cd python-fundamentals-course
code .
```

2. Install the recommended VS Code extensions (from the Extensions view or follow the links below):

- Python — Microsoft (ms-python.python): https://marketplace.visualstudio.com/items?itemName=ms-python.python
- Jupyter — Microsoft (ms-toolsai.jupyter): https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter

3. Create a virtual environment (from the VS Code integrated terminal) and install kernel support:

```powershell
python -m venv .venv

# Activate the venv in the integrated terminal (PowerShell):
.\.venv\Scripts\Activate.ps1

# Install required packages (Jupyter and ipykernel allow the venv to be selected as notebook kernel):
python -m pip install --upgrade pip

pip install jupyter ipykernel

python -m ipykernel install --user --name=python-fundamentals-venv --display-name "Python (python-fundamentals-.venv)"
```

4. Select the interpreter / kernel in VS Code:

- Press `Ctrl+Shift+P` > `"Python: Select Interpreter"` > choose the `.venv` interpreter you created. This sets the interpreter for the workspace.
- Open the notebook file `ZerotoMastery_PythonFundamentals.ipynb`. In the top-right of the notebook editor choose the kernel dropdown and select the kernel named `"Python (python-fundamentals-.venv)"` or the `.venv` interpreter.

5. Run the notebook:

- Use the play buttons on each cell, or use the "Run All" command in the notebook toolbar to execute all cells.
- Cells that use `input()` will prompt in the notebook UI.

Troubleshooting tips

- If the `.venv` interpreter doesn't appear in the list, restart VS Code and try "Python: Select Interpreter" again.
- If a notebook cell errors due to a missing package, install it in the activated virtual environment (e.g., `pip install <package>` in the integrated terminal) and re-run the cell.
- To remove the temporary kernel created with `ipykernel`, run `jupyter kernelspec list` to find the kernel path and `jupyter kernelspec remove <kernel-name>` to delete it.

## Notes

- Some cells use `input()` to demonstrate interactive input; avoid running those cells in automated environments unless you supply input.
- Cells are independent examples; you can modify variable names and rerun to see different behaviour.
