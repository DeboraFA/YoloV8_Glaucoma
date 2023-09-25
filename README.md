# YoloV8 Detect Optic Disc in Retina - Custom Dataset

Create a folder with the dataset separated into training, validation and testing. 
Within each one, create a folder called images where the original images will be 
located, and a folder called labels with the coordinates obtained in Prepare_labels.

------ Folder dataset

---- Train

-- Imagens
  - Img1.jpg
  - Img2.jpg
  - ...
-- Labels
  - img1.txt
  - img2.txt
  - ...

---- Valid

-- Train
-- Label

---- Test


# Prepare dataset train
-- Create the coordinates to localize and segment optic disc.

# Create file **data.yaml** in folder train data
```ruby
train: C:/Users/debora.assis/Documents/REFUGE/train/images
val: C:/Users/debora.assis/Documents/REFUGE/valid/images
names: ['disc']  
```
# Train custom dataset
Run the **YOLOv8_Train_REFUGE.ipynb** code in folder **Train_data** to train the model.

# Test model
Run the **YOLOv8_Predict.ipynb** code  in folder **Test_predict** to obtain the results of segmentation and localization of the optic disc.
