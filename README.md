# geo_mlvis
**This is the code repository for "Interactive visualization and representation analysis applied to Glacier Segmentation" project.**


## Motivation
In glacier segmentation, researchers focus on implementing model to automatically identify the glaciers from remote sensing data. However, the interpretation of the process is not enough. In this project, we aim to provide a comprehensive visual interpretation of glacier segmentation via interactive visualization and representation analysis. We develop a [shiny app](https://bruce-zheng.shinyapps.io/glacier_segmententation/) for error analysis where users could easily detect potential issues of the predictions. We show a screenshot of our shiny app below.

![25811638647397_ pic_hd](https://user-images.githubusercontent.com/53232883/144722760-d1a153f8-609c-46f5-b1a5-6dd5b095d43a.jpg)

We also provide a visual interpretation of the modeling via representation analysis.

![acts-1-1](https://user-images.githubusercontent.com/53232883/144722811-04a40069-fc36-4ae5-81a3-ef39ca130784.png)




## Code Guidance

Raw data coule be downloaded as .tiff files using "Data_Preview_Download/download.ipynb"

Data is processed using "Preprocess/preprocess.Rmd" where we also include bash code for cluster computing.

Data is modeled with a U-net model in "Train_Pred/train_gpu.py" and predicted with "Train_Pred/save_preds.py".

