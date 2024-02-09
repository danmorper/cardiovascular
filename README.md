# Medical Image Analysis with Python

## Overview
This project focuses on the analysis of medical images, specifically CT scans, using Python. It delves into various aspects of medical imaging, such as understanding CT images, Hounsfield units, windowing, anatomical planes, voxel manipulation, affine transformations, and the application of techniques like Maximum Intensity Projection (MIP) and volume calculation. We also explore the use of the NIfTI format and the NiBabel library for handling medical image data.

## Getting Started

### Prerequisites
- Python 3.x
- Libraries: nibabel, numpy, matplotlib, scipy

### Installation
Install the required Python libraries using pip:
```bash
pip install nibabel numpy matplotlib scipy
```

## Loading and Analyzing a CT Image
Load a CT image in NIfTI format and access its metadata:

```python
import nibabel as nib

# Load the NIfTI image
nifti_img = nib.load('path_to_your_nifti_file.nii')

# Access the image header
header = nifti_img.header

# Print the affine matrix
print(nifti_img.affine)

# Access the image data
data = nifti_img.get_fdata()
```

## Affine Transformations
Demonstrate how to apply affine transformations to adjust the orientation and position of the image data.

## MIP and Volume Calculation
Implement MIP to visualize the 3D image data in 2D and calculate the volume of specific structures within the image, such as the aorta.

## Usage Examples
Include examples of how to use the project for common tasks, such as rescaling images, applying MIP, and calculating volumes.

