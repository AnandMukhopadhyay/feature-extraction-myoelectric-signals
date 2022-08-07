# feature-extraction-myoelectric-signals

**Structure of Folders**
   
    **data**: contains the raw filtered data samples for Subject S4 of Khushaba dataset 6 (Download - https://onedrive.live.com/?authkey=%21AMM7EZHhadbAlAo&id=AAA78954F15E6559%21176&cid=AAA78954F15E6559)
     
    ** codes:**
    
        - S01_main_data_generation.mlx - main script. Need to select type of feature extraction - cTDD or fTDD
        
        - batch12.mlx - Function for trial 1 data recordings
        
        - batch22.mlx - Function for trial 2 data recordings
        
        - getcTDDfeat.mlx - Function to computes cTDD features using same window
        
        - getfTDDfeat.mlx - Function to computes fTDD features using nearby windows decided by step factor
        
        - getCategory.m - Function to get the category of the data file
        
        - GetEMGFileNames.m - Function to read the list of raw EMG data file into a cell
    
    **generatedFeatures**: Saves the generated features (cTDD or fTDD) for trials 1 and 2 position 1 to 5. 
    
        - Format - [(number of data samples), (number of features x number of electrodes)]; 
                    number of features = 6 (example)
                    number of electrodes = 7 (known)

# References

[1] R. N. Khushaba, Maen Takruri, Jaime Valls Miro, and Sarath Kodagoda, "Towards limb position invariant myoelectric pattern recognition using time-dependent spectral features", Neural Networks, vol. 55, pp. 42-58, 2014.

[2] R. N. Khushaba, A. Al-Ani, A. Al-Timemy, A. Al-Jumaily, "A Fusion of Time-Domain Descriptors for Improved Myoelectric Hand Control", ISCIT2016 Conference, Greece, 2016.pdf here: https://pdfs.semanticscholar.org/4730/98af39c66b0a4b541860a1f4617c036d8249.pdf

[3] A. Al-Timemy, R. N. Khushaba, G. Bugmann, and J. Escudero, "Improving the Performance Against Force Variation of EMG Controlled Multifunctional Upper-Limb Prostheses for Transradial Amputees", IEEE Transactions on Neural Systems and Rehabilitation Engineering, DOI: 10.1109/TNSRE.2015.2445634, 2015.

[4] Mukhopadhyay, A. K., & Samui, S. (2020). An experimental study on upper limb position invariant EMG signal classification based on deep neural network. Biomedical signal processing and control, 55, 101669.

[5] Aqeel Shaikh, A., Mukhopadhyay, A. K., Poddar, S., & Samui, S. (2022). Towards Power-Efficient Design of Myoelectric Controller based on Evolutionary Computation. arXiv e-prints, arXiv-2204.
