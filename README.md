# 2D Digital Colorful Image Code Using FFT 2D

This repository contains Python code implemented in Jupyter Notebook for generating a colorful down-sampled image from a 2D square-sized colorful image using the 2D Fast Fourier Transform (FFT) algorithm.


## Table of Contents
- [Introduction](#introduction)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Algorithm Overview](#algorithm-overview)
- [Example](#example)
- [License](#license)

## Introduction

The 2D Fast Fourier Transform (FFT) algorithm is a widely-used technique in signal processing and image analysis. It allows us to transform an image from the spatial domain to the frequency domain, enabling various operations such as filtering, compression, and enhancement.

This code focuses on down-sampling a colorful image using the 2D FFT algorithm. By applying the FFT and reducing the size of the frequency domain representation, we can achieve a down-sampled version of the original image while preserving important visual features.

## Requirements

To run the code, you need the following dependencies:
- Python (3.9 recommended)
- Jupyter Notebook
- NumPy
- OpenCV (cv2)

You can install Python from the official Python website: https://www.python.org/downloads/

Jupyter Notebook can be installed using pip, the Python package installer, with the following command:

```
pip install jupyter notebook
```

## Installation

To use the code, follow these steps:

1. Clone this repository to your local machine or download the ZIP file and extract it.

2. Open a terminal or command prompt and navigate to the directory where you cloned or extracted the repository.

3. Launch Jupyter Notebook by executing the following command:

```
jupyter notebook
```

4. In the Jupyter Notebook interface, navigate to the directory where you cloned or extracted the repository and open the `Colorful_Downsampling_method3.ipynb` notebook.

## Usage

The Jupyter Notebook contains the code for down-sampling a colorful image using the 2D FFT algorithm. It includes the following sections:

1. Importing Dependencies: This section imports the required Python libraries for image manipulation and FFT operations.

2. Loading and Displaying an Image: Here, you can specify the path to the input image and visualize it using matplotlib.

3. Transforming the Image: This section performs the 2D FFT on the image and separates the magnitude and phase components.

4. Down-sampling the Image: The magnitude and phase components are down-sampled by a scale factor of 2 to reduce the size of the frequency domain representation.

5. Inverse Transform and Visualization: This part combines the modified magnitude and phase components and performs the inverse 2D FFT to obtain the down-sampled image. The resulting image is then displayed using matplotlib.

Feel free to modify the code and experiment with different images and scale factors to generate your own down-sampled colorful images.

## Algorithm Overview

The algorithm implemented in this code can be summarized as follows:

1. Load the input 2D square-sized colorful image.

2. Perform the 2D FFT on the image to obtain its frequency domain representation.

3. Separate the magnitude and phase components of the Fourier coefficients.

4. Down-sample the magnitude and phase components by a scale factor of 2, reducing the size of the frequency domain representation.

5. Reconstruct the Fourier coefficients using the modified magnitude and phase components.

6. Perform the inverse 2D FFT on the reconstructed Fourier coefficients to obtain the down-sampled image.

7. Visualize and save the down-sampled image.

The code provides flexibility to experiment with different images and scale factors, allowing you to explore the impact of down-sampling on colorful images.



## Example

To illustrate the usage of the code, we provide an example that demonstrates how to down-sample a colorful image by a scale factor of 2.

1. Specify the path to the input image:

```python
input_image_path = "path/to/input.jpg"
```

2. Run the code in the Jupyter Notebook, and the resulting down-sampled image will be displayed.

3. You can save the down-sampled image by uncommenting and modifying the following line:

```python
# cv2.imwrite("output_image.jpg", downsampled_image)
```

Feel free to experiment with different images and scale factors to explore the effects of down-sampling on colorful images.

## License

The code in this repository is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the code for personal and commercial purposes. However, the code is provided "as is" without any warranty.
