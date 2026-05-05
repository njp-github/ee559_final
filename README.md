# ee559_final
Code and instructions to run scripts for EE 559 (Sp2026) Final Project by Rama Chandra Bhogasamudram and Neil Patel.

To run in a Linux environment-

To run in a Windows environment (VS Code)-
- Create a virtual environment (preferably Python 3.12) - python -m venv .venv
- Activate environment - .venv\Scripts\activate
- Install Jupyter + basics - pip install notebook ipykernel numpy pandas matplotlib
- Register it as a Jupyter Kernal - python -m ipykernel install --user --name=age-env --display-name "Python (age-env)"
- In VS Code, open notebook, click Kernal Picker (top-right) and select "age-env"
- To de-activate environment - deactivate
- To choose the right interpreter - Press "Ctrl+Shift+P" and select Python 3.12 and choose your ".venv"

Make sure the path to the data files is correct in the code (Cell 1 - Imports & Setup).
