# DATN-Submitted-to-IEEE-GRSL
Dropout-based Adversarial Training Networks for Remote Sensing Scene Classification (This paper has been submitted to IEEE-GRSL in 2021.)

## Usage

1. Data preparation: `make_list.py` 
2. python `train.py` --gpu_id 0 --net ResNet50 --dset N_A --s_dset_path ../data/N_A/N_A_list.txt --t_dset_path ../data/Dt-UCM/Dt-UCM_list.txt


## Figs

![image-20210601165926181](https://github.com/WangXin81/DATN-Submitted-to-IEEE-GRSL/blob/main/fig1.png)

## Datasets

UC Merced Land Use Dataset: 

http://weegee.vision.ucmerced.edu/datasets/landuse.html

AID Dataset: 

https://captain-whu.github.io/AID/

NWPU RESISC45: 

http://www.escience.cn/people/JunweiHan/NWPU-RESISC45.html

PatternNet:

https://sites.google.com/view/zhouwx/dataset#h.p_Tgef10WTuEFr

VArcGIS:

https://aistudio.baidu.com/aistudio/datasetdetail/47630

VBing:

https://aistudio.baidu.com/aistudio/datasetdetail/47638

VGoogle:

https://aistudio.baidu.com/aistudio/datasetdetail/47619

First, we combine NWPU and AID together to construct a merged data set (called N_A) with 55 categories. There are 19 identical categories between N_A and UCM. We select these classes in N_A as the source domain, while using the 19 identical categories in UCM as the target domain. Thus, we get the first transfer task: N_A→UCM.

Second, there are 22 same categories between N_A and PatternNet. We choose these categories in N_A as the source domain, while adopting the 22 identical classes in PatternNet as the target domain. Hence, we implement the second transfer task: N_A→PatternNet.

Third, as the newly proposed data sets, VA, VB, and VG have 38 identical classes. We use either of these data sets as the source domain or the target domain, and then carry out the other six transfer tasks: VA→VB, VA→VG, VB→VA, VB→VG, VG→VA, and VG→VB.


## Environments

1. Ubuntu 18.04
2. cuda 10.0
3. Pytorch 1.4
4. Python 3.6
