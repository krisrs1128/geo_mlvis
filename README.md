# geo_mlvis
**This is the code repository for "Interactive visualization and representation analysis applied to Glacier Segmentation" project.**


## Motivation
In glacier segmentation, researchers focus on implementing model to automatically identify the glaciers from remote sensing data. However, the interpretation of the process is not enough. In this project, we aim to provide a comprehensive visual interpretation of glacier segmentation via interactive visualization and representation analysis.

## For the 

Raw data coule be downloaded as .tiff files using "Data_Preview_Download/download.ipynb"

Data is processed using "Preprocess/preprocess.Rmd" where we also include bash code for cluster computing.

Data is modeled with a U-net model in "Train_Pred/train_gpu.py" and predicted with "Train_Pred/save_preds.py".

