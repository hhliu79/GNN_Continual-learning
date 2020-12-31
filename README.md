# PyTorch implementation of TWP
Overcoming Catastrophic Forgetting in Graph Neural Networks, AAAI2021

# 
![image](https://github.com/hhliu79/TWP/blob/master/overview.png)

# Cite
@inproceedings{liu2021overcoming,<br>
 > title={Overcoming Catastrophic Forgetting in Graph Neural Networks},<br>
 > author={Huihui Liu, Yiding Yang, and Xinchao Wang},<br>  > year={2021},<br>
 > booktitle={AAAI Conference on Artificial Intelligence},<br>
}

**cite** contains a Tensorflow implementation for our [paper](https://arxiv.org/abs/1711.08389).  If you find this code useful in your research, please consider citing:

    @inproceedings{plummerCITE2018,
	Author = {Bryan A. Plummer and Paige Kordas and M. Hadi Kiapour and Shuai Zheng and Robinson Piramuthu and Svetlana Lazebnik},
	Title = {Conditional Image-Text Embedding Networks},
	Booktitle  = {The European Conference on Computer Vision (ECCV)},
	Year = {2018}
    }

# Dependencies
See the file [requirements.txt](https://github.com/hhliu79/TWP/blob/master/requirements.txt) for more information about how to install the dependencies.

# Datasets
## Node classification
We conduct experiments on four public datasets (Corafull, Amazon Computer, PPI, Reddit) based on [DGL](https://docs.dgl.ai/en/0.4.x/).<br>

## Graph classification
We conduct experiments on one public dataset (Tox21) based on [DGLlife](https://lifesci.dgl.ai/index.html).

# Models
We use [DGL](https://docs.dgl.ai/en/0.4.x/) to implement all the GNN models.

# Overview
Here we provide the implementation of our method based on the Corafull dataset. The folder `< corafull_amazon/ >` is organised as follows:
* `< LifeModel/ >` contains the implementation of all the continual learning method for GNNs, including the baseline methods and our method;
* `< dataset/ >`  contains code to load the dataset; 
* `< models/ >` contains the implementation of the GNN backbone;
* `< training/ >` contains code to set seed;
* The file `< train.py >` is used to execute the whole training process on the Corafull dataset;
* The file `< run.sh >` contains an example to run the code.
