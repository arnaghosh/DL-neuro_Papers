# DL-neuro_Papers
Collection of resources dealing with confluence of DL and neuro

## Papers:-
+ [Activations of Deep CNN and visual pathway regions](https://www.biorxiv.org/content/biorxiv/early/2017/08/29/133694.full.pdf) - how brain regions responsible for visual pathway and the alenet layers capture "similar" features. They compared confusion matrix-type matrices between inputs from diff brain regions and alexnet layers. Uses Representation dissimalirity matrices(RDM) for each layer or probe characteristic ifentification and subsequent Representation similarity analysis(RSA) for quantification of mapping similarity between each probe and each layer of AlexNet.
+ [Convolutional neural network-based encoding and decoding of visual object recognition in space and time](http://www.sciencedirect.com/science/article/pii/S1053811917305864?via%3Dihub) - stimulus representations from CNNs can predict MEG source activity across visual system, both in space & time. Used encoding approach instead of RSA. Most regions are predicted well by low-level layers, whereas later in time, most regions are predicted well by high-level layers. Decoding results for some subjects are "above-chance".

+ [A novel deep learning approach for classification of EEG motor imagery signals](http://iopscience.iop.org/article/10.1088/1741-2560/14/1/016003/meta;jsessionid=47DB0AD1A3CDEDCA4054F70D1C3010AD.c2.iopscience.cld.iop.org) - Used a CNN for BCI competition dataset III and IV and got good accuracy. Greedily trained CNN layer-by-layer to achieve better accuracy.

+ [Deep Learning with CNN for EEG decoding and visualization](https://onlinelibrary.wiley.com/doi/epdf/10.1002/hbm.23730) - Schirrmeister paper. Used several network architecutres. Good visualization techniques using correlation as a metric to understand features and CNN layer output relationships (not completely clear - read once more). CNNs don't outperform FBCSP clearly. Extensive experiments, results and discussions - good to refer for comparison. Discusses flexibility of CNNs vs simplicity of other models. Github repo [Braindecode](https://github.com/robintibor/braindecode)

+ [Learning Representation from EEG with Deep RCNN](https://arxiv.org/pdf/1511.06448.pdf) - ICLR 2016 paper. Projet EEG electrode position from 3D space to 2D space and then form images with red = alpha channel activity, green = beta channel activity, blue = gamma channel activity. RCNN on this data to classify coginitive-load during task. DeconvNet to visualize filters learnt.

+ [Learning Robust Features using Deep Learning for Automatic Seizure Detection](https://arxiv.org/pdf/1608.00220.pdf) - Joelle Pineau paper. Uses the 3D to 2D projection of electrodes and then RCNN to predict seizure. Occluded image analysis to look at regions of image which affect decision of network. 

+ [Joint Optimization of Algorithmic Suites for EEG Analysis](http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6944253) - EMBC 2014 paper. Uses backprop to jointly optimize spatial projection matrix (initialized with regular CSP), temporal projection matrix and a classifier. Results on BCI II and III datasets. 

+ [Deep Feature Learning for EEG recordings](https://arxiv.org/pdf/1511.04306.pdf) - Sebastian Stober paper. Classification of listened music tracks from EEG in OpenMIIR dataset. Used supervised CNN training, then CAEs (Conv AEs) to learn common signal components and compared the reconstruction loss to PCA and ICA components. Used similarity-constraint encoding and cross-trial encoding (Hydra-nets) to learn "neural" components of the signal (noise removal) and then used these features for classification. A brief presentation of the work here - [ppt](http://bib.sebastianstober.de/2015-12-01_BMI.pdf).

+ [Deep Learning Human Mind for Automated Visual Classification](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8099962) - CVPR 2017 paper. Used LSTM cells to learn time-dependent features from EEG. Features extracted from Deep CNN for the images used for regressing the EEG features. Finally the regressed features used for predicitng which image class was the subject seeing. Best classification results for 320-480 ms after stimulus presentation (the last segment of EEG). 

## Datasets:-
http://bnci-horizon-2020.eu/database/data-sets
