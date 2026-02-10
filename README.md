This EU land cover spatial modeling project is ongoing. 
Goal: Use train/test split and validation to create spatial models which will allow accurate prediction of land type. 

The EuroSAT RGB dataset is made up of labeled satellite image patches showing different land use and land cover classes in Europe. Each image is a 64×64 RGB satellite tile, categorized into one of ten classes such as forest, residential areas, rivers, and agricultural land. 

The data was found at https://huggingface.co/datasets/blanchon/EuroSAT_RGB

The dataset has 27,000 labeled images split into training (16,200 rows), validation (5,400 rows), and test (5,400 rows) sets. Each image record includes three columns consisting of an RGB image, a categorical class label with ten possible values, and a filename identifier.

The outcome column is the "label" variable, which represents the land use or cover category of each satellite image. Future work trained on this dataset will predict the label based on the image column.

I found that the EuroSAT RGB dataset is clean and well-structured, with no missing labels or filenames detected, which I'm grateful to find from this huggingface dataset. The images are all uniform at 64×64 pixels with three RGB channels with distinct distributions. Class distribution across the ten land use categories is relatively balanced. Pixel intensity values span 0–255 for all color channels, so there will be no clipping or normalization issues. A limitation of the dataset is its relatively small image size, but this also makes the data efficient for the project.

