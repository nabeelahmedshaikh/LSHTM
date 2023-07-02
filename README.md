# Installation

Assumption : - although this can be done on a Windows OS, this exercise was done on Ububtu OS

1)	Make a directory called miniconda3 using the following command on the terminal
```
mkdir -p ~/miniconda3
```
3)	Download conda (miniconda) installer to the folder using the following command
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda3/miniconda.sh
```
5)	Install conda
```
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
```
7)	Initialise bash
```
~/miniconda3/bin/conda init bash
```
8)	Optionally initialise ZSH if you are using ZSH
```
~/miniconda3/bin/conda init zsh
```
10)	At this stage you should be ready use conda, confirm by using the following command
```
conda –version
```
11)	Install mamba
```
conda install -n base -c conda-forge mamba
```
12)	Check for mamba installation by using the following command
```
Mamba –version
```
13)	Download the folder https://github.com/nabeelahmedshaikh/LSHTM to the directory of your liking

14)	Make sure you have downloaded the config.yml file from the git directory, while in the directory use the following command to install all required resources
```
mamba env create -f config.yml
```
15)	One all the software and the virtual environment has been installed, call the following command to activate the environment
```
conda activate renv
```
16)	Type ```rstudio``` at the prompt, this should open rstudio

# Questions

a.	create a pipeline to reproduce the style and trends in Figure 3 from the publication

``` While in the downloaded folder click on question_one.Rmd, once clicked press the Kint button on the file menu, this should create the required graph ```

b.	which meets appropriate software engineering standards

``` In order to have repeatability we use the conda package manager and .yml file for consistency, Check out config.yml for more details ``` 

c.	apply this pipeline for model 3 (from the publication), and the modification to model 3 (described in bullet C below)

``` While in the downloaded folder click on question_three.Rmd, once clicked press the Kint button on the file menu, this should create the required graph, note that the Model_3_modified.R is being used```

d.	explain how the pipeline could be used to include other models.

``` Other models can be included by loading them in the.Rmd file, they can be used in the same way as model 1,2,3 or modified 3 ``` 



