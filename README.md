# DATN-Submitted-to-IEEE-GRSL
Dropout-based Adversarial Training Networks for Remote Sensing Scene Classification (This paper has been submitted to IEEE-GRSL in 2021.)

## Usage

1. Data preparation: `make_list.py` 
2. python train.py --gpu_id 0 --net ResNet50 --dset N_A --s_dset_path ../data/N_A/N_A_list.txt --t_dset_path ../data/Dt-UCM/Dt-UCM_list.txt


## Figs

![image-20210601165926181](https://github.com/WangXin81/DATN-Submitted-to-IEEE-GRSL/blob/main/fig1.png)

## Datasets

UC Merced Land Use Dataset: 

http://weegee.vision.ucmerced.edu/datasets/landuse.html

AID Dataset: 

https://captain-whu.github.io/AID/

NWPU RESISC45: 

http://www.escience.cn/people/JunweiHan/NWPU-RESISC45.html

## Environments

1. Ubuntu 18.04
2. cuda 10.0
3. Pytorch 1.4
4. Python 3.6
