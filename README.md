# Face Recognition Security

### Guide to run the script(Latest)
- Install cmake from [here](https://cmake.org/download/) and add it to your PATH.
- Visual Studio installed with [build tools for cmake](https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools&rel=15)
- cd to the project and type in 
```pip install -r requirements.txt```
- Execute the python file
```python face_rec.py```

### Guide to run the script(Older Version)

1. Install Anaconda or Miniconda from [here](https://www.anaconda.com/distribution/#download-section)
2. Now, create a folder where you want project to be located and open a command prompt in the directory.
3. Create an environment using anaconda.
    1. To list the versions of Python that are available to install, in your terminal window or an Anaconda Prompt, run: `conda search python` or `conda search --full-name python` to list packages whose full name is "python"
    2. To list all the environments : `conda info --envs`  or
    `conda env list`
    3. Most of our dependencies work on a particular version of python i.e Python 3.6 (64bit), so we create an environment with Python 3.6 
    `conda create -n py36env python=3.6 anaconda`
    4. `py36env` is the name of the environment containing python 3.6 and anaconda is a metapackage that includes all of the Python Packages comprising Anaconda distribution
    5. To verify that the current environment uses the new Python version, in your terminal window or an Anaconda Prompt, run: `python —version`
    6. List packages installed : `conda list`
    7. To install a package for a specific Python version :
     `conda install scipy=0.15.0 numpy=7.26.0 -n py36env`
    8. To deactivate the environment, run: `conda deactivate` 
    9. To activate the environment, run: `conda activate py36env`
4. Install dependencies of python
    1. Move to the directory of the project, open cmd and activate your environment : `conda activate py36env`
    2. Install Numpy: `pip install numpy`
    3. Install Pandas : `pip install pandas`
    4. Install OpenCV : `pip install opencv-python`
    5. Install cmake : `pip install cmake`
    6. Install dlib : `pip install dlib`

        dlib depends on cmake, so make sure that you install cmake from [here](https://cmake.org/download/) and add it to your PATH. Also, you should have Visual Studio installed with [build tools for cmake](https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools&rel=15)

    - Install face recognition : `pip install face_recognition`
5. Setting up [VS Code](https://code.visualstudio.com/download) with the environment, open the project folder using VS Code.
Now, we have to select the specific Python environment which will run our code, use the **Python: Select Interpreter** command from the **Command Palette (Ctrl+Shift+P)** and select the environment py36env.
