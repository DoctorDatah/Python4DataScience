Before importing libraries to the environment. We have to add it to the PATH.
Doing that from python
<code>
import sys
PATH = r"C:\Users\malik\AppData\Local\Continuum\miniconda3\envs\data601\Lib\site-packages"
sys.path.append(PATH)
</code>