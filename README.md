# Setting up Environments and Installing Packages Using Conda

## Summary of steps to complete

- [x] Fork this repository so you have your own copy to work on.
- [x] Clone the repository on your local machine. 
- [x] Edit this README.md file on your machine.
- [x] Run the Conda commands shown in the video and describe them in the table below.
- [x] Push your changes to your GitHub repository.
- [x] Submit a link to this GitHub repository in Canvas.

## 1. Fork & Clone this repository

* We did this in a previous assignment. Instructions are here: https://github.com/cmcntsh/N6806_Fall2020_DevNotes/blob/master/Projects/002%20-%20Practice%20Using%20Git%20and%20GitHub/README.md
* This can also be done directly in VSCode
  * Create a new folder on your machine where you want to put this repository if you don't already have one you want to use.
  * Copy the Clone or Download path for this repository from GitHub.
  * In VSCode from the command pallette (Ctrl-Shift-P) run Git: Clone
  * Paste the path into the path field which pops up
  * Select your new folder you created on your machine
  * A new folder for the repository with the repository files should be in the folder you selected showing in the Explorer window in VSCode on the left side.
  
## Edit your README.md file

* [ ] In an editor of your choice (i.e. VSCode) edit this README.md file to add the answers requested in the tables.

## Follow along with this tutorial

* Conda What and Why? (27 min): https://www.youtube.com/watch?v=23aQdrS58e0&list=PLG9A6ovzPqX6d9uWzx0UYN9pm0zzl5ofA&index=13&t=0s
  * He installs Miniconda. We will be using Anaconda. Don't install Miniconda.
  * Follow along with the rest of the tutorial.
  * Go ahead and create the environments as he creates them in the tutorial.

## Conda Concepts

* [ ] Describe the Conda concepts used in the video and listed in the table below.

|   Concept   |         Description or short answer         |
|     ---     |                     ---                     |
|What is the purpose of having different environments?     |(to accomplish different types of projects on a single computer)|
|What is the default package manager in Python?            |(pip)|
|How do you manage environments and packages in Anaconda?  |(by using conda)|
|`conda list`       |(list of packages)|
|`conda env list`       |(list of environments)|
|How do you keep your base environment unchanged?       |(by using separate enviornments to install packages)|
|What is the link to the Conda cheat sheet? (link in video notes is broken)      |(https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf)|
|`conda create --name XXXX`       |(ai37)|
|`source activate XXXX`       |(ai37cond)|
|`conda install YYYY`       |(numpy)|
|channels in Conda       |(default, other)|
|`conda install -c ZZZZ YYYY`       |(pytorch pytorch)|
|`conda config --show channels`       |(defaults)|
|`conda config --add channels ZZZZ`       |(forge)|
|conda-forge.org       |(enter description or short answer here)|
|`source deactivate`       |(returns to base channel)|
|`conda config --get channels`       |(will get channels from conda forge first then defaults. this is important if you have different versions of packages. )|

* After creating the environments he created in the video on your computer, what would the results of running the command `conda env list` look like with the da35 environment activated. Paste the output from your command prompt in the code block below.

```
#Paste your results here.
base                     /opt/anaconda3
ai37                     /opt/anaconda3/envs/ai37
da35                  *  /opt/anaconda3/envs/da35

```
* What command would you use to remove the environments you created for this exercise from your computer?

```
conda env remove --name [name]

```
