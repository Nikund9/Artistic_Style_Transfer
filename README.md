# Artistic_Style_Transfer

**_Note : For running the .ipynb file on google colab make sure to switch the runtime from cpu to gpu
_**

<h2>Key Components</h2>
1. Feature Extraction using VGG19:
Utilizing the VGG19 convolutional neural network, the algorithm extracts pertinent features from images. Specific layers within the VGG model are strategically selected to isolate content and style information.

2. Custom VGG Model Integration:
The repository incorporates a personalized VGG model tailored explicitly for Neural Style Transfer. This specialized model is adept at extracting essential features from designated layers critical for representing both content and style.

3. Image Loading and Pre-processing:
Images are loaded and pre-processed using the PIL library alongside torchvision transformations. This pre-processing ensures that the images align with the requirements of the custom VGG model, ensuring compatibility and optimal feature extraction.

4. Optimization Iteration:
The optimization loop functions by iteratively refining a generated image to minimize losses associated with both content and style. Employing the Adam optimizer, the total loss—a combination of content and style losses—is computed and minimized to enhance the synthesized image iteratively.

<h2>Parameters and Configuration:</h2>
1. total_steps: The total number of optimization steps, controlling the refinement of the stylized image.
2. Alpha and Beta: Weight factors for content and style losses, influencing the importance of each in the total loss calculation.
3. optimizer: Adam optimizer with a learning rate of 0.001 for image optimization.

Base_Image
![image](https://github.com/Nikund9/Artistic_Style_Transfer/assets/85832578/b60d8ff9-4620-4f06-b2e2-80dcde67ae01)

Reference_Image
![image](https://github.com/Nikund9/Artistic_Style_Transfer/assets/85832578/01795cf9-8d5f-4f5d-bae6-7257bf09c323)

Generated_Image
![image](https://github.com/Nikund9/Artistic_Style_Transfer/assets/85832578/339e2369-2bed-4f59-a040-1c824eb28e02)

