# **INAF**
<img width="975" height="564" alt="image" src="https://github.com/user-attachments/assets/b3190e3b-2751-4b81-afbd-c15b00addab1" />

Iterative Neural Alignment with Feedback **(INAF)** is an AI-enabled framework for precise image calibration. The identified calibration parameters can be used for structural condition assessment as presented in the paper. This repository provides starter code to implement the framework's algorithm and train the Alignment and Feedback networks on custom dataset. If you find this repository useful, please site the paper *"AI-enabled Image calibration for Non-contact Structural Condition Assessment"*. Contact the author at thomasngare5@gmail.com.

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
1. Run the **"runINAF.ipynb"** notebook available in the **codes** directory to calibrate query images. Provide the directory to the fine-tuned models.
2. Some test images together with backgroud masks is available for Kavita Lalith Bahl Smart bridge, in the **codes** directory.
3. Download the **"updateGBDT.txt"** file into your **"Blender*** model hosting the GBDT to update the texture for condition assessment.

# **Results for SSTL bridge**
**Query #1**
<img width="1622" height="325" alt="image" src="https://github.com/user-attachments/assets/f5247ea2-538b-42d2-b3cb-54b646a39c46" />
**Query #2**
<img width="1415" height="285" alt="image" src="https://github.com/user-attachments/assets/ae6b3136-965d-445b-b9b4-2b4d2390a53c" />
**Query #3**
<img width="1619" height="326" alt="image" src="https://github.com/user-attachments/assets/cfe461f7-0a16-4bf4-90d0-8fa917adbcd0" />
**Query #4**
<img width="1621" height="327" alt="image" src="https://github.com/user-attachments/assets/c87ddc43-3f98-410d-b55b-6575b89df2ce" />
**Query #5**
<img width="1622" height="325" alt="image" src="https://github.com/user-attachments/assets/3a78b571-5573-4aec-9687-a55e4f9c3a3e" />
**Query #6**
<img width="1620" height="325" alt="image" src="https://github.com/user-attachments/assets/eed4b65f-d463-4ca1-87f6-218b9a886846" />

# **Results for Kavita Lalith Bahl Smart bridge UIUC**
**Query #1**
<img width="1625" height="326" alt="image" src="https://github.com/user-attachments/assets/71946e3d-5ce4-4884-a40e-c94197368a1c" />
**Query #2**
<img width="1592" height="321" alt="image" src="https://github.com/user-attachments/assets/009e2c80-0ac9-46e7-b4e3-2c27c0831970" />
**Query #3**
<img width="1618" height="327" alt="image" src="https://github.com/user-attachments/assets/a0be4842-8b70-4ce2-afc7-982ba86d6f70" />
**Query #4**
<img width="1606" height="325" alt="image" src="https://github.com/user-attachments/assets/b1f5b7d2-bab5-4bfc-98e4-97dd7ff4d9c3" />
**Query #5**
<img width="1623" height="323" alt="image" src="https://github.com/user-attachments/assets/3767336d-dc11-427d-9558-4c40e86b2a6c" />

# **Results for Dalles Miter Gate Oregon**
**Query #1**
<img width="993" height="191" alt="image" src="https://github.com/user-attachments/assets/d314b61c-cd00-4603-9f41-8d0cca3e05b3" />
**Query #2**
<img width="1876" height="360" alt="image" src="https://github.com/user-attachments/assets/d9c8ea77-1932-4672-a207-38920e767943" />

