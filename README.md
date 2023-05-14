# Testing-Impact-of-ESRGAN-on-Image-Classification
Our research aims to investigate the impact of using the proposed techniques (ESRGAN and PSNR-oriented RRDB) as a preprocessing step on the performance of an image classifier model when applied on noisy images. Our hypothesis is that by preprocessing the noisy images with the proposed techniques, the quality of the images will be improved and the image classifier model will perform better. This is because the techniques should enhance the image quality, making them closer to their original counterpart, which are considered the optimal input for the classifier.

To properly test our hypothesis, it was essential to ensure that the outcomes are not influenced by any other factors apart from image resolution. Our approach was to assess the effect of image resolution on the task of Image Classification using three major neural network architectures that have made significant contributions in recent times, namely 19-layer VGGNet, 50-layer ResNet, and MobileNet. We implemented the three network architectures on three different datasets as our benchmarks to evaluate and monitor how image resolution can affect the accuracy across nine different architecture-dataset combinations.

We then created multiple versions of each dataset. Specifically, we generated four distinct versions of each dataset: the original dataset, a noisy version created by downsampling the images with a factor of 0.25 using MATLAB bicubic interpolation, an ESRGAN-enhanced version, and a PSNR-oriented-enhanced version. In total, we produced 12 different datasets. We employed the three classification network architectures mentioned earlier on each of the 12 datasets, resulting in 36 distinct architecture-dataset-resolution combinations.

Results were as follows:

<img width="688" alt="image" src="https://github.com/hagarshalabyy/Testing-Impact-of-ESRGAN-on-Image-Classification/assets/83888834/beec2801-e72a-4c99-99bb-f76ff5f3dde1">


![image](https://github.com/hagarshalabyy/Testing-Impact-of-ESRGAN-on-Image-Classification/assets/83888834/0f05a8ed-760e-43b6-805b-abf46a7734fd)


