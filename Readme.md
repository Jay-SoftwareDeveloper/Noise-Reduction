# Read Me File Instructions:


To run the provided scripts, open the project folder in a Python-compatible IDE such as Visual Studio Code or a Jupyter environment. Each script is preset with default paths to our dataset. For the DFT and Gaussian scripts, adjust the image path variables to test different images. The CNN model script will train using the "Clean-10" and "Noise-10" datasets and save the trained model to the designated path. To evaluate the trained model, use the provided test image path, which you can modify as needed. For a comprehensive assessment, execute the graph scripts to visualize the performance metrics: MSE, SNR, SSIM, and PSNR. Ensure all scripts are run in the specified order and adhere to the directory structure outlined in the documentation for seamless operation.

## Script Execution Instructions:

Programming Language and Version:

Language: Python
Version: 3.12.2

Installation and Setup:

1. Ensure Python 3.12.2 is installed on your system.
2. Clone the repository or download the source code to your local machine.
3. Navigate to the code directory where the script is located.

Configuring the Code Environment

1. Install the required packages:
   
   pip install numpy matplotlib scikit-image scikit-learn
   

2. Dataset Information
     Dataset name: Dataset
     Contains 4 folders: 
   1. Clean-10 (Clean images)
   2. Noisy-10 (Noisy images)
   3. Denoised
   4. DenoisingCNN_Model1.pth

Preparing the Dataset
1. Download the dataset.
2. Unzip the dataset into the directory where the script is located. Ensure the folders Clean-10 and Noisy-10 are in the same directory as the script.
3. The script is set up to automatically detect and use images from these folders.


File hierarchy:

1.DFT(ButterWorth)
2.CNN Model
3.Save CNN model
4.Test CNN Model
5.DFT(Gaussian Model)
6.Evaluation Metrics Graphs

## Running the Code

To run the code, simply execute the script after navigating to its directory:



### Running the Code

To execute the scripts provided in this project, open the folder in a Python development environment such as Visual Studio Code or a Jupyter notebook. Here's a step-by-step guide on running each component:

1. DFT (Butterworth Filter) Script:
    This script is configured with a default image path. If you want to test it with a different image from the dataset, simply change the noisy_image_path and clean_image_path variables to point to the new image files.
   
   
2. CNN Model Training :
    Run the training script for the CNN model. The script is pre-set to use images from the "Clean-10" and "Noisy-10" datasets. The trained model will be saved in the specified directory within the script.

3. Testing the Trained CNN Model:
    With the CNN model trained, you can now run the testing script. To test the model with a different image, the current path leads to an image that has already been processed by the DFT (Butterworth) filter.  To use a new image, run it through the DFT (Butterworth) model first. The resulting image will be saved in the 'denoised' folder; from there, you can take the new image path and update it accordingly in the script.

4. Gaussian Model Comparison:
   - Execute the Gaussian model script, which is used for comparison purposes. This script also comes with a default example image path set; modify the noisy_image_path and clean_image_path to use a different image for comparison.

5. Graph Generation Scripts:
   - For visual analysis, run the following scripts to generate graphs for evaluation metrics:
      - MSE Graph: This will plot the Mean Squared Error comparisons.
      - SNR Graph: This script plots the Signal to Noise Ratio for each method.
      - SSIM Graph: Execute this to get a graph of the Structural Similarity Index.
      - PSNR Graph: This plots the Peak Signal to Noise Ratio.

Note: It is crucial to follow the file hierarchy as mentioned in the 'File Hierarchy' section to ensure the scripts run correctly. After running each script, the results (graphs or processed images) will be saved to their designated paths as set in the scripts. Be sure to check these paths for your outputs.

