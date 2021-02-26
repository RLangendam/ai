# AI

# How to run

Install [Python 3.8](https://www.python.org/downloads/) and use pip to install the required packages

    python.exe -m pip install --upgrade pip
    
    python.exe -m pip install tensorflow tensorflow-datasets numpy pandas keras ipykernel jupyter seaborn scikit-learn

# Use GPU

Follow [these](https://www.tensorflow.org/install/gpu) instructions and

    python.exe -m pip install pycuda

# VSCode

Use the [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) plugin.

# Problems

Run the following to find out what's wrong

    python.exe -c "import tensorflow as tf; print('tf version:', tf.version); tf.config.list_physical_devices()"

For example

    Could not load dynamic library 'cudart64_110.dll'

indicates that [CUDA Toolkit 11(.2)](https://developer.nvidia.com/cuda-toolkit-archive) must be installed.

    Could not load dynamic library 'cusolver64_10.dll'

indicates that `C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.2\bin\cusolver64_11.dll` needs to be renamed to `cusolver64_10.dll`

# Resources

* [Deap Learning with Python](https://livebook.manning.com/book/deep-learning-with-python/about-this-book/)
* 