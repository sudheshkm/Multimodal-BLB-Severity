# Multimodal Fusion of Visual and Lesion Features for Mobile-Based Severity Assessment of Rice Bacterial Leaf Blight

This repository contains the implementation associated with the manuscript:

**"Multimodal Fusion of Visual and Lesion Features for Mobile-Based Severity Assessment of Rice Bacterial Leaf Blight"**

The present implementation is distinct from the original Detectron2-based RCAMNet implementation reported in our earlier work. The current framework was redesigned for lightweight offline mobile deployment.

## Current framework

The proposed pipeline consists of:

1. Lightweight U-Net for rice leaf segmentation
2. HSV-based lesion mask generation
3. Lesion-specific handcrafted descriptors
4. MobileNetV2 with CBAM for visual feature extraction
5. Feature-level fusion of visual and structured lesion features
6. Severity classification

The structured lesion descriptors include lesion size, GLCM texture features, mean hue, and dominant lesion colour.

## Code

The main implementation is provided in:

`multimodal/Multimodal_Fusion_BLB_Severity.ipynb`

## Dataset

BLBVisionDB is not redistributed with this repository. The dataset is available from the corresponding author upon reasonable request.

## Reproducibility

The notebook contains the model definition, preprocessing, lesion feature extraction, training procedure, and evaluation procedure used for the reported experiments.

The final test evaluation uses the complete 329-image test set reported in the manuscript.

## Previous RCAMNet implementation

The original RCAMNet implementation used Detectron2-based multiclass segmentation and is retained separately for reference. It should not be interpreted as the implementation of the present manuscript.

## Code archive

A versioned copy of the implementation associated with this manuscript is deposited in Zenodo.

DOI: 10.5281/zenodo.23078360
