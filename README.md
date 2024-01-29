# Supplementary Material for IEEE ICIP 2024
Supplementary Material for IEEE ICIP 2024
**A Dictionary Based Approach For Removing Out-Of-Focus Blur** <br />
Authors: <samp>{aurangau, anil.kokaram}@tcd.ie</samp>

## Abstract
The field of image deblurring has seen tremendous progress with the rise of deep learning models. These models, albeit efficient, are computationally expensive and energy consuming. Dictionary based learning approaches have shown promising results in image denoising and Single Image Super-Resolution. We propose an extension of the Rapid and Accurate Image Super-Resolution (RAISR) algorithm introduced by Isidoro, Romano and Milanfar for the task of out-of-focus blur removal. We define an image quality index measure which aligns well with the perceptual quality of an image. A metric based blending strategy based on asset allocation strategies is also proposed. Our method demonstrates an average increase of approximately 13% (PSNR) and 10% (SSIM) compared to popular deblurring methods. Furthermore, our blending scheme curtails ringing artefacts post restoration.

## Filter Learning Algorithm

## Index J
| ![Image 1](IndexJ_Experiments/barbara_original.png) | ![Image 2](IndexJ_Experiments/barbara_p13_restored.png) |
| --- | --- |
| Original Image, J = 1.0 | Image Restored with a patch size of 13, J = 0.7031 |

| ![Image 1](IndexJ_Experiments/barbara_blurred.png) | ![Image 2](IndexJ_Experiments/barbara_p21_rsetored.png) |
| --- | --- |
| Blurry Image, J = 0.0 | Image Restored with a patch size of 21, J = 0.7796 |


## Results

### Tabular Results 
Set14[] and set5 were used to measure the performance of our algorithm against popular restoration techniques. 
#### Set14
| Algorithm | PSNR (dB) | SSIM |
| --- | --- | --- |
| IFAN | 23.100 | 0.653 | 
| Restormer | 24.566 | 0.723 | 
| NBDNet | 27.280 | 0.754 | 
| Landweber | 26.263 | 0.757 | 
| NA Landweber | 26.291 | 0.758 | 
| PC Landweber | 27.732 | 0.820 | 
| Ours | 29.287 | 0.847 | 

### Set 5
| Algorithm | PSNR (dB) | SSIM |
| --- | --- | --- |
| IFAN | 25.409 | 0.789 | 
| Restormer | 26.645 | 0.823 | 
| NBDNet | 31.036 | 0.869 | 
| Landweber | 29.011 | 0.849 | 
| NA Landweber | 30.019 | 0.867 | 
| PC Landweber | 30.715 | 0.890 | 
| Ours | 31.999 | 0.900 | 

### Visual Comparison 
| ![Image 1](Superimposed_Images/face_original_superimposed.png) | ![Image 2](Superimposed_Images/face_blurred_superimposed.png) | ![Image 3](Superimposed_Images/face_restormer_superimposed.png) |
| --- | --- | --- |
| Original Image | Blurry Image | Restormer |

| ![Image 4](Superimposed_Images/face_ifan_superimposed.png) | ![Image 5](Superimposed_Images/face_NBDNet_superimposed.png) | ![Image 6](Superimposed_Images/face_L_superimposed.png) |
| --- | --- | --- |
| IFAN | NBDNet | Landweber |

| ![Image 7](Superimposed_Images/face_NAL_superimposed.png) | ![Image 8](Superimposed_Images/face_PCL_superimposed.png) | ![Image 9](Superimposed_Images/face_RAID_superimposed.png) |
| --- | --- | --- |
| NA Landweber | PC Landweber | Ours |

### Average Blur
Size = 3 * 3
| ![Image 100](Box_Blur_Comparison/barbara_original.png) | ![Image 101](Box_Blur_Comparison/barbara_blurred_3_box.png) | ![Image 102](Box_Blur_Comparison/barbara_restored_3_box.png)  |
| --- | --- | --- |
| Original Image| Blurry Image | Restored Image |

### Comparison of Moore-Penrose Pseudoinverse and Least Squares Solver

| ![Image 10](MP_LS_Comparison/img_001_SRF_2_HR_original.png) | ![Image 11](MP_LS_Comparison/img_001_SRF_2_HR_blurred.png) |
| --- | --- |
| Original Image | Blurry Image |

| ![Image 12](MP_LS_Comparison/img_001_SRF_2_HR_LeastSquares_restored.png) | ![Image 13](MP_LS_Comparison/img_001_SRF_2_HR_MoorePenrose_restored.png) |
| --- | --- |
| Image restored using Least Squares Approach | Image restored using Moore-Penrose Pseudoinverse Approach |


## Metric Q based blending strategy
| ![Original Image](Blending_Images/flower_original_superimposed.png) | ![Patch13](Blending_Images/flower_P13_superimposed.png) | ![Image 3](Blending_Images/flower_iter0_superimposed.png) |
| --- | --- | --- |
| Original Image | Image restored with P=13 | Averaging |

| ![Original Image](Blending_Images/flower_iter1_superimposed.png) | ![Patch13](Blending_Images/flower_iter2_superimposed.png) | ![Image 3](Blending_Images/flower_iter3_superimposed.png) |
| --- | --- | --- |
| Iteration 1| Iteration 2 | Iteration 3 |

## References

## Acknowledgments
