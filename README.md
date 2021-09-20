# FMI in the Cloud

This repository contains the materials and instructions for the tutorial [FMI in the Cloud](https://2021.international.conference.modelica.org/vendor_tutorial.html) at the [14th International Modelica Conference 2021](https://2021.international.conference.modelica.org/).

## Prerequesites

- a [Google account](https://accounts.google.com/SignUp) to run the Python Notebook on [Google Colab](https://colab.research.google.com/)
- a clone or local copy of this repository
- a [GitHub account](https://github.com/join) to fork this repository
- a Conda environment with [FMPy](https://github.com/CATIA-Systems/FMPy) to run the Jupyter Notebook locally and to run the Web App
- a Python IDE or text editor to write the Web App

To create the Conda environment

- install [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (if you don't already have Conda installed)

- create a new Conda environment

```
conda create -n fmi-tutorial -c conda-forge python=3.9 fmpy notebook ipywidgets
```

- activate the environment

```
conda activate fmi-tutorial
```

## Part 1: Create a Jupyter Notebook

`Option 1:` run the Jupyter Notebook on the cloud

- [open Heater.ipynb](https://colab.research.google.com/github/t-sommer/fmi-cloud-tutorial/blob/main/Heater.ipynb) on Google Colab

`Option 2:` run the Jupyter Notebook locally

- change into the directory where you downloaded or cloned this repository and run

```
jupyter notebook Heater.ipynb
```

## Part 2: Create a Web App

Resources and inspirations:

- [Dash Bootstrap Components](https://dash-bootstrap-components.opensource.faculty.ai/)
- [Plotly Python Examples](https://plotly.com/python/)
- [Bootstrap CSS Framework](https://getbootstrap.com/docs/5.1/getting-started/introduction/)
- [generic FMPy Web App](https://github.com/CATIA-Systems/FMPy/blob/master/fmpy/webapp/__main__.py)
- [FMU Check](https://fmu-check.herokuapp.com/) ([source code](https://github.com/modelica/fmu-check))
- [FMI-based simulation workflows based on open source and commercial tools](https://2021.international.conference.modelica.org/Documents/Modelica2021_program.pdf) (Thu, 13:50 h)

Exercises:

- change the default simulation time to 50 s
- change the result variables
- add an additional parameter
- add the description from the modelDescription.xml below the image
- create a custom input signal
- deploy the web app

## Part 3: Hackathon and Q&A

Build your own Jupyter Notebooks and Web Apps and ask any questions about FMPy.

- explore the test FMUs in the [FMI Cross-Check](https://github.com/modelica/fmi-cross-check)
- fork this repository and share your results!
