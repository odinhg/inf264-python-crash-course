# Installing Required Software for INF264

## 1. Installing Anaconda

To install Anaconda, click the link below corresponding to your operating system and follow the instructions there.

- [Windows](https://docs.anaconda.com/free/anaconda/install/windows/)
- [macOS](https://docs.anaconda.com/free/anaconda/install/mac-os/)
- [Linux](https://docs.anaconda.com/free/anaconda/install/linux/)

## 2. Create an Environment

We will now create a new Anaconda environment for INF264.

1. Open a terminal window.
2. Run the command `conda create --name=INF264 python` to create a new environment named `INF264` with the latest Python version.
3. Run the command `conda activate INF264` to activate the newly create environment.
4. Run `conda install -c conda-forge numpy scikit-learn jupyter pandas matplotlib ipykernel` to download and install the required packages. 

To test that everything is working as expected, create a new notebook by running `jupyter-lab` (if you use VS Code, see below) and create and run a code cell with the following content:

```python
import sklearn
import numpy
import pandas
import matplotlib.pyplot
```

**If your are using VSCode, you can also work with the Jupyter notebooks there.** After opening a notebook in VSCode, choose the `INF264` environment as the kernel for your notebook. To do this, click on the kernel name or the "Select Kernel" button in the top right corner of the notebook and choose the `INF264` environment.

**Useful notebook shortcuts:**
- Arrow keys to navigate between cells.
- `Shift + Enter` to run the current cell and move to the next one.
- `Ctrl + Enter` to run the current cell and stay in the same cell.
- `Esc` to enter command mode.
- `Enter` to enter edit mode.
- `A` to insert a new cell above the current cell.
- `B` to insert a new cell below the current cell.
- `DD` to delete the current cell.
- `M` to change the current cell to a Markdown cell.
- `Y` to change the current cell to a code cell.


If the cell runs without any import errors, congratulations! If you get any error message(s), ask a group leader for help or post your question in the Discord channel [#technical-help](https://discord.com/channels/1248589525341704254/1248593123026927726). 

## 3. Managing the Environment

Enter the environment by running `conda activate INF264`. To exit the `INF264` environment, simply run `conda deactivate`.

(Optional) To update all packages in your environment, run `conda update --all` (when the environment is already activated).

(Optional) At the end of the semester, if you want to clean up and delete the `INF264` environment from your system, run the command `conda env remove --name INF264`.

