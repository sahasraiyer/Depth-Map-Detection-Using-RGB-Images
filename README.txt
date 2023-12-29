The data loader and image processing part is inspired by the PixelFormer paper for nyu-depth-2 dataset.


Steps to run the code:


1. Load the dataset and train_values and test_values txt files. The txt files contain the path to the train and val/test images and their corresponding depth maps. Change the path in the txt files according to your local path of the dataset using find and replace method. 
   1. For eg : /content/drive/MyDrive/PixelTransformer/PixelFormer-main/dataset/nyu_depth_v2/official_splits/test/kitchen/rgb_00001.jpg /content/drive/MyDrive/PixelTransformer/PixelFormer-main/dataset/nyu_depth_v2/official_splits/test/kitchen/sync_depth_00001.png
                THIS WILL CHANGE TO /YOUR_DATASET_PATH/dataset/nyu_depth_v2/official_splits/test/kitchen/rgb_00001.jpg /YOUR_DATASET_PATH/dataset/nyu_depth_v2/official_splits/test/kitchen/sync_depth_00001.png
2. There are three different model notebooks each for one model - ResNet, ResNet+Swin, ResNet+Swin+PSP+SAM. These files can be run directly for training and validation, they have some dependencies whose installations are included in the code. (use pip install timm)
3. To test the models, there are checkpoints given for each model of each notebook, put them in the correct path and, just skip the training part and run the Testing part of the notebook to see results.
