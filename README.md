# CLAHE

CLAHE was used in this study to improve the image's contrast and features by making abnormalities more noticeable. Among the histogram equalization family, Contrast Limited Adaptive Histogram Equalization (CLAHE) is more natural in appearance and useful in the reduction of noise amplification, and we have investigated CLAHE and applied it to our dataset as shown in {Figure \ref{fig:3}}. A full explanation of the CLAHE approach is given below to demonstrate its effectiveness:

1.) The generation of the image transformation using the bin value of the histogram is the first stage of the CLAHE technique.

2.) Following that, using clip boundary, the contrast is confined to a binary count from 0 to 1. Before the image segment is processed, the clip boundary is added to the image. 

3.) To prevent mapping background areas to gray scale, a specific bin value from the histogram region is used to create the entire image region. Clip boundary is used with the help of histogram clip to obtain better mapping.

4.) Finally, the finished CLAHE image is created by computing the image's regions, then extracting, mapping, and interpolating all of the image pixels to get the most out of the image.


This is the code for preproessing original image(s) to CLAHE image(s). This code will help researcher process their images into CLAHE  images. This code process single and multiple images in a folder and save them in another folder. Kindly ensure that the right directory path is called properly. The result of the code is presented below:



![65](https://user-images.githubusercontent.com/61402731/149647964-01de8663-e9b4-469a-83b0-42eaa919b2ee.jpg)
Original CXR image




![65_1_CLAHE](https://user-images.githubusercontent.com/61402731/149647965-a4de1f1b-694b-43a5-a173-9e7c825646f1.jpg)
CLAHE CXR image
