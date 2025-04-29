# EEG Based Source Localization Using PML

This repository contains the implementation and analysis of EEG-based brain source localization techniques, carried out as part of an Undergraduate Project under **Prof. Tushar Sandhan** at IIT Kanpur.

## 🧠 Project Overview

The objective of this project is to accurately estimate the sources of brain activity from EEG signals using advanced signal processing and Bayesian inference techniques. We compare several source localization algorithms and highlight the advantages of using the **Nonnegative Block-Sparse Bayesian Learning (NNBSBL)** method.

## 👥 Contributors

- **Students:** Asolla Lokesh (210226), Kinjarapu Gnan (210520)  
- **Supervisor:** Prof. Tushar Sandhan  
- **Mentor:** Swathi Pratapa

## 📊 Dataset: COG-BCI

We used the publicly available **COG-BCI dataset**, which includes EEG data collected over multiple sessions and tasks, such as:

- **Flanker Task:** Measures attention and conflict resolution.
- **Psychomotor Vigilance Task (PVT):** Measures sustained attention and vigilance.

**EEG Setup:**
- 64-channel Ag-AgCl electrodes
- Sampling rate: 500 Hz
- Standard 10–20 electrode placement

## 🧪 EEG Preprocessing & Visualization

- **ERP Plots** and **Topoplots** were generated for both tasks.
- Data was cleaned, segmented, and baseline-corrected before source localization.

## 🔍 Source Localization Techniques Compared

1. **LCMV Beamforming**  
2. **sLORETA**  
3. **Smooth Champagne**  
4. **BSBL-2S (Block Sparse Bayesian Learning - 2 Stage)**  
5. **NNBSBL (Nonnegative Block-Sparse Bayesian Learning)**

## 🏆 Key Results

- **NNBSBL** emerged as the most accurate and robust method:
  - High AUC (Area Under FROC Curve)
  - Low RMSE (Root Mean Square Error)
  - Robust to noise and missing electrodes
  - Physically realistic nonnegative priors

## 📌 Conclusion

The NNBSBL algorithm demonstrated superior performance in localizing EEG sources compared to traditional and other Bayesian approaches. Its use of nonnegative priors and covariance simplifications makes it ideal for practical, noisy EEG data.

## 📚 References

1. Hinss et al. (2022) - COG-BCI database  
2. Dinh et al. (2021) - Spatiotemporal LSTM for MEG/EEG  
3. Qu et al. (2022) - Nonnegative block-sparse Bayesian learning  
