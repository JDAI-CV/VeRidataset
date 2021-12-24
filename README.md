# 1. VeRi dataset 
(Please click [**here**](http://vehiclereid.github.io/VeRi/) to the new webpage.)

To facilitate the research of vehicle re-identification (Re-Id), we build a large-scale benchmark dateset for vehicle Re-Id in the real-world urban surveillance scenario, named "VeRi". The featured properties of VeRi include:
* It contains over 50,000 images of 776 vehicles captured by 20 cameras covering an 1.0 km^2 area in 24 hours, which makes the dataset scalable enough for vehicle Re-Id and other related research. 
* The images are captured in a real-world unconstrained surveillance scene and labeled with varied attributes, e.g. BBoxes, types, colors, and brands. So complicated models can be learnt and evaluated for vehicle Re-Id.
* Each vehicle is captured by 2 ∼ 18 cameras in different viewpoints, illuminations, resolutions, and occlusions, which provides high recurrence rate for vehicle Re-Id in practical surveillance environment.
* It is also labeled with sufficient license plates and spatiotemporal information, such as the BBoxes of plates, plate strings, the timestamps of vehicles, and the distances between neighbouring cameras.

&ensp;&ensp;&ensp;&ensp;![Image](./images/VeRi_240.png)&ensp;&ensp;![Image](./images/VeRi2_240.png)

**Recently, we release a large-scale Multi-grained Vehiclde Parsing dataset in the wild. Please refer to [MVP](https://lxc86739795.github.io/MVP.html) to download it!**

# 2. Download
To encourage related research, we will provide the dataset according to your request. 
Please email your full name and affiliation to the contact person (*xinchenliu at bupt dot cn*). 
We ask for your information only to make sure the dataset is used for non-commercial purposes. 
We will not give it to any third party or publish it publicly anywhere.

# 3. Citation
If you use the dataset, please kindly cite the following paper:
* 	Xinchen Liu, Wu Liu, Huadong Ma, Huiyuan Fu: Large-scale vehicle re-identification in urban surveillance videos. ICME 2016: 1-6 (**Best Student Paper Award**, Citation=178)
* Xinchen Liu, Wu Liu, Tao Mei, Huadong Ma: A Deep Learning-Based Approach to Progressive Vehicle Re-identification for Urban Surveillance. ECCV (2) 2016: 869-884 (Citation=126)
* Xinchen Liu, Wu Liu, Tao Mei, Huadong Ma: PROVID: Progressive and Multimodal Vehicle Reidentification for Large-Scale Urban Surveillance. IEEE Trans. Multimedia 20(3): 645-658 (2018) (Citation=102)

# 4. Code and Models
Now, the FastReID toolbox has supported the VeRi dataset with powerful models.
Please refer to [FsatReID](https://github.com/JDAI-CV/fast-reid).



# 5. State-of-the-art Results on the VeRi Dataset

|Reference|Year|           mAP|        Rank-1|        Rank-5|
|:-------:|:--:|-------------:|-------------:|-------------:|
|[1]|2016|19.92|59.65|75.27|
|[2]|2016|27.77|61.44|78.78|
|[3]|2017|58.27|83.49|90.04|
|[4]|2017|57.4|86.59|92.85|
|[5]|2017|58.78|86.41|92.91|
|[6]|2017|51.42|68.30|89.70|
|[7]|2017|60.47|85.52|95.11|
|[8]|2018|53.42|81.56|95.11|
|[9]|2018|59.47|96.24|98.97|
|[10]|2018|61.5|88.6|94|
|[11]|2018|53.53|82.9|91.6|
|[12]|2018|61.32|85.92|91.84|
|[13]|2018|53.45|83.49|92.55|
|[14]|2018|61.11|89.27|94.76|
|[15]|2018|53.35|82.06|92.31|
|[16]|2018|49.3|88.56|-|
|[17]|2018|64.78|88.62|94.52|
|[18]|2018|25.12|60.83|78.55|
|[19]|2018|60.49|77.33|88.27|
|[20]|2019|62.62|90.58|97.14|
|[21]|2019|57.44|84.39|94.05|
|[22]|2019|67.55|90.23|96.42|
|[23]|2019|61.83|88.5|94.46|
|[24]|2019|67.6|90.2|-|
|[25]|2019|55.49|84.27|92.43|
|[26]|2019|74.3|94.3|98.7|
|[27]|2019|72.5|93.3|97.1|
|[28]|2019|71.88|92.86|96.97|
|[29]|2019|66.34|89.78|95.99|
|[30]|2019|66.35|90.17|94.34|
|[31]|2019|61.7|89.4|95.0|
|[32]|2020|75.9|95.8|-|
|[33]|2020|79.5|95.6|98.4|
|[34]|2020|68.9|94.0|97.6|
|[35]|2020|79.6|96.4|98.6|
|[36]|2020|78.6|95.4|98.4|
|[37]\*|2020|83.41|96.78|-|
|[Ours](https://github.com/JDAI-CV/fast-reid)|2020|81.9|97.9|99.0|
|[38]|2021|79.5|96.0|98.5|
|[39]\**|2021|82.0|97.1|-|
|[40]|2021|81.0|96.7|98.6|

\* This method [37] uses large additional data from other datasets.

\** This method [39] uses 384x128 input, camera labels, and viewpoint labels.


# 6. Our Results on Six Datasets
![Image](./images/mAP_on6.jpg)
![Image](./images/Rank1_on6.jpg)


## Reference
[1] Liu, Xinchen, et al. "Large-scale vehicle re-identification in urban surveillance videos." ICME 2016.

[2] Liu, Xinchen, et al. "A deep learning-based approach to progressive vehicle re-identification for urban surveillance." ECCV 2016.

[3] Liu, Wu, et al. "Beyond human-level license plate super-resolution with progressive vehicle search and domain priori GAN." ACMMM 2017.

[4] Shen, Yantao, et al. "Learning deep neural networks for vehicle re-id with visual-spatio-temporal path proposals." ICCV 2017.

[5] Zhang, Yiheng, Dong Liu, and Zheng-Jun Zha. "Improving triplet-wise training of convolutional neural network for vehicle re-identification." ICME 2017.

[6] Wang, Zhongdao, et al. "Orientation invariant feature embedding and spatial temporal regularization for vehicle re-identification." ICCV 2017.

[7] Tang, Yi, et al. "Multi-modal metric learning for vehicle re-identification in traffic surveillance environment." ICIP 2017.

[8] Liu, Xinchen, et al. "PROVID: Progressive and multimodal vehicle reidentification for large-scale urban surveillance." IEEE TMM 20.3 (2018): 645-658.

[9] Bai, Yan, et al. "Group-Sensitive Triplet Embedding for Vehicle Reidentification." IEEE TMM 20.9 (2018): 2385-2399.

[10] Liu, Xiaobin, et al. "Ram: a region-aware deep model for vehicle re-identification." ICME 2018.

[11] Zhu, Jianqing, et al. "Joint feature and similarity deep learning for vehicle re-identification." IEEE Access 6 (2018): 43724-43731.

[12] Zhou, Yi, and Ling Shao. "Aware attentive multi-view inference for vehicle re-identification." CVPR 2018.

[13] Zhu, Jianqing, et al. "A shortly and densely connected convolutional neural network for vehicle re-identification." ICPR 2018.

[14] Jiang, Na, et al. "Multi-Attribute Driven Vehicle Re-Identification with Spatial-Temporal Re-Ranking." ICIP 2018.

[15] Wu, Chih-Wei, et al. "Vehicle re-identification with the space-time prior." CVPRW 2018.

[16] Kanaci, Aytac, Xiatian Zhu, and Shaogang Gong. "Vehicle Re-Identification in Context." arXiv preprint arXiv:1809.09409(2018).

[17] Wu, Fangyu, et al. "Joint Semi-supervised Learning and Re-ranking for Vehicle Re-identification." ICPR 2018.

[18] Zhou, Yi, Li Liu, and Ling Shao. "Vehicle re-identification by deep hidden multi-view inference." IEEE TIP 27.7 (2018): 3275-3287.

[19] Zhou, Yi, and Ling Shao. "Vehicle Re-Identification by Adversarial Bi-Directional LSTM Network." WACV 2018.

[20] Liu, Xinchen, et al. "PVSS: A Progressive Vehicle Search System for Video Surveillance Networks." arXiv preprint arXiv:1901.03062 (2019).

[21] Lou, Yihang, et al. "Embedding Adversarial Learning for Vehicle Re-Identification." IEEE TIP (2019).

[22] Kumar, Ratnesh, et al. "Vehicle Re-Identification: an Efficient Baseline Using Triplet Embedding." arXiv preprint arXiv:1901.01015 (2019).

[23] Zhu, Jianqing, et al. "Vehicle Re-Identification Using Quadruple Directional Deep Learning Features." IEEE TITS (2019).

[24] Tang, Zheng, et al. "CityFlow: A City-Scale Benchmark for Multi-Target Multi-Camera Vehicle Tracking and Re-Identification." CVPR (2019).

[25] Lou, Yihang, et al. "VERI-Wild: A Large Dataset and a New Method for Vehicle Re-Identification in the Wild." IEEE CVPR (2019).

[26] He, Bing, et al. "Part-regularized Near-duplicate Vehicle Re-identification." IEEE CVPR (2019).

[27] Qian, Jingjing, et al. "Stripe-based and Attribute-aware Network: A Two-Branch Deep Model for Vehicle Re-identification." arXiv (2019).

[28] Tang, Zheng, et al. "PAMTRI: Pose-Aware Multi-Task Learning for Vehicle Re-Identification Using Highly Randomized Synthetic Data." IEEE ICCV (2019).

[29] Chu, Ruihang, et al. "Vehicle Re-identification with Viewpoint-aware Metric Learning." IEEE ICCV (2019).

[30] Pirazh Khorramshahi et al. "A Dual-Path Model With Adaptive Attention For Vehicle Re-Identification." IEEE ICCV (2019).

[31] Xiaobin Liu, Shiliang Zhang, Xiaoyu Wang, Richang Hong, Qi Tian: Group-Group Loss-Based Global-Regional Feature Learning for Vehicle Re-Identification. IEEE TIP (2020).

[32] Xin Jin, Cuiling Lan, Wenjun Zeng, Zhibo Chen: Uncertainty-Aware Multi-Shot Knowledge Distillation for Image-Based Object Re-Identification. AAAI 2020: 11165-11172

[33] Dechao Meng, et al. Parsing-based View-aware Embedding Network for Vehicle Re-Identification. IEEE CVPR (2020).

[34] Tsai-Shien Chen, et al. Orientation-aware Vehicle Re-identification with Semantics-guided Part Attention Network. ECCV (2020).

[35] Pirazh Khorramshahi, et al. The Devil is in the Details: Self-Supervised Attention for Vehicle Re-Identification. ECCV (2020).

[36] Xinchen Liu, et al. Beyond the Parts: Learning Multi-view Cross-part Correlation for Vehicle Re-identification. ACM MM (2020).

[37] Zhedong Zheng, et al. VehicleNet: Learning Robust Visual Representation for Vehicle Re-identification. IEEE Trans. Multimedia (2020).

[38] Wei Sun, et al. TBE-Net: A Three-Branch Embedding Network With Part-Aware Ability and Feature Complementary Learning for Vehicle Re-Identification
. IEEE Transactions on Intelligent Transportation Systems (2021).

[39] Shuting He, et al. TransReID: Transformer-based Object Re-Identification. ICCV (2021).

[40] Ming Li, et al. Self-supervised Geometric Features Discovery via Interpretable Attention for Vehicle Re-Identification and Beyond. ICCV (2021).

_Last modified in **Dec, 2021**_
