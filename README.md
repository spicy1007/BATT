# BATT

This is the official implementation of our paper [BATT](https://arxiv.org/abs/2211.01806), accepted by ICASSP, 2023. This research project is developed based on Python 3 and Pytorch, created by [Tong Xu](https://github.com/spicy1007) and [Yiming Li](http://liyiming.tech/)



## Reference
If our work or this repo is useful for your research, please cite our paper as follows:
```
@inproceedings{li2022defending,
  title={BATT: Backdoor Attack with Transformation-based Triggers},
  author={Xu, Tong and Li, Yiming and Jiang, Yong and Xia, Shu-Tao},
  booktitle={ICASSP},
  year={2023}
}
```

## Pipeline
![Pipeline](pipeline.png)



## Requirements

To install requirements:

```setup
pip install -r requirements.txt
```
Make sure the directory follows:
```File Tree
BATT
├── model
│   ├── resnet
│   └── vgg
├── data
│   ├── cifar10
│   └── GTSRB
|
```

## Dataset Preparation
Make sure the directory ``data`` follows:
```File Tree
data
├── cifar10  
├── GTSRB
│   ├── train
│   └── test
```
>📋  Data Download Link:  
>[data]( wait to update )


## Attack
To train the BATT-R in the paper, run these commands:

CIFAR-10:
```train
python run_batt_r.py
```

## Infected model
Get attacked model in the dictionary 'result':
```File Tree
result
├── attack
│   ├── batt_r_cifar10.pth
│   └── ...
```
>📋  Sample Infected Model Download Link:  
>[model]( wait to update )
