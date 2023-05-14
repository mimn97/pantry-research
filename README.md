# Code Repository

## Introduction 

Code Repository of "Socio-geographic Disparities in Accessibility to Food Pantries in the United States". Preprint. 2023. 

----------
## How to Run Jupyter Notebooks in Conda Environment

- Install Anaconda. 
- Create a conda environment named `fp_env`. 

```conda
conda create -n fp_env python=3.8
pip install -r requirements.txt
conda install -c conda-forge googlemaps
```

- Place the following five files in the `data` folder:
    - `food_bg20_adi_st.pkl`
    - `bg_transit_adi.csv`
    - `ruralurbancodes2013.csv`
    - `US_2020_ADI_Census Block Group_v3.2.csv`  
    - `us-state-fips.csv`
- Run `main.ipynb` to replicate the results in main body texts. 
- Run `accessibility_regression.ipynb` to replicate the results in regression analysis. (Supplementary Table 2)
- Run `supp_material.ipynb` to replicate the results in supplementary Information. 


Please note that `prepare_data.ipynb` and `compute_travel_time.ipynb` are to show how we were able to prepare our dataset for the main study. This files will take considerable amount of time and require your own API key, so please skip to `main.ipynb` to observe the results and understand insights about our study. 
