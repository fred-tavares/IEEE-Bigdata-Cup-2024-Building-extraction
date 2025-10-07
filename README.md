https://www.kaggle.com/competitions/building-extraction-generalization-2024/overview
Problem Statement: Detect building footprints from 0.3 m Google Earth satellite images of Japan with the purpose of city cross-generalization.


Model chosen: Detectron 2, provides pretrained checkpoints for COCO objects, so it was the first choice for this attempt. Parameters were tuned to achieve the best result possible
Evaluation metric: The evaluation of results utilizes the object-wise F1-score, using an IoU=0.5

Image pre processement of the data was used for some improvement. Histogram equalization was used but with no detected improvement. Some gamma reduction followed by a contrast bumb was seen to have the edge.

On the Kaggle submission platform, this model achieved a private score of 0.5053

Due to the generalization nature of the problem, a simple image pre processing and fine-tunning of a deep learning model was not enough to achieve a truly good result on this challange. More research was needed.
