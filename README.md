# EDANet
This repository contains the implementation details of our paper: [[arXiv:1809.06323]](https://arxiv.org/abs/1809.06323)

**"Efficient Dense Modules of Asymmetric Convolution for Real-Time Semantic Segmentation"**

by Shao-Yuan Lo, Hsueh-Ming Hang, Sheng-Wei Chan, Jing-Jhih Lin

![EDANet](https://github.com/shaoyuanlo/EDANet/blob/master/models/EDANet_figure.PNG)

NOTE: The source codes must be kept confidential due to the sponsor's request for this project. We try our best to provide the implementation details as much as possible. We hope it would be easy for you to reproduce and utilize this work.

## Pakages
This repository is organized as:

*   [models](https://github.com/shaoyuanlo/EDANet/tree/master/models) contains the layer disposal of EDANet and each network variant introduced in our paper.
*   [train](https://github.com/shaoyuanlo/EDANet/tree/master/train) contains the training details and the class weights used to train our networks.

We replace our source codes with lists to show the detailed network architectures and training setup. In our actual implementation, **PyTorch (v0.4.1)** is used to perform all the experiments.

## Performance on the Cityscapes dataset
EDANet achieves a mIoU of **67.32** on the [Cityscapes](https://www.cityscapes-dataset.com/) test set without any pretrained model. ([Cityscapes leaderboard](https://www.cityscapes-dataset.com/benchmarks/#scene-labeling-task))

For an input resolution of 512x1024, EDANet can run at the speed of **108 FPS** on a single GTX 1080Ti GPU and **81 FPS** on a single Titan X GPU.

![sample_results](https://github.com/shaoyuanlo/EDANet/blob/master/train/sample_results.PNG)


In our paper, it also shows the evaluation results on the [CamVid](http://mi.eng.cam.ac.uk/research/projects/VideoRec/CamVid/) dataset.

## Citation
If EDANet is useful for your research, please consider citing our paper:

*   S.-Y. Lo, H.-M. Hang, S.-W. Chan, and J.-J. Lin, “Efficient dense modules of asymmetric convolution for real-time semantic segmentation,” arXiv preprint arXiv: 1809.06323, 2018.
