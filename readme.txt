# Create environment

conda env create --name dsbook --file environment.yml
conda activate dsbook
python -m ipykernel install --user --name=dsbook

# Build

jupyter-book build dsbook

# Before commiting to git

nbstripout *.ipynb
