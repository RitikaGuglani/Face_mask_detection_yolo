Face Mask Detection using YOLO-lite

This project implements an end-to-end face mask detection pipeline using a CNN-based object detector.
The dataset is annotated in Pascal VOC format and includes three classes: with_mask, without_mask, and mask_weared_incorrect.

The pipeline covers:
- Annotation parsing
- Model training
- Inference and visualization
- IoU-based evaluation

Limitations: Localization accuracy is limited due to simplified YOLO formulation.

The end to end pipeline implemented is as follows:
1. Raw Input
    Images + Pascal VOC XML
2. Pre-processing
    Resize
    Normalize
    Encode boxes + labels
3.Model
    CNN detector
4.Training
    model.fit()
5.Inference
    Run model on new images
6.Post-processing
    Decode predictions
    Draw bounding boxes
7.Output
    Saved images 
    metrics
8.Deployment artifact
    SavedModel
    TFLite