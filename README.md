# TLS Treelist Prediction

Predict tree plant functional type, genus, and species from terrestrial lidar scans tree features using hyper-param tuned CatBoost trained on FastFuel dataset

### Getting started
1. Download the data and form the directory structure shown as follows.
```bash
sprint_4/
├── FastFuel
│   ├── FF_treelist_all.csv
│   ├── blk_plot_identification.csv
│   └── fftl_column_description.csv
├── SPCD_from_points.ipynb
├── TLS_catboost.ipynb
├── fia-database-california
│   ├── CA_PLOT.csv
│   └── CA_TREE.csv
├── field_data
│   ├── 01_plot_identification.csv
│   └── 03_tree.csv
├── requirements.txt
├── species_reference
│   ├── FIATreeSpeciesCode_pft.csv
│   └── REF_SPECIES.csv
├── terrestrial-lidar-scans-tls-and-derived-tree-lists-for-field-sampled-plots-for-uc-climate-actio
│   ├── TLS_treelist.csv
│   ├── blk_plot_identification.csv
│   ├── intellimon_chm.zip
│   ├── intellimon_column_descriptions.csv
│   └── tls_files_download_paths.txt
└── tls_catboost_v3.cbm
```
2. Create environment & install:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook 
   > **Note:**  
   > The notebook currently loads fine-tuned model weights.  
   > - To replicate the training process, set `is_infer = False` in the `CFG` class.  
   > - To perform hyperparameter tuning, set `n_hyper_trial > 0`.  
   >  
   > Additional details and explanations are included as comments within the notebook.

### Results
<img width="706" alt="tls distribution plot" src="https://github.com/user-attachments/assets/6e025843-ce11-4de9-84e9-aee8ef5bcc52" />



