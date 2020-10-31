# DETR based on Detectron2

## Instructions
1. Follow detectron2's readme to install detection2
  * ```cd DETR.detectron2```
  * ```python setup.py build develop```
  * link dataset path to DETR.detectron2/datasets/
2. Run DETR
  * ```python projects/DETR/train_net.py --num-gpus 8 --config-file projects/DETR/configs/detr.res50.coco.multiscale.150e.yaml```

## Results

| config                               | COCO AP         | Paper        |
| ------------------------------------ | --------------- | ------------ |
| detr.res50.coco.multiscale.150e.yaml | 38.8 without RC | 39.5 with RC |

"**RC**" means RandomCrop, it brings about 1% AP improvements accroding to paper.


## Disclaimer
* I haven't add RandomCrop.
* I haven't add support for segmentaion, but it can be easily added. 

## Advantage
* Training faster
* Avoid memory leaking in official implementation
* Use backbone in detectron2
