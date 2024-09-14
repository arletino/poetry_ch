# poetry_ch
# poetry with jupyter notebook
Create a new project with Poetry:

poetry new test_ipynb
cd test_ipynb
Use a specific Python version with your environment:

poetry env use 3.12
Add ipykernel to your environment:

poetry add ipykernel
Check your environment's executable path:

poetry env info
Example output:

/home/guillaume/.cache/pypoetry/virtualenvs/test-ipynb-pH8Jwd_U-py3.12/bin/python
Open your project in VSCode:

code .
Then, in VSCode:

Install Jupyter extension

In the top right, click on the Select Kernel.

choose Python environment

Choose "Python Environments".

Python Environments

And select the environment you got from the env info command.

select the environment

This should allow you to use your Poetry-managed virtual environment directly within VSCode for Jupyter notebooks.

Additionally, if you want to use Jupyter or JupyterLab, just follow the steps above and add:

poetry add jupyter
poetry run jupyter notebook
# For JupyterLab
poetry add jupyterlab
poetry run jupyter lab
