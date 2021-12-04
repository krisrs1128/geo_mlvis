# geo_mlvis
This is the code repository for "Glacier Segmentation" project.

Raw data coule be downloaded as .tiff files using "Data_Preview_Download/download.ipynb"

Data is processed using "Preprocess/preprocess.Rmd" where we also include bash code for cluster computing.

Data is modeled with a U-net model in "Train_Pred/train_gpu.py" and predicted with "Train_Pred/save_preds.py".

