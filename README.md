# Tensorflow Object Detection Walkthrough
This repository provides a comprehensive set of notebooks for training and utilizing custom object detection models using the Tensorflow Object Detection API. The content is designed to complement the Tensorflow Object Detection course available on YouTube.

Steps
Create a Virtual Environment
Create a new virtual environment using the following commands:

bash
Copy code
python -m venv tfod1
Activate the Virtual Environment
Activate the virtual environment based on your operating system:

bash
Copy code
# Linux
source tfod1/bin/activate

# Windows
.\tfod1\Scripts\activate
Install Dependencies and Add Virtual Environment to Python Kernel
Upgrade pip, install ipykernel, and add the virtual environment to the Python Kernel:

bash
Copy code
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=tfodj
Collect Images
Use the provided Notebook (Image Collection.ipynb) to collect images. Ensure you change the kernel to the virtual environment.

Divide Collected Images
Manually divide the collected images into two folders: train and test. Place them in the following directories:

TFODCourse/Tensorflow/workspace/images/train
TFODCourse/Tensorflow/workspace/images/test
Begin Training
Open Notebook (Training and Detection.ipynb) to initiate the training process. This notebook guides you through installing Tensorflow Object Detection, making detections, and saving/exporting your model.

Verify Successful API Installation
Ensure the Tensorflow Object Detection API is installed successfully. You should receive a notification with the last line stating "OK." If issues arise, refer to the Error Guide.md in this folder for troubleshooting.

Train the Model
Within the notebook, choose to train the model. Note that training inside a separate terminal on a Windows machine allows you to display live loss metrics.

Evaluate the Model with Tensorboard
Optionally, evaluate your model using Tensorboard. After training and running the evaluation command, navigate to the evaluation folder for your trained model (e.g., Tensorflow/workspace/models/my_ssd_mobnet/eval). Open Tensorboard with the following command:

bash
Copy code
cd Tensorflow/workspace/models/my_ssd_mobnet/eval
tensorboard --logdir=.
Tensorboard will be accessible through your browser, displaying metrics such as mAP (mean Average Precision) and Recall.

Additional Notes
For more in-depth troubleshooting, please refer to the Error Guide.md in this folder.

Happy training!
