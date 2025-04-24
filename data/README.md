# data

This directory contains both MATLAB-compatible EEG datasets (`.set`/`.fdt`) and CSV files with concatenated, feature-enriched data from 54 participants (excluding participant 52). These datasets were collected and preprocessed for analyses involving decision-making tasks across two environments.

---

## Preprocessed EEG Data

### 1. MATLAB EEG Datasets (`.set` / `.fdt`)
- Final preprocessed datasets for 53 participants (participant 52 excluded).
- Each `.set` file is accompanied by a corresponding `.fdt` file.
- Sampling frequency: **500 Hz**
- Epoch length: **1100 ms** (from **-1s to 0.1s** relative to the event marker)
- Channels: **26** (except Participant 1 who has **25** due to one noisy channel removal)
- Reference: **TP8 and TP9 channels**
- Each epoch is labeled with decision events: **‘stay’** or **‘leave’**

These files can be accessed and analyzed using **EEGLAB** in **MATLAB**.

---

### 2. CSV Datasets

All CSV files contain the same feature-rich columns (see below) and differ in how the data is grouped or filtered:

#### File Descriptions

- **`All_epochs_combined_e1.csv`**  
  Contains **epoch-wise** EEG data from **environment 1** only.

- **`All_epochs_combined_e2.csv`**  
  Contains **epoch-wise** EEG data from **environment 2** only.

- **`All_epochs_combined.csv`**  
  Contains **epoch-wise** EEG data from **both environments** combined.

- **`participant_wise_combined.csv`**  
  Contains **participant-level averaged** EEG data across **both environments**.

---

## CSV Columns

Each CSV file includes:

- **Task-related metadata**:  
  `Tree number`, `Time elapsed`, `Decision`, `trait_anx_level`, `Reaction time`, `Reward`, `Cumulative reward per tree`, `Total cumulative reward`

- **EEG power features** (by electrode):  
  Raw power: `En_Fp1`, `En_Fp2`, ..., `En_FCz`  
  Band ratios:  
  - `*_theta_alpha`  
  - `*_theta_beta`  
  - `*_theta_gamma`

- **Connectivity metrics** (e.g., TFC, AFC):  
  `F3_F4_TFC`, `F3_Fz_TFC`, ..., `F4_Fz_AFC`

- **ERP component features** (mean and peak amplitudes):  
  `FRN_mean`, `FRN_peak`, `LPP_mean`, `LPP_peak`,  
  `MMN_mean`, `MMN_peak`, `N170_mean`, `N170_peak`,  
  `N200_mean`, `N200_peak`, `P1_mean`, `P1_peak`,  
  `P300_mean`, `P300_peak`

---

## Usage Tips

- CSV files can be read directly using Python, R, or MATLAB for statistical analysis and machine learning tasks.
- `.set` files are best analyzed with EEGLAB for ERP analysis, time-frequency analysis, and visualization.

---

## Citation

If you use this dataset in your research or analysis, please cite appropriately.
