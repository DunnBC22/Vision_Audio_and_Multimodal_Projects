

<h1>Transformer Comparison Using Brain Tumor (Multiclass Image Classification)</h1>

<p align='center'>
    The purpose of this project was to train <strong><em>seventeen (17)</em></strong> different transformers on the same dataset to see which one is the most efficient and effective. All projects are the same with the exception of the transformer used.
</p>

<p align='center'>
    <span style="font-size: 18px">
        <strong>
            Sample Images
        </strong>
    </span>
</p>    

<p align='center'>
    <img src="./Images/Sample Images.png" alt="Class Distribution of Evaluation Dataset" height=600 width=600>
</p>

<p align='center'>
    <span style="font-size: 18px">
        <strong>
            Further Details on Methodology
        </strong>
    </span>
</p>

<p align='center'>
I trained each model for 3 epochs on apple's 'mps'.
</p>

<p align='center'>
    <span style="font-size: 18px">
        <strong>
            Dataset Name
        </strong>
    </span>
</p>

<p align='center'>
    Brain Tumor Classification MRI
</p>

<p align='center'>
    <span style="font-size: 18px">
        <strong>
            Dataset Source
        </strong>
    </span>
</p>

<p align='center'>
    <a href='https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri'>
        Brain Tumor Classification MRI
    </a>
</p>

<p align='center'>
    <span style="font-size: 18px">
        <strong>
            Class Distribution
        </strong>
    </span>
</p>
<p align="center">
    <em>Training Dataset</em>
</p>

<p align="center">
    <img src="./Images/Class Distribution - Training Dataset.png" alt="Class Distribution of Training Dataset" height=385 width=550>
</p>

<p align="center">
<em>Evaluation Dataset</em>
</p>

<p align="center">
    <img src="./Images/Class Distribution - Testing Dataset.png" alt="Class Distribution of Evaluation Dataset" height=385 width=550>
</p>

<hr />

<p align='center'>
    <span style="font-size: 26px">
        <strong>
            Results
        </strong>
    </span>
</p>

| Transformer Model | Checkpoint  | Training Duration (Min) | Memory (GB) |  Loss  | Accuracy |  F1  | Recall | Precision |
| :--------------:  | :---------------------: | :---------------: | :--------: | :-------: | :-------: | :-------: | :-------: | :-------: |
| **BEiT** | `microsoft/beit-base-patch16-224` | 109 | 3.79 | 1.9943 | 0.7056 | 0.6507 | 0.6830 | 0.7451 |
| **BiT** | `google/bit-50` | 153 | 1.04 | 2.3367 | 0.7005 | 0.6461 | 0.6791 | 0.8164 |
| **ConvNeXt_V2** | `convnextv2-base-22k-224` | 135 | 3.86 | 2.0777 | 0.2437 | 0.1969 | 0.2470 | 0.1834 |
| **CvT** | `microsoft/cvt-13` | 59 | 0.8651 | 1.2689 | 0.7640 | 0.7246 | 0.7543 | 0.8498 |
| **DeiT** | `facebook/deit-base-distilled-patch16-224` | 181 | 3.78 | 1.8587 | 0.8046 | 0.7814 | 0.7996 | 0.8710 |
| **DiNAT** | `shi-labs/dinat-base-in1k-224` | 333 | 3.91 | 1.7133 | 0.7589 | 0.7322 | 0.7427 | 0.8548 |
| **EfficientFormer** | `snap-research/efficientformer-l3-300` | 51 | 1.34 | 2.2761 | 0.7817 | 0.7465 | 0.7771 | 0.8613 |
| **EfficientNet** | `google/efficientnet-b5` | 363 | 1.25 | 0.9410 | 0.8020 | 0.7802 | 0.7977 | 0.8682 |
| **Levit** | `facebook/levit-256` | 25 | 0.7659 |  98.6443 | 0.7437 | 0.7031 | 0.7309 | 0.7796 |
| **NAT** | `shi-labs/nat-base-in1k-224` | 235 | 4.62 | 1.9715 | 0.7792 | 0.7515 | 0.7688 | 0.8544 |
| **PoolFormer** | `sail/poolformer_s36` | 52 | 1.34 | 1.7590 | 0.7665 | 0.7314 | 0.7577 | 0.8606 |
| **RegNet** | `facebook/regnet-y-064` | 145 | 1.29 | 1.1561 | 0.8046 | 0.7839 | 0.7978 | 0.8736 |
| **ResNet** | `microsoft/resnet-101` | 69 | 1.87 | 1.1940 | 0.6701 | 0.6302 | 0.6611 | 0.7733 |
| **Swin V2** | `microsoft/swinv2-base-patch4-window12to24-192to384-22kto1k-ft` | 805 | 3.83 | 1.8574 | 0.6447 | 0.5922 | 0.6249 | 0.7436 |
| **VAN** | `Visual-Attention-Network/van-base` | 114 | 1.15 | 1.7847 | 0.7919 | 0.7665 | 0.7865 | 0.8675 |
| **Vision Transformer (ViT)** | `google/vit-base-patch16-224-in21k` | 139 | 3.78 | 0.8584 | 0.8198 | 0.8054 | 0.8149 | 0.8769 |
| **ViT-MSN** | `facebook/vit-msn-base` | 135 | 3.78 | 1.8106 | 0.7690 | 0.7347 | 0.7588 | 0.8477 |

<hr />

<p align='center'>
    <span style="font-size: 20px">
        <strong>
            Notes on Above Table
        </strong>
    </span>
</p>
<ul>
    <li>Training durations are approximate because many (but not all) times I trained two projects at the same time. Additionally, times are rounded to the nearest whole minute. They are just meant to be a relative idea of durations.</li>
    <li>Memory includes all <strong>3 epochs</strong> and files saved to local hard drive.</li>
    <li>F1, Recall, and Precision are the <strong>macro averaged</strong> version for each of those calculations.</li>
</ul>

<p align='center'>
    <span style="font-size: 20px">
        <strong>
            Conclusions
        </strong>
    </span>
</p>
<ul>
<li>The fastest model was Levit. Even though the results were about 7.5 percent worse (overall) than ViT (which I used as the baseline for comparisons), it was so quick that you could run it five times as many iterations as ViT and still have time leftover. I am curious how the results of running Levit five times as many iterations would compare to the results from ViT.</li>
<li>The surprising model that I will keep in mind for the future: regnet similar metrics to ViT, yet uses less hard drive memory</li>
<li>I was most surprised that with all of the alternatives to ViT, none of them outperformed ViT</li>
<li>I will remove about half of the models from my HuggingFace Portfolio as they underperformed to the point that I see no reason to retain them. The models I will remove are: 
    <ul>
        <li>convnextv2-base-22k-224</li>
        <li>facebook/vit-msn-base</li>
        <li>microsoft/resnet-101</li>
        <li>microsoft/beit-base-patch16-224</li>
        <li>google/bit-50</li>
        <li>microsoft/cvt-13</li>
        <li>shi-labs/dinat-base-in1k-224</li>
        <li>microsoft/swinv2-base-patch4-window12to24-192to384-22kto1k-ft</li>
        <li>shi-labs/nat-base-in1k-224</li>
    </ul>
</li>
</ul>