# detr.res50.c5.coco.multiscale.150e.bs16  

## Evaluation results for bbox:  

```  
 Average Precision  (AP) @[ IoU=0.50:0.95 | area=   all | maxDets=100 ] = 0.388
 Average Precision  (AP) @[ IoU=0.50      | area=   all | maxDets=100 ] = 0.592
 Average Precision  (AP) @[ IoU=0.75      | area=   all | maxDets=100 ] = 0.404
 Average Precision  (AP) @[ IoU=0.50:0.95 | area= small | maxDets=100 ] = 0.176
 Average Precision  (AP) @[ IoU=0.50:0.95 | area=medium | maxDets=100 ] = 0.424
 Average Precision  (AP) @[ IoU=0.50:0.95 | area= large | maxDets=100 ] = 0.569
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=   all | maxDets=  1 ] = 0.317
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=   all | maxDets= 10 ] = 0.507
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=   all | maxDets=100 ] = 0.551
 Average Recall     (AR) @[ IoU=0.50:0.95 | area= small | maxDets=100 ] = 0.273
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=medium | maxDets=100 ] = 0.611
 Average Recall     (AR) @[ IoU=0.50:0.95 | area= large | maxDets=100 ] = 0.783
```  
|   AP   |  AP50  |  AP75  |  APs   |  APm   |  APl   |  
|:------:|:------:|:------:|:------:|:------:|:------:|  
| 38.777 | 59.247 | 40.418 | 17.633 | 42.435 | 56.857 |

### Per-category bbox AP:  

| category      | AP     | category     | AP     | category       | AP     |  
|:--------------|:-------|:-------------|:-------|:---------------|:-------|  
| person        | 50.080 | bicycle      | 28.648 | car            | 35.517 |  
| motorcycle    | 42.360 | airplane     | 66.972 | bus            | 63.586 |  
| train         | 65.379 | truck        | 34.368 | boat           | 20.353 |  
| traffic light | 18.903 | fire hydrant | 65.399 | stop sign      | 57.985 |  
| parking meter | 42.823 | bench        | 23.603 | bird           | 31.029 |  
| cat           | 71.092 | dog          | 66.310 | horse          | 56.220 |  
| sheep         | 49.848 | cow          | 54.030 | elephant       | 64.146 |  
| bear          | 77.556 | zebra        | 66.765 | giraffe        | 69.397 |  
| backpack      | 11.565 | umbrella     | 35.710 | handbag        | 11.917 |  
| tie           | 28.961 | suitcase     | 33.638 | frisbee        | 55.884 |  
| skis          | 19.832 | snowboard    | 32.312 | sports ball    | 34.562 |  
| kite          | 34.698 | baseball bat | 31.088 | baseball glove | 30.337 |  
| skateboard    | 47.306 | surfboard    | 35.508 | tennis racket  | 46.385 |  
| bottle        | 28.293 | wine glass   | 28.083 | cup            | 35.060 |  
| fork          | 29.195 | knife        | 14.709 | spoon          | 14.847 |  
| bowl          | 36.779 | banana       | 22.801 | apple          | 16.817 |  
| sandwich      | 33.751 | orange       | 28.691 | broccoli       | 22.862 |  
| carrot        | 17.752 | hot dog      | 33.599 | pizza          | 49.125 |  
| donut         | 41.362 | cake         | 33.109 | chair          | 24.069 |  
| couch         | 48.725 | potted plant | 25.442 | bed            | 46.263 |  
| dining table  | 29.257 | toilet       | 63.753 | tv             | 54.101 |  
| laptop        | 59.655 | mouse        | 50.442 | remote         | 20.055 |  
| keyboard      | 49.267 | cell phone   | 28.183 | microwave      | 54.855 |  
| oven          | 37.273 | toaster      | 25.362 | sink           | 32.600 |  
| refrigerator  | 58.604 | book         | 9.787  | clock          | 43.984 |  
| vase          | 32.962 | scissors     | 33.718 | teddy bear     | 47.690 |  
| hair drier    | 8.586  | toothbrush   | 18.602 |                |        |
