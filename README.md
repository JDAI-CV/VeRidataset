Welcome to the veridataset wiki!
# 1. VeRi dataset
To facilitate the research of vehicle re-identification (Re-Id), we build a large-scale benchmark dateset for vehicle Re-Id in the real-world urban surveillance scenario, named "VeRi". The featured properties of VeRi include:
* It contains over 50,000 images of 776 vehicles captured by 20 cameras covering an 1.0 km^2 area in 24 hours, which makes the dataset scalable enough for vehicle Re-Id and other related research. 
* The images are captured in a real-world unconstrained surveillance scene and labeled with varied attributes, e.g. BBoxes, types, colors, and brands. So complicated models can be learnt and evaluated for vehicle Re-Id.
* Each vehicle is captured by 2 ∼ 18 cameras in different viewpoints, illuminations, resolutions, and occlusions, which provides high recurrence rate for vehicle Re-Id in practical surveillance environment.
* It is also labeled with sufficient license plates and spatiotemporal information, such as the BBoxes of plates, plate strings, the timestamps of vehicles, and the distances between neighbouring cameras.

# 2. Download
In order to guarantee the quality, the dataset is under revision. To encourage related research, we will provide the dataset according to your request. Please email your full name and affiliation to the contact person (xinchenliu at bupt dot edu dot cn). We ask for your information only to make sure the dataset is used for non-commercial purposes. We will not give it to any third party or publish it publicly anywhere.

# 3. Citation
If you use the dataset, please kindly cite the following paper:
* 1. Liu X., Liu W., Ma H., Fu H.: Large-scale vehicle re-identification in urban surveillance videos. In: IEEE International Conference on Multimedia and Expo. (2016) accepted.
* 2. Liu X., Liu W., Mei T., Ma H. A Deep Learning-Based Approach to Progressive Vehicle Re-identification for Urban Surveillance. In: European Conference on Computer Vision. Springer International Publishing, 2016: 869-884.

# 4. Example codes
Here we give an example code for vehicle search evaluation.

In this code, we should first the distance matrix of all query images and test images.
As in the example code, we have three distance matrixes obtained with SIFT-BOW, CN-BOW, CNN features seperately.

Then these matrixes are summed with different weights to obtain the final "dist" matrix.
Then we read the ground truth and junk image index (the test images that have the same camera ID with the query image, they are not considered when computing the AP) from the gt_image.txt and jk_image.txt.

After that, for each query, we rank the distance to each test image and compute the Average Presicion using the compute_AP function.
At last, we can obtain the mAP, HIT@1, HIT@5, and the CMC curves.
