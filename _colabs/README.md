# colab demos
Few baselines for the Change Detection task


## 0_oneraCD_rgb_simpleUnet.ipynb

First running version of the U-NET model trained on tiled (64x64) dataset subset (taking only samples with more change present, and only rgb).

Inputs from image 1 and image 2 are differenced before being sent to the U-NET (this can be done better with SiamU-NET).

Super simple first version that works ...
