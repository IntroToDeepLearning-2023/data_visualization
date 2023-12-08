# Crop Type Mapping in Africa: Ghana

This repository contains code for visualizing randomly selected npy and truth images from the Africa crop type mapping dataset, focusing on Ghana. The images represent crop type classifications.

## Prerequisites

Make sure you have the following libraries installed:

\`\`\`bash
pip install numpy matplotlib
\`\`\`

## Usage

Clone the repository:
\`\`\`bash
git clone https://github.com/your-username/your-repository.git
cd your-repository
\`\`\`

Run the provided Python script:
\`\`\`bash
python visualize_images.py
\`\`\`
This script loads random npy and truth images, displays them in a subplot grid, and saves the figure as images.png.

## File Structure

- `visualize_images.py`: Python script for visualizing npy and truth images.
- `/content/data/africa_crop_type_mapping/ghana/npy`: Directory containing npy files.
- `/content/data/africa_crop_type_mapping/ghana/truth`: Directory containing truth files.

## Additional Notes

- The color mapping for npy images is grayscale.
- Images are randomly selected for demonstration purposes.
- Adjustments can be made to the script for different configurations or use cases.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
