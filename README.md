# change_detection_onera_baselines
Few baselines for the Change Detection task


## Dataset

Onera Satellite Change Detection Dataset - https://rcdaudt.github.io/oscd/

Loading with a subset of all available channels (only rgb vs more channels). Possibly filtering tiles to balance samples with more changes (or maybe re-weight losses later).

## Methods

U-Net based models, simple concatenation or difference between two images as inputs

Later Siamese version of U-Net - see also: https://github.com/previtus/ChangeDetectionProject with https://github.com/previtus/ChangeDetectionProject/blob/ad2bd4adb2df7a2125b0737af385572d2d743e75/Model2_builder.py#L37 - these however worked with older version of the segmentation_models library

## Libraries

Segmentation models: https://github.com/qubvel/segmentation_models

## Metrics

Plans to have them comparable with "Fully Convolutional Siamese Networks for Change Detection" (https://arxiv.org/abs/1810.08462) or perhaps also using AUC as a non-thresholded metric.
