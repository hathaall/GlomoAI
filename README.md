# Thyroid Cancer Classification

This repository contains a deep learning model for classifying thyroid images as cancerous or non-cancerous using TensorFlow and OpenCV.

## Running in Google Colab

This project is designed to run seamlessly in **Google Colab**. Follow these steps to set it up and run it in a Colab environment:

### Step 1: Open Google Colab
1. Go to [Google Colab](https://colab.research.google.com/).
2. Click on **File** > **Upload notebook** and upload this repository, or just create a **New Notebook**.

### Step 2: Open the Notebook
Upload `GlomoAI.ipynb` from this repository into Google Colab.

### Step 3: Upload the Dataset
1. Zip your local `thyroid_dataset` folder so you have `thyroid_dataset.zip`.
2. In Colab, click the **Folder icon** on the left sidebar to open the Files panel.
3. Click the **Upload** icon and select your `thyroid_dataset.zip` file.
4. The notebook already contains a cell to unzip this file automatically:
   ```bash
   !unzip -q thyroid_dataset.zip -d ./
   ```
   *Make sure the dataset extracts into the current directory with `Cancerous` and `non_Cancerous` subfolders.*

### Step 4: Run the Script
1. Run the cell containing the Python code. 
2. The model will compile and begin training for 10 epochs.
3. Once training is complete, a prompt will appear asking you to upload an image.
4. Choose an image from your computer to test the model. It will predict whether the image is cancerous or non-cancerous and display a prediction score!

---
*Note: Since Colab already comes pre-installed with TensorFlow, OpenCV (`cv2`), and NumPy, you do not need to install any additional dependencies.*
