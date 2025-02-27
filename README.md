# install_steps
# Setup Instructions

1. Install conda-forge for Windows from [https://conda-forge.org/](https://conda-forge.org/)

2. Install Git for desktop from [https://git-scm.com/downloads/win](https://git-scm.com/downloads/win)

3. Open mini-forge command prompt and type in the below commands:
    ```sh
    conda create -n openvino python=3.11
    conda activate openvino
    conda install jupyterlab ipywidgets
    git clone https://github.com/openvinotoolkit/openvino_notebooks.git
    git clone https://github.com/intel/AI-PC_Notebooks.git
    jupyter lab
    ```

4. Make sure you are in the root of your home directory.

5. Once you open the Jupyter lab, navigate to: `openvino_notebooks/notebooks/llm-agent-react` and run the `llm-agent-react-langchain.ipynb` notebook.
 
