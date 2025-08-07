# **INAF**
<img width="975" height="564" alt="image" src="https://github.com/user-attachments/assets/b3190e3b-2751-4b81-afbd-c15b00addab1" />

Iterative Neural Alignment with Feedback **(INAF)** is an AI-enabled framework for precise image calibration. The identified calibration parameters can be used structural condition assessment as presented in the paper. This repository provides starter code to implement the framework's algorithm and train the alignment and feedback networks on custom dataset. If you find this repository useful, please site the paper *"AI-enabled Image calibration for Non-contact Structural Condition Assessment"*.

# **Install dependencies** 
Run the *"requirements.txt"* to install neccessary libraries, a virtual environment is recommended:
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

# **Generate the dataset** 
1. Manually calibrate the baseline image as presented in the paper. An example calibrated baseline image for the UIUC Smart bridge is avalibale in the **"codes"** directory.
2. Run the **"datagenNotebook.ipynb"** notebook to generate the dataset.

# **Train the ALignment and Feedback networks**
1. Download the pretained weights for the alignment and feedback networks provided in the releasese **"INAF_pretrained_weights"**.
2. Run the **"trainINAF.ipynb"** notebook to train both the alignment and feedback networks.

# **Run INAF to calibrate query image(s)**
1. Run the **"runINAF.ipynb"** notebook available in the codes directory to calibrate query images. Provide the directory to the fine-tuned models.
2. Download the **"updateGBDT.txt"** file into your **"Blender*** model hosting the GBDT to update the texture for condition assessment.
