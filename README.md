# Dermoscopic Image handling for Training Deep Learning Models
From ISIC 2019 dataset of approximately 25000 dermoscopic skin lesion pictures, I opted to train a neural network by extracting a suitable sample out of this dataset.
Step 1: The dataset harbors a CSV file with each image's name and its provided classification label. I assigned images with the same label into a separate folder named the same as the class label.
Step 2: From each class (or created folder), I randomly selected 125 images without (or with the minimum) black margine. Out of 125, 25 was randomly allocated to a test subfolder, leaving the remainder as train images.
Step 3: As images varied in their original dimensions, I resized them all to 512*512 pixels.
