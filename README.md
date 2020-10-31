# DETR based on Detectron2

## Instructions
1. Follow detectron2's readme to install detection2
  * ```cd DETR.detectron2```
  * ```python setup.py build develop```
  * link dataset path to DETR.detectron2/datasets/
2. Train DETR
  * ```python projects/DETR/train_net.py --num-gpus 8 --config-file projects/DETR/configs/detr.res50.coco.multiscale.150e.yaml```: use MSRA pretrain weights
3. Evaluate DETR using provided weights [here](https://drive.google.com/drive/folders/1QxTslMLapXcgsIu36jFJyceY04J9Hk-e?usp=sharing)
  * ```python projects/DETR/train_net.py --num-gpus 8 --config-file projects/DETR/configs/detr.res50.coco.multiscale.150e.yaml --eval-only MODEL.WEIGHTS path/to/provided/ckpt.pth```
4. For faster training:
  * ```python projects/DETR/train_net.py --num-gpus 8 --config-file projects/DETR/configs/detr.res50.coco.multiscale.150e.bs48.yaml```
  Using a 8x2080ti server, 150 epochs take about 3 day 6 hours.

## Results

| config                               | COCO AP         | Paper        | Checkpoint |
| ------------------------------------ | --------------- | ------------ | ---------- |
| detr.res50.coco.multiscale.150e.yaml | 38.6 without RC | 39.5 with RC | [LINK](https://drive.google.com/drive/folders/1QxTslMLapXcgsIu36jFJyceY04J9Hk-e?usp=sharing)

"**RC**" means RandomCrop, it brings about 1% AP improvements accroding to paper.


## Disclaimer
* I haven't add RandomCrop.
* I haven't add support for segmentaion, but it can be easily added. 

## Advantage
* Training faster
* Avoid memory leaking in official implementation
* Use backbone in detectron2
