# install_steps
Install conda-forge for windows from https://conda-forge.org/

Install Git for desktop from https://git-scm.com/downloads/win

Open mini-forge command prompt and type in the below commands:

   conda create -n openvino python=3.11
   
   conda activate openvino 
   
   conda install jupyterlab ipywidgets
   
   git clone https://github.com/openvinotoolkit/openvino_notebooks.git
   
   git clone https://github.com/intel/AI-PC_Notebooks.git
   
   jupyter lab  (Make sure you are in the root of your home directory

   Once you open the Jupyter lab Navigate to: openvino_notebooks/notebooks/llm-agent-react and run the llm-agent-react-langchain.ipynb notebook
 
