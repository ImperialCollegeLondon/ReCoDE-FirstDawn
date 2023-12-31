<!-- Your Project title, make it sound catchy! -->

# Using Convolutional Neural Networks to extract information from the Cosmic Dawn

<!-- Provide a short description to your project -->

## Description

This exemplar will explain and demonstrate the steps required to go from image-based data to a finished Convolutional Neural Network (CNN) pipeline, which can be used to extract relevant information from the images. While demonstrating how to solve this machine learning problem, I will also explain how to prototype code in Jupyter notebooks. I will start by explaining how to analyse the statistics of the data to create appropriate training, validation and testing sets; here I will emphasize the importance of uniform parameter spaces. The exemplar will then go through the process of setting up the architecture of the network and how to train it. Once the network is trained I will discuss what possible next steps are, and which is the most appropriate. Finally, I will go through how to convert the code prototyped in Jupyter notebooks into a useable package

<!-- What should the students going through your exemplar learn -->

## Learning Outcomes

- Use a Jupyter Lab notebook to prototype code
- Use tensorflow to create a CNN to infer parameters from simulated images
- Convert that prototyped code into a runable script that can then be scaled up to be run on something like the HPC

<!-- How long should they spend reading and practising using your Code.
Provide your best estimate -->

| Task       | Time    |
| ---------- | ------- |
| Introduction to CNNs    | 1 hours |
| FirstDawn | 3 hours |

## Requirements

<!--
If your exemplar requires students to have a background knowledge of something
especially this is the place to mention that.

List any resources you would recommend to get the students started.

If there is an existing exemplar in the ReCoDE repositories link to that.
-->

### Academic

- Familiarity with Python 3
- Have used Jupyter Lab before
- Very little command line knowledge



<!-- List the system requirements and how to obtain them, that can be as simple
as adding a hyperlink to as detailed as writting step-by-step instructions.
How detailed the instructions should be will vary on a case-by-case basis.

Here are some examples:

- 50 GB of disk space to hold Dataset X
- Anaconda
- Python 3.11 or newer
- Access to the HPC
- PETSc v3.16
- gfortran compiler
- Paraview
-->

### System

- 4GB of disk space for datasets
- Python 3.11 or newer
- Access to the HPC (optional)

<!-- Instructions on how the student should start going through the exemplar.

Structure this section as you see fit but try to be clear, concise and accurate
when writing your instructions.

For example:
Start by watching the introduction video,
then study Jupyter notebooks 1-3 in the `intro` folder
and attempt to complete exercise 1a and 1b.

Once done, start going through through the PDF in the `main` folder.
By the end of it you should be able to solve exercises 2 to 4.

A final exercise can be found in the `final` folder.

Solutions to the above can be found in `solutions`.
-->

## Getting Started

To get started, first clone this repo, then change directories into it:
```
  git clone https://github.com/kimeels/ReCode_FirstDawn.git
  cd ReCode_FirstDawn
```

If python virtualenv  and Jupyter Lab isn't already installed on your system, install it using:

```
  python3 -m pip install virtualenv
  python3 -m pip install jupyterlab
```

Then create a virtual environment for this exemplar:

```
python3 -m venv venv_recode_firstdawn
```

Source into your new virtual environment using:

```
  source venv_recode_firstdawn/bin/activate
```

Run this line to install all the necessary packages:

```
  pip install -r requirements.txt
```
Finally, run these two lines to setup your virtual env with jupyter lab.
```
  pip install ipykernel
  python -m ipykernel install --user --name=venv_recode_firstdawn
```


<!-- An overview of the files and folder in the exemplar.
Not all files and directories need to be listed, just the important
sections of your project, like the learning material, the code, the tests, etc.

A good starting point is using the command `tree` in a terminal(Unix),
copying its output and then removing the unimportant parts.

You can use ellipsis (...) to suggest that there are more files or folders
in a tree node.

-->

## Project Structure

```log
.
├── docs
├── notebooks
    ├── figures
    ├── Converting to a python script.ipynb
    ├── FirstDawn.ipynb
    └── Introduction to CNNs.ipynb
│   
└── requirements.txt
```

<!-- Change this to your License. Make sure you have added the file on GitHub -->

## License

This project is licensed under the [BSD-3-Clause license](LICENSE.md)
