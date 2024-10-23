# Nature Paper PyTorch Implementation: "Rapid identification of pathogenic bacteria using Raman spectroscopy and deep learning"

## Files
2 Jupyter Notebooks are provided:
1. Input intensity waveforms of the bacteria and predicting the output label of the bacteria "DL-PyTorch-CNN-bacteria-prediction.ipynb"
2. Input intensity waveforms of the bacteria while binarizing (combining) output prediction of bacteria into antibiotic groups "DL-PyTorch-CNN-bacteria-antibiotic-prediction.ipynb"

## Datasets
[Dataset-Link-here](https://www.dropbox.com/scl/fo/fb29ihfnvishuxlnpgvhg/AJToUtts-vjYdwZGeqK4k-Y?rlkey=r4p070nsuei6qj3pjp13nwf6l&dl=0)

### Test data
Used to test the model output and ensure it is working correctly. Shape of (3000,1000)
1. Shape 3000 sample
2. Each image is represented with 1000 datapoints (1 second), representing an intensity point each millisecond
```
data/X_test.npy
data/y_test.npy
```

### Reference data
Used to train the model from scratch. Shape of (60000,1000)
Shape breakdown:
1. Shape 60000 sample
2. Each image is represented with 1000 datapoints (1 second), representing an intensity point each millisecond
```
data/X_reference.npy
data/y_reference.npy
```
- With non-binarized bacteria predictions
  ![text](/results/bacteria-prediction-x-ref.png)

- With binarized bacteria predictions
  ![text](/results/binarized-antibiotic-prediction-x-ref.png)

### Finetune data
Used to finetune the model after training on the reference data. Shape of (3000,1000)
1. Shape 3000 sample
2. Each image is represented with 1000 datapoints (1 second), representing an intensity point each millisecond
```
data/X_finetune.npy
data/y_finetune.npy
```
- With non-binarized bacteria predictions
  ![text](/results/bacteria-prediction-x-finetune.png)

- With binarized bacteria predictions
  ![text](/results/binarized-antibiotic-prediction-x-fine-tune.png)


### 2018 & 2019 Clinical data
2018 clinical data has a shape of (10000,1000)
2018 has 10000 sample
2019 clinical data has a shape of (2500,1000)
2019 has 2500 sample
Each image is represented with 1000 datapoints (1 second), representing an intensity point each millisecond
```
data/X_2018clinical.npy
data/y_2018clinical.npy
data/X_2019clinical.npy
data/y_2019clinical.npy
```
![text](/results/binarized-antibiotic-prediction-clinical.png)



##
