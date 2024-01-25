# Supplementary Material for IEEE ICIP 2024
Supplementary Material for IEEE ICIP 2024
**A Dictionary Based Approach For Removing Out-Of-Focus Blur** <br />
Authors: <samp>{aurangau, anil.kokaram}@tcd.ie</samp>

## Abstract
The field of image deblurring has seen tremendous progress with the rise of deep learning models. These models, albeit efficient, are computationally expensive and energy consuming. Dictionary based learning approaches have shown promising results in image denoising and Single Image Super-Resolution. We propose an extension of the Rapid and Accurate Image Super-Resolution (RAISR) algorithm introduced by Isidoro, Romano and Milanfar for the task of out-of-focus blur removal. We define an image quality index measure which aligns well with the perceptual quality of an image. A metric based blending strategy based on asset allocation strategies is also proposed. Our method demonstrates an average increase of approximately 13% (PSNR) and 10% (SSIM) compared to popular deblurring methods. Furthermore, our blending scheme curtails ringing artefacts post restoration.

## Filter Learning Algorithm

## Index J

## Results

| ![Image 1](Superimposed_Images/face_original_superimposed.png) | ![Image 2](Superimposed_Images/face_blurred_superimposed.png) | ![Image 3](Superimposed_Images/face_restormer_superimposed.png) |
| --- | --- | --- |
| Original Image | Blurry Image | Restormer |

| ![Image 4](Superimposed_Images/face_ifan_superimposed.png) | ![Image 5](Superimposed_Images/face_NBDNet_superimposed.png) | ![Image 6](Superimposed_Images/face_L_superimposed.png) |
| --- | --- | --- |
| IFAN | NBDNet | Landweber |

| ![Image 7](Superimposed_Images/face_NAL_superimposed.png) | ![Image 8](Superimposed_Images/face_PCL_superimposed.png) | ![Image 9](Superimposed_Images/face_RAID_superimposed.png) |
| --- | --- | --- |
| NA Landweber | PC Landweber | Ours |

### Comparison of Moore-Penrose Pseudoinverse and Least Squares Solver

## Metric Q based blending strategy
| ![Original Image](Blending_Images/flower_original_superimposed.png) | ![Patch13](Blending_Images/flower_P13_superimposed.png) | ![Image 3](Blending_Images/flower_iter0_superimposed.png) |
| --- | --- | --- |
| Original Image | Image restored with P=13 | Averaging |

| ![Original Image](Blending_Images/flower_iter1_superimposed.png) | ![Patch13](Blending_Images/flower_iter2_superimposed.png) | ![Image 3](Blending_Images/flower_iter3_superimposed.png) |
| --- | --- | --- |
| Iteration 1| Iteration 2 | Iteration 3 |

## References

## Acknowledgments
