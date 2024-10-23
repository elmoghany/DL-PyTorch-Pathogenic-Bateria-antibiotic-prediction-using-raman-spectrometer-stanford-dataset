# Nature Paper PyTorch Implementation: "Rapid identification of pathogenic bacteria using Raman spectroscopy and deep learning"

## Files
2 Jupyter Notebooks are provided:
1. Input intensity waveforms of the bacteria and predicting the output label of the bacteria "DL-PyTorch-CNN-bacteria-prediction.ipynb"
2. Input intensity waveforms of the bacteria while binarizing (combining) output prediction of bacteria into antibiotic groups "DL-PyTorch-CNN-bacteria-antibiotic-prediction.ipynb"

## Datasets
[Dataset-Link-here](https://www.dropbox.com/scl/fo/fb29ihfnvishuxlnpgvhg/AJToUtts-vjYdwZGeqK4k-Y?rlkey=r4p070nsuei6qj3pjp13nwf6l&dl=0)

### Reference data
Used to train the model from scratch
```
data/X_reference.npy
data/y_reference.npy
```

### Finetune data
Used to finetune the model after training on the reference data
```
data/X_finetune.npy
data/y_finetune.npy
```

### Test data
Used to test the model output and ensure it is working correctly
```
data/X_test.npy
data/y_test.npy
```

### 2018 & 2019 Clinical data
```
data/X_2018clinical.npy
data/y_2018clinical.npy
data/X_2019clinical.npy
data/y_2019clinical.npy
```

##
