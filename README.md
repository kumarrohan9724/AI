Image Enhancement Project
=========================

Overview
--------

This project focuses on image enhancement using a combination of techniques, including color space transformation, 2D Discrete Wavelet Transform (DWT), and Contrast Limited Adaptive Histogram Equalization (CLAHE). The main goal is to improve the visual quality of images while preserving important details.

Table of Contents
-----------------

-   [Installation](https://chat.openai.com/c/beeab78b-673b-45f2-96db-4d5b61bbd315#installation)
-   [Usage](https://chat.openai.com/c/beeab78b-673b-45f2-96db-4d5b61bbd315#usage)
-   [Methods](https://chat.openai.com/c/beeab78b-673b-45f2-96db-4d5b61bbd315#methods)
-   [Results](https://chat.openai.com/c/beeab78b-673b-45f2-96db-4d5b61bbd315#results)
-   [License](https://chat.openai.com/c/beeab78b-673b-45f2-96db-4d5b61bbd315#license)

Installation
------------

To use this image enhancement tool, follow these steps:

1.  Clone the repository to your local machine:

    bashCopy code

    `git clone https://github.com/your-username/image-enhancement-project.git
    cd image-enhancement-project`

2.  Install the required dependencies:

    bashCopy code

    `pip install -r requirements.txt`

Usage
-----

Ensure you have the required image file (`pexels-guilherme-rossi-1668928.jpg` in this case) in the project directory. Modify the `image_enhancement` function call at the end of the script to specify your image file.

pythonCopy code

`if __name__ == '__main__':
    start_time = time.time()
    image_enhancement('your_image.jpg')`

Run the script:

bashCopy code

`python image_enhancement.py`

Methods
-------

The main method for image enhancement is the `image_enhancement` function. This function utilizes various image processing techniques, including:

-   RGB to HSV color space transformation
-   2D Discrete Wavelet Transform (DWT) on the 'Value' channel of HSV
-   Contrast Limited Adaptive Histogram Equalization (CLAHE) on the approximated coefficient (cA) of DWT
-   Inverse DWT to reconstruct the enhanced 'Value' channel
-   HSV to RGB color space transformation
-   Visualization of the original image, 2D DWT decomposition, CLAHE on cA, and the final enhanced image

Results
-------

The script provides similarity measurements such as Mean Squared Error (MSE) and Peak Signal-to-Noise Ratio (PSNR) for each channel (R, G, B) of the image. Additionally, it generates visualizations of the original image, 2D DWT decomposition, CLAHE on cA, and the enhanced image.

License
-------

This project is licensed under the [MIT License](https://chat.openai.com/c/LICENSE).

Feel free to experiment with different images and parameters to explore the capabilities of the image enhancement techniques implemented in this project.
