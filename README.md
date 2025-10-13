# In-Class Exercises for Equilibrium Modeling Course
Instructors: Steven A. Gabriel, Seksun Moryadee, Fabricio Oliveira, Helmi Hankimaa
Date: October 2025

This repository contains a set of Jupyter notebooks meant to complement lectures on the Equilibrium Modeling as part of the in-person course at Petrobras. The repository contains three notebooks:

Module 1: Bilevel Problems

Module 2: Optimization Problems & Karush-Kuhn-Tucker (KKT) Conditions

Module 3: Mixed Complementarity Problems (MCPs) 

Each notebooks corresponds to a module in the course and they each include several exercises. The notebooks are designed to be self-contained but are closely linked with the in-person lectures of the course. The notebooks implement optimization models using Pyomo, a Python-based, open-source optimization modeling language. The problems are solved using SCIP, an open-source optimization solver and PATH, a solver for mixed complementarity problems.

## Getting Started
There are two main options for installing and running the Jupyter notebooks (1) remotely or (2) locally. For users with limited Python programming experience, running the notebooks remotely via Google Colab is highly recommended. Users comfortable with environment management in Python and command line interfaces may prefer option 2.

### (1) Running Notebooks in Google Colab (recommended)
Google Colaboratory is a free, browser-based tool that allows users to write and run Python code. To access and run the notebooks on Google Colab, click on the links below. The links will open the notebooks in a separate web browser.

To edit the notebooks, you must save a copy of the notebook to your Google Drive which can be done from the menu File -> Save a copy in Drive. For Modules 2 and 3, after saving a copy, you will need to **upload the PATH solver linux executable file** to the Colab project. The code expects to find this file in ```/content/path/pathampl```. To do this

 1. Download the linux executable file from this repository: it is the ```path/linux/pathampl``` file.
 2. In the Colab notebook, open the file explorer by clicking the folder icon in the left-hand side bar. Create a new folder named ```path``` in the file explorer with right-click -> New folder.
 3. Upload the ```pathampl``` file to the ```path``` folder by right-clicking on the ```path``` folder and selecting Upload.

The first cells in each notebook will install the necessary package dependecies and set up solvers. Once you have run these cells you will be good to go!

Module 1: [notebook 1](https://drive.google.com/file/d/1V3B1-z5ukzxppb0n36vigkPd3o6rJB2r/view?usp=sharing)

Module 2: [notebook 2](https://drive.google.com/file/d/11C0ZIebo6y_dMHzv1ymAW63hoe2mBxKg/view?usp=sharing)

Module 3: [notebook 3](https://drive.google.com/file/d/1-StG3rq54fhPNRpjx19egFJYWAj1K3Q6/view?usp=sharing) 




### (2) Running the Notebooks Locally
To run the notebooks locally, there are two main options: (1) running on a jupyter server or (2) running on VS Code. Both of these steps require cloning this repository via the following command:

```git clone https://github.com/helmihankimaa/PB_equilibrium_course.git```

In addition, both methods assume [pip](https://pip.pypa.io/en/stable/installation/) and [Anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) are installed on your local machine. 

#### The Jupyter Server
The Jupyter notebook is a web-based notebook environment for interactive computing.

First, you will need to create your conda environment using the course_env.yml file:

```conda env create -f course_env.yml```

This will create a conda environment on your local machine and install all dependencies needed to run the notebooks.

Then, activate the environment:

```conda activate course_env```

Once the environment is activated, navigate to the directory of your cloned repository and run the following command to start the Jupyter session:

```jupyter notebook```

This will start a remote connection to the Jupyter server and open this repository in your web browser. Clicking on one of the notebooks will start a new kernel and allow you to run the notebooks.

#### VS Code Set-Up
Alternatively, [Visual Studio Code](https://code.visualstudio.com)  recently introduced support to run Jupyter notebooks natively. To run these notebooks directly in Visual Studio code, perform Steps 1 and 2 above to install and activate your conda environment. Then, open VS Code and follow [these instructions](https://code.visualstudio.com/docs/datascience/jupyter-notebooks) to open and run the notebook in VS Code.
