
# Crop Type Mapping in Africa: Ghana
##  Running the Visualization

This repository contains code for visualizing randomly selected npy and truth images from the Africa crop type mapping dataset, focusing on Ghana. The images represent crop type classifications.

## Prerequisites

## 1. Installation:

Before running the visualization, you need to install the necessary libraries:

```bash
!pip install visdom==0.1.7 wandb rasterio
!pip install einops
!pip install einsum
```

## 2. Mount Google Drive:

`from google.colab import drive`
`drive.mount('/content/drive')`

## 3. Downloading the Dataset:

The dataset can be downloaded from the provided public shared files on Google Drive. Use the following command to access the files:

`!gsutil ls gs://data_ctm/data/data/africa_crop_type_mapping/ghana/`

To download specific files or the entire directory, use the gsutil command with the appropriate paths. Remember to replace dataset_path with the actual path of the dataset.

`!gsutil -m cp -r gs://data_ctm/data/data/africa_crop_type_mapping/ghana/dataset_path /content/data`

## 4. Data Preprocessing:
The data is stored in .npz files. You can access the data inside the file using libraries like NumPy. Here's an example in Python:

| Field          | Description                                 |
| -------------- | ------------------------------------------- |
| planet         | PlanetScope satellite imagery               |
| s1             | Sentinel-1 satellite data                   |
| s2             | Sentinel-2 satellite data                   |
| s2_cloudmask   | Cloud mask for Sentinel-2 data               |

## 4. Data Transformation and Augmentation:
The visualization process involves transforming single-channel grayscale masks to pseudo-color masks and applying data augmentation techniques (optional). This enhances the visualization and improves data robustness.

## 5. Running the Visualization:
The actual visualization code needs to be implemented and placed within the Python script. This code will utilize the loaded data and perform the visualization process.

#### Image
![images](https://github.com/IntroToDeepLearning-2023/data_visualization/assets/44385819/d8be515c-0382-42b9-97b8-9933e9e22482)

## 6. Execution Environment:
Choose an appropriate execution environment based on your needs:

#### File Structure

- `visualize_images.py`: Python script for visualizing npy and truth images.
- `/content/data/africa_crop_type_mapping/ghana/npy`: Directory containing npy files.
- `/content/data/africa_crop_type_mapping/ghana/truth`: Directory containing truth files.

### Additional Notes

- The color mapping for npy images is grayscale.
- Images are randomly selected for demonstration purposes.
- Adjustments can be made to the script for different configurations or use cases.

#### GPU on Google Cloud Platform (GCP):
Configure your environment for GPU usage by running the following command:

`!nvidia-smi`

This will ensure your code utilizes the available GPU resources for faster processing.

### Other environment (CPU, local machine):
No specific configuration is needed. However, running the code on CPU might be slower compared to GPU.

## Run the 

Clone the repository:
`git clone https://github.com/IntroToDeepLearning-2023/data_visualization.git`
`cd your-repository`

Run the provided Python script:
`python visualize_images.py`

This script loads random npy and truth images, displays them in a subplot grid, and saves the figure as images.png.

## 7. Results:
The visualization results will be displayed in the code editor with markdown format. This provides an interactive and clear way to view the output.

## 8. Readme Integration:
Once you're satisfied with the visualization results, you can copy and paste the markdown code into the project's Readme file. This will provide clear instructions and enhance readability for other users.

Important Note:

This is a general overview of the visualization process.

## Contributors

- **Deo Uwimpuhwe**
  - Program: MECE 2024
  - Email: [duwimpuh@andrew.cmu.edu](mailto:duwimpuh@andrew.cmu.edu)

- **Gustave Bwirayesu**
  - Program: MECE 2024
  - Email: [gbwiraye@andrew.cmu.edu](mailto:gbwiraye@andrew.cmu.edu)

- **Eric Maniraguha**
  - Program: MSIT 2024
  - Email: [emanirag@andrew.cmu.edu](mailto:emanirag@andrew.cmu.edu)

- **Bienvenue Jules Himbaza**
  - Program: MECE 2024
  - Email: [hjulesbi@andrew.cmu.edu](mailto:hjulesbi@andrew.cmu.edu)

# Happy Code 😄

*Celebrate the joy of coding and collaboration!* 🚀✨


