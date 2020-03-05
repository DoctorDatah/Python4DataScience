conda create --name ENV_NAME

activate ENV_NAME

conda info --envs
conda env list

conda env remove -n ENV_NAME


conda install jupyter

**If you want to install Matplotlib for Python 3 through the APT package manager, you need the package python3-matplotlib:**

sudo apt-get install python3-matplotlib
If you want to install it with Pip for Python 3, you need to use pip3:

sudo pip3 install matplotlib


**List libraries**

pip list 

pip freeze  > file.txt



**Here are 3 solutions to your problem**

You can add the directory containing the file you with to import to your path and then import the file. like this
import sys  
sys.path.insert(0, '/path/to/application/app/folder')

import file
You can create a local module by having an empty __init__.py file in the folder you want to import. There are some weird rules regarding the folder hierarchy that you have to take into consideration.

You can create a module for the file you wish to import and install it globally.

https://stackoverflow.com/questions/448271/what-is-init-py-for
https://pythontips.com/2013/07/28/what-is-__init__-py/


**jupyter notebook import error: no module named 'matplotlib'**

first of all, I would got for one python Version. Preferably the Python3 Version. Uninstall Conda with conda install anaconda-cleanand re-install

**Extensions Jupyter notebook**<br>
User<br>
pip install jupyter_contrib_nbextensions
jupyter contrib nbextension install --user
<br>Virtual environment<br>
pip install jupyter_contrib_nbextensions <br>
jupyter contrib nbextension install --sys-prefix
<br>Enable<br>
jupyter nbextension enable varInspector/main


https://github.com/lckr/jupyterlab-variableInspector

**Adding Path Variable** <br>
https://www.youtube.com/watch?v=A7E18apPQJs

**Spell Checker Jupyter Lab**

conda install -c conda-forge nodejs<br>
jupyter labextension install @ijmbarr/jupyterlab_spellchecker


**Update Conda** <br>
conda update -n base -c defaults conda 

**install Jupter lab**<br>
Latest version might have Errors <br>
conda install -c conda-forge jupyterlab
<br> For Specific Version <br>
conda install -c conda-forge jupyterlab=1.0.0
<br> List of Releases <br>
https://jupyterlab.readthedocs.io/en/stable/getting_started/changelog.html
<br>**Build Extension after install**<br>
jupyter lab build



**Nodejs** <br>
conda install -c conda-forge nodejs
<br>
conda install nodejs

**Reset Everything base+all**<br>
conda install --revision 0
 <br>


**TIP:** <br>
**pip/conda try either of one, if one does not work**

