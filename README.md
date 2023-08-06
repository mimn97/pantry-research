# Code Repository

## Introduction 

Code Repository of "Socio-geographic Disparities in ...." [Full title to be revealed after acceptance]. Preprint. 2023. Please note that all dataset needed for this study will be available upon request. 

----------
## How to replicate results in Conda Environment

- Install Anaconda. Enable pip dependency. 
- Create a conda environment named `fp_env`. 

```conda
conda create -n fp_env python=3.8
pip install -r requirements.txt
conda install -c conda-forge googlemaps
```
- After creating the virtual environment `fp_env`, run the following command to activate the environment: 
```conda
conda activate fp_env
```

- Place the following six data files from the attached Google Drive to the `data` folder in the repository ([Google Drive Link to Data](https://drive.google.com/drive/folders/1t_jOIKYtD_pKVYPa9V6dU00FPQ6RoHv7?usp=sharing)):
    - `fp_bg_pairs.pkl` (37.1M pairs of pantry and BGs in the U.S.)
    - `bg_pantry_travel_time_updated.csv` (~238K BG and pantry pairs with transit time information)
    - `bg_fp_regression.csv` (ALL 239K BGs' distance, ADI, travel time, rurality)
    - `ruralurbancodes2013.csv` (US county and rural/urban codes)
    - `US_2020_ADI_Census Block Group_v3.2.csv` (2020 ADI percentiles)
    - `us-state-fips.csv` (All US states and their FIPS code)
- Run `main.ipynb` to replicate the results in main body texts. 
- Run `accessibility_regression.ipynb` to replicate the results in regression analysis. (Supplementary Table 2)
- Run `supp_material.ipynb` to replicate the results in supplementary Information. 


Please note that `prepare_data.ipynb` and `compute_travel_time.ipynb` are to show how we were able to prepare our dataset for the main study. This files will take considerable amount of time and require your own API key, so please skip to `main.ipynb` to observe the results and understand insights about our study. 

For Figure 1(b), Supp. Figures 4 and 5, they were created by Tableau Desktop and require you to have your own API key to access the visuals. Please contact me if you further would like to see the software.

- Minhwa Lee (minhwalee@umass.edu)
