# Backdoor Pruning Defence

## Overview
This code repository is designed to protect machine learning models from backdoor attacks. The defense approach includes selectively pruning activation channels in susceptible layers to strengthen the model against potential manipulation by backdoor patterns. Furthermore, an additional GoodNet model is presented, which identifies anomalies by integrating predictions from both the original Backdoor Model and the Repaired Backdoor Model.

## Requirements

`pip install -r requirements.txt`

## Dataset

- Download the validation and test datasets from [here](https://drive.google.com/drive/folders/13o2ybRJ1BkGUvfmQEeZqDo1kskyFywab?usp=sharing) and store them under **data/** directory.
- The dataset comprises images sourced from the YouTube Aligned Face Dataset, consisting of 1283 individuals, each with 9 images in the validation dataset. The test images with a sunglasses trigger activating the backdoor for sunglasses_bd_net.h5 are stored in sunglasses_poisoned_data.h5. 
- Similarly, there are other .h5 files containing poisoned data corresponding to different BadNets in the models directory.
