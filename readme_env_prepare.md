Set up your conda environment:

    download and install miniconda
    restart your terminal
    create an environment with 'conda create -y -n mlpc2025 -c conda-forge python=3.12 numpy pandas matplotlib scikit-learn jupyterlab'

Set up the project:

    download 'MLPC2025_data_exploration.zip' from Moodle (link below)
    unzip the folder
    the project structure looks like this:


MLPC2025_data_exploration/   <---- start your terminal, powershell, etc in this folder or navigate to this folder (e.g., with 'cd')
├── MLPC2025_dataset/
 |   ├── audio/
 |   ├──── audio_features/
 |   ├──── metadata.csv
 |   └──── annotations.csv
└──── MLPC2025_data_exploration.ipynb <---- run this notebook

Start a terminal and navigate to folder 'MLPC2025_data_exploration', e.g., via the cd command.

Activate the conda environment via 'conda activate mlpc2025'.

Start JuypterHub via 'python -m jupyterlab'; a browser window should open automatically.

