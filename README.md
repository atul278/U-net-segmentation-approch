# U-net-segmentation-approch

This is an image segmentation and classification system which will be able to predict mask
image of lung nodule in give image and classify it to benign or malignant. I am using dataset
from LUNA 16 challenge which has made available CT images with annotated nodule locations.
It contains data from 888 patients. It contains total of 1186 malign lung nodule. We first preprocess
images to isolate areas of lung from images to create lung mask. These lung mask is then applied
to original image to form final image for training. We used U-Net segmentation approach for the
localization of position of lung nodule. These model is then trained using final training image after
preprocessing. Our second aim to classify the known lung nodule to benign or malignant. We used
convolutional neural network for classification of nodule. We used dice coefficient as a parameter
to evaluate performance of mask prediction and confusion matrix for evaluation of classification.
