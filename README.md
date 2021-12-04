# geo_mlvis
**This is the code repository for "Interactive visualization and representation analysis applied to Glacier Segmentation" project.**


## Motivation
In glacier segmentation, researchers focus on implementing model to automatically identify the glaciers from remote sensing data. However, the interpretation of the process is not enough. In this project, we aim to provide a comprehensive visual interpretation of glacier segmentation via interactive visualization and representation analysis. We develop a [shiny app](https://bruce-zheng.shinyapps.io/glacier_segmententation/) for error analysis where users could easily detect potential issues of the predictions. Here we display two examples below, one for the screenshot of the shinyapp and another one for the visual representation of one satellite image.


## Code Guidance

Raw data coule be downloaded as .tiff files using "Data_Preview_Download/download.ipynb"

Data is processed using "Preprocess/preprocess.Rmd" where we also include bash code for cluster computing.

Data is modeled with a U-net model in "Train_Pred/train_gpu.py" and predicted with "Train_Pred/save_preds.py".





| ![25811638647397_ pic_hd](https://user-images.githubusercontent.com/53232883/144722760-d1a153f8-609c-46f5-b1a5-6dd5b095d43a.jpg) | 
|:--:| 
| *Figure 1: Screenshot of shiny app* |


| ![acts-1-1](https://user-images.githubusercontent.com/53232883/144722811-04a40069-fc36-4ae5-81a3-ef39ca130784.png) | 
|:--:| 
| *Activations of one satellite image across five convolutional layers of the U-Net model. Rows represent the first, third, fifth and seventh downsampling convolutional layers, the first and third upsampling convolutional layers, the last pooling layer and the second middle convolutional layer. For each layer, we randomly plot eight activations in grayscale. We observe that the activations capture basic features at the first layer, become more blurred as down sampling goes deeper, and becomes clearer at the middle layer. Comparing activations in the same layer, we find that the activations look alike in the first layer, but different in the middle layer.* |
| *Figure 2: Visual representations of one satellite image* |





