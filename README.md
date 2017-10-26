# DL-neuro_Papers
Collection of resources dealing with convergence of DL and neuro

## Papers:-
+ [Activations of Deep CNN and visual pathway regions](https://www.biorxiv.org/content/biorxiv/early/2017/08/29/133694.full.pdf) - how brain regions responsible for visual pathway and the alenet layers capture "similar" features. They compared confusion matrix-type matrices between inputs from diff brain regions and alexnet layers. Uses Representation dissimalirity matrices(RDM) for each layer or probe characteristic ifentification and subsequent Representation similarity analysis(RSA) for quantification of mapping similarity between each probe and each layer of AlexNet.
+ [Convolutional neural network-based encoding and decoding of visual object recognition in space and time](http://www.sciencedirect.com/science/article/pii/S1053811917305864?via%3Dihub) - stimulus representations from CNNs can predict MEG source activity across visual system, both in space & time. Used encoding approach instead of RSA. Most regions are predicted well by low-level layers, whereas later in time, most regions are predicted well by high-level layers. Decoding results for some subjects are "above-chance".

+ [A novel deep learning approach for classification of EEG motor imagery signals](http://iopscience.iop.org/article/10.1088/1741-2560/14/1/016003/meta;jsessionid=47DB0AD1A3CDEDCA4054F70D1C3010AD.c2.iopscience.cld.iop.org) - Used a CNN for BCI competition dataset III and IV and got good accuracy. Greedily trained CNN layer-by-layer to achieve better accuracy.
