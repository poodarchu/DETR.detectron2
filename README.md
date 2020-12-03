# DETR based on cvpods 

**DETR.detectron2 has been deprecated. Please see our new implementation based on [cvpods](https://github.com/poodarchu/cvpods), which is more user-friendly.**

## Instructions
1. Install cvpods from [here](https://github.com/poodarchu/cvpods)
2. `cd detr.res50.c5.coco.multiscale.150e.bs16`
3. `pods_train --num-gpus 8`

## Results

| config                               | COCO AP         | Paper        | Checkpoint |
| ------------------------------------ | --------------- | ------------ | ---------- |
| detr.res50.c5.coco.multiscale.150e.bs16 | 38.8 without RC | 39.5 with RC | [LINK](https://drive.google.com/drive/folders/1QxTslMLapXcgsIu36jFJyceY04J9Hk-e?usp=sharing)

"**RC**" means RandomCrop, it brings about 1% AP improvements accroding to paper.
