# MIIC Dataset for Image Anomaly Detection
Microscopic Images of Integrated Circuits (MIIC)
=============

The Microscopic Images of Integrated Circuits (MIIC) accompanies the following publication: 
"Joint Anomaly Detection and Inpainting for Microscopy Images via Deep Self-Supervised Learning," IEEE International Conference on Image Processing (ICIP), 2021

Dataset description:

MIIC is a novel dataset of real microscopic images of integrated circuits (ICs), to benchmark the IAD algorithms. The MIIC dataset includes 25,160 normal and 116 anomalous high-resolution IC images obtained by ScanningElectron Microscopy (SEM). The SEM images are taken at the metal layer of a manufactured IC and are in gray-scale with a dimension of 512x512 pixels. For each image containing anomalies, we provide differ-ent types of annotations, including the bounding box and pixel-wise ground truth mask for them, which enables future research toward various computer vision applications.

Dataset Link: [Download MIIC](https://researchdata.ntu.edu.sg/dataset.xhtml?persistentId=doi:10.21979/N9/WBLTFI).

Use
---
All data is subject to copyright and may only be used for non-commercial research. 

Contact Bihan Wen (bihan.wen@ntu.edu.sg) for any questions.

In case of use, please cite our publication:
L. Huang, D. Cheng, X. Yang, T. Lin, Y. Shi, K. Yang, B.-H. Gwee, and B. Wen, "Joint Anomaly Detection and Inpainting for Microscopy Images via Deep Self-Supervised Learning," in Proc. IEEE Int. Conf. Image Processing (ICIP), 2021.

Bibtex:
@inproceedings{huang2021,
  author={Huang, Ling and Cheng, Deruo and Xulei, Yang and Tong, Lin and Yiqiong, Shi and Kaiyi Yang and Bah-Hwee, Gwee and Bihan, Wen},
  title={Joint Anomaly Detection and Inpainting for Microscopy Images via Deep Self-Supervised Learning},
  year={2021},
  booktitle={IEEE International Conference on Image processing (ICIP)}
}




%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
--------------------------------------------------------------
Data:

Anomaly_train: 
	a mixture of 25,160 normal and 116 abnormal images									- 	Anomaly_train/*.jpg		

Anomaly_test (this is a subset of Anomaly_train):
	1,272 normal images (a random subset of 25,160 normal images in Anomaly_train)		- 	Anomaly_test/normal_img/*.jpg
	116 abnormal images (same as the 116 abnormal images in Anomaly_train)				- 	Anomaly_test/abnormal_img/*.jpg
	bounding box for the anomalies in the 116 abnormal images							- 	Anomaly_test/abnormal_bbox/*_bbox.jpg
	pixel-wise mask for the anomalies in the 116 abnormal images						-	Anomaly_test/abnormal_mask/*_mask.jpg
	location (col, row, width, height) for the anomalies in the 116 abnormal images		-	Anomaly_test/anomalyPosition.mat

Inpainting_train:
	1,312 pairs of synthesized abnormal images and corresponding normal images			-	Inpainting_train/*.jpg

Inpainting_test:
	135 pairs of synthesized abnormal images and corresponding normal images			-	Inpainting_test/*.jpg

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%