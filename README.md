# DeepLearningVision

(unfinished, Work in Progress)

Intro

#### Sources
http://github.com - automatic!
[GitHub](https://github.com/segments-ai/fast-labeling-workflow)


## Labeling by hand
![Image of segments.ai workflow](https://github.com/Ermaconomist/DeepLearningVision/blob/main/img/1_segments.ai.png)

Segments.ai is a service that greatly simplifies labeling. In a first step we uploaded the photos to the website and started to mark the individual leaves with a digital brush. After 20-30 images, we downloaded the labeled images and trained a model based on Facebooks Detectron2 with the help of Segments.ai toolkit. The trained model and the suggested masks were than uploaded again to the website, were the labeling began to become really easy. 

At the beginning, we had to label every leaf by hand were after a few iterations of downloading, training and uploading we just had to correct a few segmentation errors. 

### Masks after training 

![Image of masks after training](https://github.com/Ermaconomist/DeepLearningVision/blob/main/img/2_masks.png)


## Transferlearning with COCO and Mask-RCNN

Surely, MASK RCNN offers a wide range on possible settings. Hyperparameters like the “max regions of interest per image” needed to be fine-tuned to get the most accurate result possible and to further improve the trained model. 

![Image of Mask-RCNN Workflow used](https://github.com/Ermaconomist/DeepLearningVision/blob/main/img/3_mask-r-cnn.png)

## A sample of different models after training

![Image of example segmentation results](https://github.com/Ermaconomist/DeepLearningVision/blob/main/img/4_models.png)

## Final comparison of the Models with tensorboard

![Image of model results](https://github.com/Ermaconomist/DeepLearningVision/blob/main/img/5_results.png)


@misc{matterport_maskrcnn_2017,
  title={Mask R-CNN for object detection and instance segmentation on Keras and TensorFlow},
  author={Waleed Abdulla},
  year={2017},
  publisher={Github},
  journal={GitHub repository},
  howpublished={\url{https://github.com/matterport/Mask_RCNN}},
}
