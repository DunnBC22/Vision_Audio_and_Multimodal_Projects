<h1>Computer Vision, Audio, & Multimodal Projects</h1>

This repository houses both semi-structured and non-structured projects that both were not completed using Spark and are not Natural Language (NLP) projects.

<details open>

<summary>Computer Vision</summary>

<br />

<caption>
    Computer Vision (currently) includes image classification (binary, multiclass, and multilabel) and object detection projects.
</caption>

<br />

<h3>
    Binary Image Classification
</h3>

<br />

| Project Name | Accuracy | F1-Score | Precision | Recall |
| :----------: | :----------: | :----------: | :----------: | :----------: |
| Bart vs Homer | 0.9863 | 0.9841 | 0.9688 | 1.0 |
| Brain Tumor MRI Images | 0.9216 | 0.9375 | 0.8824 | 1.0 |
| COVID19 Lung CT Scans | 0.94 | 0.9379 | 0.9855 | 0.8947 |
| Car or Motorcycle | 0.9938 | 0.9939 | 0.9951 | 0.9927 |
| Dogs or Cats Image Classification | 0.99 | 0.9897 | 0.9885 | 0.9909 |
| Male or Female Eyes | 0.9727 | 0.9741 | 0.9818 | 0.9666 |

<br />

<h3>
    Multiclass Image Classification
</h3>

| Project Name | Accuracy | Macro F1-Score | Macro Precision | Macro Recall | Best Algorithm |
| :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| Brian Tumors Image Classification[^1] | 0.8198 | 0.8054 | 0.8769 | 0.8149 |Vision Transformer (ViT) |
| Diagnoses from Colonoscopy Images | 0.9375 | 0.9365 | 0.9455 | 0.9375 | - |
| Human Activity Recognition | 0.8381 | 0.8394 | 0.8424 | 0.839 | - |
| Intel Image Classification | 0.9487 | 0.9497 | 0.9496 | 0.95 | - |
| Landscape Recognition | 0.8687 | 0.8694 | 0.8714 | 0.8687 | - |
| Lung & Colon Cancer | 0.9994 | 0.9994 | 0.9994 | 0.9994 | - |
| Mango Leaf Disease Dataset | 1.0 | 1.0 | 1.0 | 1.0 | - |
| Simpsons Family Images | 0.953 | 0.9521 | 0.9601 | 0.9531 | - |
| Vegetable Image Classification | 1.0 | 1.0 | 1.0 | 1.0 | - |
| Weather Images | 0.934 | 0.9372 | 0.9398 | 0.9354 | - |

<br />

<h3>
    Multilabel Image Classification
</h3>

| Project Name | Subset Accuracy | F1 Score | ROC AUC |
| :----------: | :----------: | :----------: | :----------: |
| Futurama - ML Image CLF | 0.9672 | 0.9818 | 0.9842 |

<br />

<h3>
    Object Detection
</h3>

| Project Name | Avg. Precision[^3] | Avg. Recall[^4] |
| :----------: | :----------: | :----------: |
| License Plate Object Detection | 0.513 | 0.617 |
| Pedestrian Object Detection | 0.560 | 0.745 |

</details>

<details>

<summary>Document AI Projects</summary>

<br />

<h3>
    Multiclass Classification
</h3>

| Project Name| Accuracy | Macro F1 Score | Macro Precision | Macro Recall |
| :---: | :---: | :---: | :---: | :---: |
| Document Classification - Desafio_1 | 0.9865 | 0.9863 | 0.9870 | 0.9861 |
| Real World Documents Collections | 0.767 | 0.7704 | 0.7767 | 0.7707 |
| Real World Documents Collections_v2 | 0.826 | 0.8242 | 0.8293 | 0.8237 |
| Tobacco-Related Documents | 0.7532 | 0.722 | - | - |
| Tobacco-Related Documents_v2 | 0.8666 | 0.8308 | - | - |
| Tobacco-Related Documents_v3 | 0.9419 | 0.9278 | - | - |

</details>

<details>

<summary>Audio Projects</summary>

<br />

| Project Name | Project Type |
| :---: | :---: |
| Vinyl Scratched or Not | Binary Audio Classification |
| Audio-Drum Kit Sounds | Multiclass Audio Classification |
| Speech Emotion Detection | Emotion Detection |
| Toronto Emotional Speech Set (TESS) | Emotion Detection |
| ASR Speech Recognition Dataset | Automatic Speech Recognition |
</details>

<details>

<summary>Optical Character Recognition Projects</summary>

<br />

| Project Name | CER[^2] |
| :---: | :---: |
| 20,000 Synthetic Samples Dataset | 0.0029 |
| Captcha | 0.0075 |
| Handwriting Recognition (v2) | 0.0533 |
| Handwriting Recognition (v2) | 0.0360 |
| OCR License Plate Text Recognition | 0.0368 |

</details>

<br />

Footnotes:

[^1]: This project is a transformer comparison.

[^2]: CER is Character Error Rate.

[^3]: Average Precision (AP) @[IoU=0.50:0.95 | area=all | maxDets=100]

[^4]: Average Recall (AR) @[IoU=0.50:0.95 | area=all | maxDets=100]