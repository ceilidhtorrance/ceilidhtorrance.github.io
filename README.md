# ceilidhtorrance.github.io

## Repository
This repository is the completed project for the DSCI 521 class. This site is built using Quarto and demonstrates a number of skills I learned during Block 1. 

## Software Requirements
The following software is required to build this website: 
- Quarto: 1.10.18
- Python: 3.14.7
- uv: 0.12.6
- R: 4.6.1
- renv: bootstraps automatically from the project configuration

## Instructions to build site

### 1. Clone the repository
In your terminal, navigate to the directory where you want the cloned repository to exist. Then, run the following commands in a terminal: 

```bash
git clone https://github.com/ceilidhtorrance/ceilidhtorrance.github.io.git

cd ceilidhtorrance.github.io
```
### 2. Setup the Python environment
Run these commands in the repository root (this is the folder you landed in at the ended the last step in after changing directory). 

```bash
uv sync
```

### 3. Setup the R environment
Open RStudio or Positron in the repository root. In the console of your environment run:  

```r
renv::restore()
```

### 4. Preview the site before building
If desired, preview the website locally by running the following command from the repository root: 

```bash
uv run quarto preview
```

Quarto will provide a local URL that can be opened in a web browser. Press `CRTL+C` in the terminal to stop the preview server. 

### 5. Build and view the website
Return to the terminal and run: 

```bash
uv run quarto render
```
Rendering writes the built website to the `docs/` directory. The main page can be viewed locally by opening `docs/index.html` in a web browser. 

## Data Sources
The penguin data used in this project comes from the Palmer Penguins dataset, provided by Allison Horst and the Palmer Station Antarctica LTER. 

The dataset is accessed through the `palmerpenguins` R package / Python package. The data is included with the packages, so the website build does not need to download the dataset from the internet once the required packages have been installed. 