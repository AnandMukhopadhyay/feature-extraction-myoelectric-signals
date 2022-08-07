# feature-extraction-myoelectric-signals

Structure

Folders
    - codes:
        - S01_main_data_generation.mlx - main script. Need to select type of feature extraction - cTDD or fTDD
        - batch12.mlx - Function for trial 1 data recordings
        - batch22.mlx - Function for trial 2 data recordings
        - getcTDDfeat.mlx - Function to computes cTDD features using same window
        - getfTDDfeat.mlx - Function to computes fTDD features using nearby windows decided by step factor
        - getCategory.m - Function to get the category of the data file
        - GetEMGFileNames.m - Function to read the list of raw EMG data file into a cell
    - data: contains the raw filtered data samples for Subject S4 of Khushaba dataset 6
    - generatedFeatures: Saves the generated features (cTDD or fTDD) for trials 1 and 2 position 1 to 5. Format - 
        [(number of data samples), (number of features x number of electrodes)] 
        number of features = 6 (example)
        number of electrodes = 7 (known)

