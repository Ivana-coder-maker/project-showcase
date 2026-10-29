# Medical image analysis

**Imperial College London Summer School · Group project · Python**

[← All projects](../README.md)

## The project

The team built a workflow for dermoscopic image analysis: segmenting skin lesions, detecting visual attributes and generating findings reports consistent with the predictions. The project also included a bonus task for retrieving similar images.

This was an educational project, not a clinically validated diagnostic system.

## My contributions

### Prediction evaluation

I developed the evaluation component that compares predicted attribute masks with reference annotations. It calculates Dice, Intersection over Union (IoU), precision and recall, and provides visualisations for inspecting the results.

Metrics are reported separately for each attribute. In the integrated version, pairs where both masks are empty are excluded from averages, so the many cases without an attribute do not inflate segmentation scores. Cases with only one empty mask remain part of the evaluation.

### Retrieval bonus

I developed the image retrieval bonus using a pretrained CLIP model. Images are represented as embeddings and compared using cosine similarity. The output includes ranked neighbours, similarity scores and a CSV record of the retrieved image IDs.

I also implemented visualisations that show a query image alongside its retrieved neighbours. These make the retrieval results easier to inspect and discuss.

The segmentation, attribute-detection model and report-generation components were handled by other members of the group.

### Supporting data preparation

I also helped a teammate prepare for model training. The volume of images made the dataset difficult to work through, so we worked on preprocessing and sorting the images before training. My main implementation responsibilities remained evaluation and retrieval.

## Technologies

Python, NumPy, PyTorch, OpenCLIP and Pillow.

## Learning to work with Git

At the start, I did not yet know how to push or pull. My first version of collaboration was copy, paste, and ask a teammate to integrate my changes. Effective teamwork, less effective version control. I quickly started learning Git and the importance of synchronising changes and coordinating edits to shared files.

## Materials

The public showcase contains descriptions only. The team's source code, medical images, model weights and course materials are not distributed here.
