This is a repository for paper "Machine Learning-Assisted Prediction of Ground- and Excited-State Redox Potentials in Iridium(III) Photocatalysts".
# PC-Ir-ML: Machine Learning Models for Predicting Redox Potentials of Ir Photocatalysts

This repository contains the machine learning models and code used to predict the ground- and excited-state redox potentials of Ir(III) photocatalysts. The project is organized into folders for each of the six models developed in the paper, with code for model selection, optimization, and final model evaluation.

## Repository Structure
- `Gox/`  
  Contains the model selection and optimization notebooks for the first model, as well as the final trained model saved in a `joblib` file.
- `Gred/`  
  Contains the model selection and optimization notebooks for the second model, as well as the final trained model saved in a `joblib` file.
- `Eox/`  
  Contains the model selection and optimization notebooks for the third model, as well as the final trained model saved in a `joblib` file.
- `Ered/`  
  Contains the model selection and optimization notebooks for the fourth model, as well as the final trained model saved in a `joblib` file.
- `Model_G/`  
  Contains the model selection and optimization notebooks for the fifth model, as well as the final trained model saved in a `joblib` file.
- `Model_E/`  
  Contains the model selection and optimization notebooks for the sixth model, as well as the final trained model saved in a `joblib` file.

Each folder includes:
- **Model Selection (`model_selection.ipynb`)**: This notebook demonstrates how different algorithms and hyperparameters were tested to select the best model.
- **Model Optimization (`model_optimization.ipynb`)**: This notebook shows the optimization process to fine-tune the selected model's performance.
- **Final Model (`final_model.joblib`)**: The trained model saved in `.joblib` format for easy loading and inference.

## How to Use
1. Clone or download this repository to your local machine.
2. Install the required Python packages by using the provided `requirements.txt` or manually.
3. Navigate to the desired model folder, and open the corresponding `.ipynb` files in Jupyter Notebook or JupyterLab.
4. Follow the steps in the notebooks for model selection, optimization, and evaluation.
