# install_steps
# Setup Instructions: Demo on AI PC

1. Install conda-forge for Windows from [https://conda-forge.org/](https://conda-forge.org/)

2. Install Git for desktop from [https://git-scm.com/downloads/win](https://git-scm.com/downloads/win)

3. Open mini-forge command prompt and type in the below commands:
    ```sh
    conda create -n openvino python=3.11
    conda activate openvino
    conda install jupyterlab ipywidgets
    git clone https://github.com/openvinotoolkit/openvino_notebooks.git
    git clone https://github.com/intel/AI-PC_Notebooks.git    
    ```

4. Make sure you are in the root of your home directory.
   ```sh    
    jupyter lab
    ```

6. Once you open the Jupyter lab, navigate to: `openvino_notebooks/notebooks/llm-agent-react` and run the `llm-agent-react-langchain.ipynb` notebook.

# Setup Instructions: Demo on Intel® Tiber™ AI Cloud

1. Open File->New->Terminal

3. Type in the below commands:
    ```sh
    conda create -n gpu_llmsycl python=3.11
    conda activate gpu_llmsycl    
    git clone https://github.com/intel/AI-PC_Notebooks.git
    source /opt/intel/oneapi/setvars.sh --force
    CMAKE_ARGS="-DGGML_SYCL=on -DCMAKE_C_COMPILER=icx -DCMAKE_CXX_COMPILER=icpx" pip install llama-cpp-python -U --force --no-cache-dir --verbose
    
    ```

4. Create a ipykernel as below
   ```sh    
    python -m ipykernel install --user --name=gpu_llmsycl
    ```

5.  Navigate to: `AI-PC_Notebooks/AI-Travel-Agent/` and run
          
   pip install -r requirements.txt
          
 
