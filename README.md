# PCD Assignment 02

## Image Enhancement Based on Filtering

This repository contains the implementation and analysis for **PCD Assignment 02**.
The project focuses on comparing several image enhancement and filtering methods using Google Colab and Python.

## Objectives

The objectives of this assignment are:

- Implement different image filtering methods.
- Apply filtering methods to different image conditions.
- Compare the visual results of each filtering method.
- Analyze the effectiveness of each method for different image conditions.

## Image Conditions

One original image is used as the main input. From the original image, several different conditions are created:

1. **Original Image**
   - The original image is used as the reference image.

2. **Blurred Image**
   - The image is blurred to reduce image details and sharp edges.

3. **Dark Image**
   - The image intensity is reduced to produce a darker image.

4. **Bright Image**
   - The image intensity is increased to produce a brighter image.

5. **Low-Contrast Image**
   - The intensity range of the image is reduced to produce a low-contrast image.

6. **Salt & Pepper Noise**
   - Salt-and-pepper noise is added to the image to simulate impulsive noise.

## Methods

Several filtering methods are implemented and applied to the different image conditions.

### Spatial Filters

Four spatial filtering methods are implemented:

1. **Smoothing Linear Filter**
   - Uses a linear kernel to average neighboring pixels.
   - Produces a smoother image and reduces small variations.

2. **Gaussian Filter**
   - Uses a Gaussian kernel to smooth the image.
   - Reduces high-frequency components and produces a smooth result.

3. **Median Filter**
   - Replaces a pixel value using the median value of its neighborhood.
   - Useful for reducing impulsive or salt-and-pepper noise.

4. **Laplacian Sharpening**
   - Uses the Laplacian operator to emphasize image details and edges.
   - Can be used to sharpen an image.

### Frequency Domain Filters

Several filters are implemented in the frequency domain using Fourier Transform.

1. **Low Pass Filtering**
   - Preserves low-frequency components and reduces high-frequency components.
   - Produces a smoother image.

2. **High Pass Filtering**
   - Preserves high-frequency components.
   - Emphasizes edges and image details.

3. **Gaussian Low Pass Filter**
   - Uses a Gaussian function in the frequency domain.
   - Produces smooth transitions between passed and rejected frequencies.

4. **Ideal Low Pass Filter**
   - Uses a cutoff frequency to determine which frequency components are preserved.
   - Can produce blurring and ringing effects.

5. **Butterworth Low Pass Filter**
   - Uses the cutoff frequency and filter order to control the frequency response.
   - Provides a smoother transition compared to an Ideal Low Pass Filter.

6. **Ideal High Pass Filter**
   - Removes low-frequency components below the cutoff frequency.
   - Preserves high-frequency components.

7. **Butterworth High Pass Filter**
   - Uses a Butterworth frequency response to preserve high-frequency components.
   - Provides a smoother transition than an Ideal High Pass Filter.

8. **Gaussian High Pass Filter**
   - Uses a Gaussian frequency response to emphasize high-frequency components.
   - Can be used to highlight image details and edges.

9. **Laplacian HPF**
   - Uses the Laplacian operator in the frequency domain.
   - Emphasizes high-frequency components and image details.

### Ringing and Blurring

The experiment also observes the effects of **ringing and blurring** produced by low-pass filtering, particularly with different cutoff frequencies.

## Comparison

The filtering methods are compared visually for the following image conditions:

- **Blurred Image**
- **Dark Image**
- **Bright Image**
- **Low-Contrast Image**
- **Salt & Pepper Noise**

The comparison is used to determine which filtering method is more suitable for each image condition based on the visual appearance of the resulting image.
