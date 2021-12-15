# DL-CMB_Labeler
Code and trained models for deep learning-based CMB detection.

**Directories:**
python_code: deep CNN implementation, training, testing and prediction code.
matlab_code: essential matlab code to prepare data for training, testing and prediction.
final_models: trained model weights and demo data.

**Usage:**

1. Run Lupo-Lab/CMB_Labeler with 'semion' (user-guided GUI for FP reduction) or 'semioff'.
2. Generate .mat data for CNN (See matlab code example. the .mat requires two fields: 'centroids' and 'swi', see demo data)
3. Run CNN (in virtualenv/conda):

cd python_code
python predict.py MAT_FILE_PATH

The result will be added to the original .mat file.
