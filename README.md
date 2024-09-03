# Image-Compression-Using-Singular-Value-Decomposition-SVD


Image compression is a crucial technique in modern digital media, allowing us to reduce the size of image files while retaining as much quality as possible. In this project, we explore the application of Singular Value Decomposition (SVD) to compress images efficiently. SVD is a powerful linear algebra tool that breaks down an image into its fundamental components, enabling us to approximate the original image with fewer data points.

## Singular Value Decomposition (SVD)
Singular Value Decomposition (SVD) is a mathematical technique that factors a matrix \( A \) into three distinct matrices:

$$A = U \Sigma V^T$$

- ** $U$ **: An orthogonal matrix representing the left singular vectors.
- **$\Sigma$**: A diagonal matrix containing the singular values, which represent the magnitude of each component.
- **$V^T$**: An orthogonal matrix representing the right singular vectors.

In the context of image compression, the matrix \( A \) represents the pixel intensity values of the image. By retaining only the largest singular values in \( \Sigma \), we can reconstruct an approximation of the original image with significantly reduced data, effectively compressing the image.

## Project Overview
This project demonstrates the use of SVD in image compression through the following steps:

1. **Matrix Construction**: We begin by constructing a simple binary matrix and applying SVD to understand the basic concepts.

2. **SVD Decomposition**: SVD is applied to decompose the matrix into its component matrices \( U \), \( \Sigma \), and \( V^T \). The importance of each singular value is analyzed by reconstructing the matrix using varying numbers of singular values.

3. **Image Compression**: The SVD technique is then applied to a grayscale image. By retaining only the most significant singular values, we achieve a compressed version of the original image.

4. **Noise Analysis**: We introduce random noise into the image to study the robustness of SVD in image reconstruction. The effect of noise on the singular values and the quality of the reconstructed image is examined.

5. **Visualization**: The project includes visualizations of the singular values, their cumulative sum, and the reconstructed images at different compression levels. This helps in understanding the trade-offs between compression ratio and image quality.

## Results
- **Singular Value Analysis**: The singular values are plotted to show their contribution to the image data. Most of the image information is captured by the largest singular values, which allows for significant compression with minimal loss in quality.
  
- **Image Reconstruction**: Images reconstructed with a reduced number of singular values demonstrate the effectiveness of SVD in compressing images. As the number of retained singular values increases, the quality of the reconstructed image improves, closely approximating the original.

- **Noise Impact**: The analysis shows that SVD can partially mitigate the effects of noise, as the most significant singular values still dominate the image structure, even in the presence of noise.

## Conclusion
This project illustrates how Singular Value Decomposition can be leveraged for image compression. By focusing on the most significant singular values, we can achieve high levels of compression with minimal loss in image quality. Additionally, SVD shows resilience to noise, making it a robust choice for image processing tasks.

## Acknowledgments
This work is inspired by the wide applications of SVD in data science, signal processing, and image compression. Special thanks to the open-source community for providing the tools and libraries that made this project possible.
