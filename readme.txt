# Create environment

conda env create --name dsbook --file environment.yml
conda activate dsbook
python -m ipykernel install --user --name=dsbook

# Build

jupyter-book build data-science-forelesningsnotater

# Before commiting to git

nbstripout *.ipynb

# Publish built book

ghp-import -n -p -f _build/html

