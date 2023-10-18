# Data and code for "How does the Minnesota Alternative Minimum Tax Affect Household Filers?"
This repository contains the data and code for the analyses in the *Research in Focus* article by [Richard W. Evans](https://sites.google.com/site/rickecon) ([@rickecon](https://github.com/rickecon)) and Mitchell Pound ([@mitchellpound](https://github.com/mitchellpound)) entitled "How does the Minnesota Alternative Minimum Tax Affect Household Filers?".

## How to run the code from these analyses in the cloud in your browser
We have created a [Google Colab notebook](https://colab.research.google.com/drive/1TYFiOsyHzkdmXEn5ygFDcZioq2GqAT7C?usp=sharing) with code almost exactly the same as th code in the Jupyter Notebook [`MN_AMT.ipynb`](MN_AMT.ipynb) decribed in the next section. The [Google Colab notebook](https://colab.research.google.com/drive/1TYFiOsyHzkdmXEn5ygFDcZioq2GqAT7C?usp=sharing) has the advantage of using a distribution of Python and corresponding packages that run in the cloud on remote servers instead of on your local machine. This allows you to use the notebook from any kind of device with a browser. You can execute th code, see the results, and save output to a temporary cloud folder from which you can download anything you want to keep.

## How to run the Jupyter Notebook on your machine
This repository contains a Jupyter Notebook [`MN_AMT.ipynb`](MN_AMT.ipynb) that can be run locally on your own machine to replicate the analyses in the paper. You can also modify this notebook to use for other analyses you might want to experiment with. To run this notebook locally on your machine, do the following steps:
* Fork and clone (or download) the https://github.com/TheCGO/MN-AMT repository
* In your computer's terminal, navigate to the directory of the `MN-AMT` repository on your local machine.
* Create the conda environment `mn-amt-dev` by typing the following command: `conda env create -f environment.yml`
* Activate the `mn-amt-dev` conda environment by typing the following command: `conda activate mn-amt-dev`
* This should allow your notebook to run while this conda environment is activated.


## Files and directories in the repository
This repository contains the following items:
* [`MN_AMT.ipynb` Jupyter notebook](MN_AMT.ipynb). An executable notebook you can use to replicate all the analyses in the article and creation of output and figures.
* [`/data/` directory](data/). This directory contains the data used in the analyses in the article--PEW total balances and rainy day fund balances historical data for all 50 states.
    * [`/data/cb_2018_us_state_20m`](/data/cb_2018_us_state_20m). Folder containing US Census Bureau shapefiles (7 files) and corresponding files for US states. We use the "<1.0 MB" files (the `_20m` extension). See https://www.census.gov/geographies/mapping-files/2018/geo/carto-boundary-file.html. These are used in the creation of the [`/images/state_amt_2023.html`](/images/state_amt_2023.html) map image in [`MN_AMT.ipynb` Jupyter notebook](MN_AMT.ipynb).
    * [`/data/fig1_state_amt.csv`](/data/fig1_state_amt.csv). Source data for Figure 1 map in the paper.
    * [`/data/fig2_source.csv`](/data/fig2_source.csv). Source data for Figure 2 in the paper.
    * [`/data/fig3_source.csv`](/data/fig3_source.csv). Source data for Figure 3 in the paper.
    * [`/data/fig4_source.csv`](/data/fig4_source.csv). Source data for Figure 4 in the paper.
    * [`/data/fig5_source.csv`](/data/fig5_source.csv). Source data for Figure 5 in the paper.
* [`/images/` directory](images/). This folder contains the `.html` files for the dynamic visualizations in the paper and created in the notebook and the corresponding static `.png` image files.
    * [`/images/fig1_state_amt_2023.html`](/images/fig1_state_amt_2023.html). Dynamic data visualization Bokeh `.html` file. Figure 1. Four states with state alternative minimum tax (AMT) as of November 2023
    * [`/images/fig1_state_amt_2023.png`](/images/fig1_state_amt_2023.png). Static `.png` file. Figure 1. Four states with state alternative minimum tax (AMT) as of November 2023
    * [`/images/fig2_amt_minus_stnd_mar_children.html`](/images/fig2_amt_minus_stnd_mar_children.html). Dynamic data visualization Bokeh `.html` file, for web publication. Figure 2. Minnesota AMT minus standard tax liability for married filers by employment income and number of children
    * [`/images/fig2_amt_minus_stnd_mar_children.png`](/images/fig2_amt_minus_stnd_mar_children.png). Static `.png` file, for web publication. Figure 2. Minnesota AMT minus standard tax liability for married filers by employment income and number of children
    * [`/images/fig3_amt_minus_stnd_sngl_children.html`](/images/fig3_amt_minus_stnd_sngl_children.html). Dynamic data visualization Bokeh `.html` file, for web publication. Figure 3. Minnesota AMT minus standard tax liability for single filers by employment income and number of children
    * [`/images/fig3_amt_minus_stnd_sngl_children.png`](/images/fig3_amt_minus_stnd_sngl_children.png). Static `.png` file, for web publication. Figure 3. Minnesota AMT minus standard tax liability for single filers by employment income and number of children
    * [`/images/fig4_amt_minus_stnd_deduct_mar_children.html`](/images/fig4_amt_minus_stnd_deduct_mar_children.html). Dynamic data visualization Bokeh `.html` file, for web publication. Figure 4. Minnesota AMT minus standard tax liability for married filers by AMT-non-allowable deductions and number of children
    * [`/images/fig4_amt_minus_stnd_deduct_mar_children.png`](/images/fig4_amt_minus_stnd_deduct_mar_children.png). Static `.png` file, for web publication. Figure 4. Minnesota AMT minus standard tax liability for married filers by AMT-non-allowable deductions and number of children
    * [`/images/fig5_amt_minus_stnd_deduct_sngl_children.html`](/images/fig5_amt_minus_stnd_deduct_sngl_children.html). Dynamic data visualization Bokeh `.html` file, for web publication. Figure 5. Minnesota AMT minus standard tax liability for single filers by AMT-non-allowable deductions and number of children
    * [`/images/fig5_amt_minus_stnd_deduct_sngl_children.png`](/images/fig5_amt_minus_stnd_deduct_sngl_children.png). Static `.png` file, for web publication. Figure 5. Minnesota AMT minus standard tax liability for single filers by AMT-non-allowable deductions and number of children
