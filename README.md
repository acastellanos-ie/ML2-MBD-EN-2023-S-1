# Machine Learning 2
Repository for the ML2 class of the Big Data and Analytics Master. 

In this repository you will find all the technical materials related to this course (notebooks, scripts, files,...).

Please read carefully the following instructions ([Using the ML2 environment](#using-the-ML2-environment)) to setup the environment needed for the practices if you want to configure your computer to execute the notebooks.

If you prefer to execute them in an online environment in Google Colab, please refer to [Execute the notebooks remotely](#execute-the-notebooks-remotely). 


# Using the ML2 environment

## Create the working directory

On your computer, create the directory on which you want to work. In my case, it's called `machine_learning_2`.

## Connect your local directory to this repository

In this step you will connect your local directory to this repository. In this way you will download the data initially included here, as well as the new materials that I will be uploading regularly.

The first thing you need to do is to open a terminal and go to the folder that you previously created (please note that the following is where I have the directory, change the path with yours)

```
cd /home/acastellanos/Dropbox/IE/IE_ML/Practice Directory/machine_learning_2
```  
Clone the repository
```
git clone https://github.com/acastellanos-ie/ML2-MBD-EN-OCT-2021-S-1.git
```

After cloning you should see all the materials in your local folder (and your local folder will be connected to this repo).

I will be regularly updating the materials, so, please, before each practical class make sure that you have the latest version of the repo ([Guide](https://www.atlassian.com/git/tutorials/syncing/git-pull). for pulling data from a repo)

## Download Anaconda

I strongly recommend you to use Anaconda to manage your Python environments. [Link to download Anaconda](https://www.anaconda.com/products/individual)

## Create the `conda` environment

`conda` environments are the playgrounds on which we’ll work in Python. There are other tools to create environments too, but `conda` is included and installed when installing the
Anaconda suite and is one the industry’s standards.

1. Open a terminal and go the folder you previously created

  ```
  cd /home/acastellanos/Dropbox/IE/IE_ML/Practice Directory/machine_learning_2
  ```
  
2. Create the environment with a name of your choice:

  ```
  conda create --name ml2 python=3.8
  ```
  
After the parameter `--name` we define the name of our environment. In my case, it’s `ml2`. Also you can choose the python version (3.8 for us).

3. Activate your environment:

  ```
  conda activate ml2
  ```
  
## Install the required libraries in your environment

In order to have a smooth and stable environment, it’s common to have a `requirements.txt` file that includes all the libraries that are used in your projects. 

That way, whenever you join a new project, it’s easy to start working without worrying about missing libraries or modules.

Installing the required libraries in our environment it’s as easy as follows (the requirements.txt is the file included in this repository):

```
pip install -r requirements.txt
```

## Open a Jupyter/JupyterLab session with our current environment

Before opening a Jupyter session, we have to make sure that our environments will be included. In order to solve this, run the following command:

```
conda install nb_conda_kernels
```

Once this is installed, we are ready to open a Jupyter session by using the following command:

```
jupyter lab
```

or if you prefer the old notebooks use:

```
jupyter notebook
```

A new tab of your browser will open with the Jupyter session, showing all the available environments. To create a Notebook with your current environment, select it from the
Notebooks list.

And now you’re ready to start!

# Execute the notebooks remotely

If you prefer to execute the notebooks remotely, I am configured each notebooks so they can be easily executed at Google Colab. At the beginning of each notebook you have a button to open the notebook in Colab. Once in Colab, you just need to execute the configuration steps included at the beginning of each notebook.
