# DATN-Submitted-to-IEEE-GRSL
Dropout-based Adversarial Training Networks for Remote Sensing Scene Classification (This paper has been submitted to IEEE-GRSL in 2021.)

## Usage

1. Data preparation: `split.py`

```
dataset|——train
	   |——Airport
	   |——BareLand
	   |——....
	   |——Viaduct
       |——val
	   |——Airport
	   |——BareLand
	   |——....
	   |——Viaduct
```



2. run `train.py` to train the model
3. `confusionmatrix.py` for drawing

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
3. pytorch 1.4
