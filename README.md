# BA512

To obtain a fine-grained and integral functional brain atlas, an eigen clustering (EIC) approach was developed for whole-brain parcellation. This approach, with more detailed description in our previous study [1], has demonstrated its superiority in the robustness to noise and the automatic determination of the optimal clustering number. The functional parcellation was performed at the group level using functional connectivity (FC) from 7.0 Tesla fMRI data of 184 HCP subjects. In specific, an initial “coarse” template was defined at first by the FreeSurfer Desikan–Killiany (DK) atlas [2] using automatic subcortical segmentation and surface parcellation based on gyri and sulci. Second, for each ROI in the initial template, the FC matrix was obtained for each subject by calculating the Pearson’s correlation coefficients between the voxels within the ROI and from the whole brain, followed by a Fisher’s z transformation to improve the normality. Then, the FC matrixes were averaged across subjects and served as the inputs of the EIC algorithm to get the clustering labels automatically. Finally, on the basis of resting-state functional connectome, we subdivided the brain into a total of 512 subregions (including 428 cortical, 56 subcortical and 28 cerebellar regions) as our functional brain atlas, i.e., BA512 atlas. It should be noted that this atlas was derived from the “REST1_PA” dataset of HCP, in which the fMRI phase encoding direction was from the posterior side to the anterior side, and similar results could also be reproduced when using another HCP dataset with the opposite encoding direction, indicating the robustness of our parcellation framework. In addition, the BA512 atlas also demonstrated its advantages of intraregional connectivity homogeneity and task-based functional inhomogeneity, compared with other brain atlases widely used in the fMRI study [3, 4]. The nii file of the parcellation (spatial resolution of 3mm) are provided. Feel free to contact me for parcellation file with spatial resolution of 1mm and 2mm. 

This work is published in IEEE Transactions on Pattern Analysis and Machine Intelligence [5].

References:

[1]. Luo, Z., et al., Functional Parcellation of Human Brain Precuneus Using Density-Based Clustering. Cereb Cortex, 2020. 30(1): p. 269-282.

[2]. Desikan, R.S., et al., An automated labeling system for subdividing the human cerebral cortex on MRI scans into gyral based regions of interest. Neuroimage, 2006. 31(3): p. 968-80.

[3]. Glasser, M.F., et al., A multi-modal parcellation of human cerebral cortex. Nature, 2016. 536(7615): p. 171-178.

[4]. Fan, L., et al., The Human Brainnetome Atlas: A New Brain Atlas Based on Connectional Architecture. Cereb Cortex, 2016. 26(8): p. 3508-26.

[5]. Su, J., et al., Few-shot domain-adaptive anomaly detection for cross-site brain images. IEEE Transactions on Pattern Analysis and Machine Intelligence, 2024. 46(3): p. 1819-1835.
