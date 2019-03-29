# 1. VeRi dataset
To facilitate the research of vehicle re-identification (Re-Id), we build a large-scale benchmark dateset for vehicle Re-Id in the real-world urban surveillance scenario, named "VeRi". The featured properties of VeRi include:
* It contains over 50,000 images of 776 vehicles captured by 20 cameras covering an 1.0 km^2 area in 24 hours, which makes the dataset scalable enough for vehicle Re-Id and other related research. 
* The images are captured in a real-world unconstrained surveillance scene and labeled with varied attributes, e.g. BBoxes, types, colors, and brands. So complicated models can be learnt and evaluated for vehicle Re-Id.
* Each vehicle is captured by 2 ∼ 18 cameras in different viewpoints, illuminations, resolutions, and occlusions, which provides high recurrence rate for vehicle Re-Id in practical surveillance environment.
* It is also labeled with sufficient license plates and spatiotemporal information, such as the BBoxes of plates, plate strings, the timestamps of vehicles, and the distances between neighbouring cameras.

&ensp;&ensp;&ensp;&ensp;![Image](./images/VeRi_240.png)&ensp;&ensp;&ensp;&ensp;![Image](./images/VeRi2_240.png)

# 2. Download
In order to guarantee the quality, the dataset is under revision. To encourage related research, we will provide the dataset according to your request. Please email your full name and affiliation to the contact person (*xinchenliu at bupt dot edu dot cn*). We ask for your information only to make sure the dataset is used for non-commercial purposes. We will not give it to any third party or publish it publicly anywhere.

Former version of the VeRi dataset has some errors in the train_label.xml file:
Vehicle 3, 7, and 41 in the training set are labeled as typeID="0" which does not correspond to a legal type in list_type.txt.

Vehicle 0003 is an Audi Q3, and typeID="2" (SUV).

Vehicle 0007 is a Nissan SUV, and typeID="2" (SUV).

Vehicle 0041 is a Hummer H2, so typeID="2" (SUV).

# 3. Citation
If you use the dataset, please kindly cite the following paper:
* Xinchen Liu, Wu Liu, Tao Mei, Huadong Ma: A Deep Learning-Based Approach to Progressive Vehicle Re-identification for Urban Surveillance. ECCV (2) 2016: 869-884
* Xinchen Liu, Wu Liu, Tao Mei, Huadong Ma: PROVID: Progressive and Multimodal Vehicle Reidentification for Large-Scale Urban Surveillance. IEEE Trans. Multimedia 20(3): 645-658 (2018)

# 4. Example codes
Here we give an example code for vehicle search evaluation.

In this code, we should first get the distance matrix of all query images and test images.
As in the example code, we have three distance matrixes obtained with SIFT-BOW, CN-BOW, CNN features seperately.
Then these matrixes are summed with different weights to obtain the final "dist" matrix.

Then we read the ground truth and junk image index (the test images that have the same camera ID with the query image, they are not considered when computing the AP) from the gt_image.txt and jk_image.txt.

After that, for each query, we rank the distance to each test image and compute the Average Presicion using the compute_AP function.
At last, we can obtain the mAP, HIT@1, HIT@5, and the CMC curves.
