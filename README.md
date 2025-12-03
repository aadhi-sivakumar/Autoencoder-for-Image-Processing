# CS 4375 - Project

## Denoising Autoencoder for Image Processing

### Prerequisites

No local installation required. The notebook runs entirely on Google Colab with pre-installed libraries:

- NumPy
- Matplotlib
- Scikit-learn

### Running the Code on Google Colab

1. Open Google Colab: [https://colab.research.google.com](https://colab.research.google.com)

2. Click on **File → Upload notebook** and upload `ImageProcessing.ipynb`

3. (Optional) For faster execution, enable GPU:
   - Go to **Runtime → Change runtime type**
   - Select **GPU** under Hardware accelerator
   - Click **Save**

4. Run all cells by clicking **Runtime → Run all** or press `Ctrl + F9`

5. The notebook will:
   - Load the Fashion-MNIST dataset (70,000 images)
   - Add Gaussian noise to the images (noise factor = 0.3)
   - Split data into training (80%) and testing (20%) sets
   - Train four autoencoder experiments with different hyperparameters
   - Display training curves and reconstruction results
   - Save experiment results to `experiment_log.csv`

6. To download the results CSV:
   - Click the folder icon on the left sidebar
   - Locate `experiment_log.csv`
   - Right-click and select **Download**


### Expected Output

- Training curves showing loss convergence for each experiment
- Visual comparison of original, noisy, and denoised images
- Best model selection based on lowest test MSE
- CSV file with all experiment results

### Notes

- The entire implementation is from scratch using only NumPy (no deep learning frameworks)
- Training time is approximately 5-10 minutes per experiment on Colab