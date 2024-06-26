# Accuracy-Loss-Evaluation

[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)

## Table of Contents

- [Introduction](#Introduction)
- [Implement](#Implement)
- [Experiment](#Experiment)
- [License](#license)

## Introduction 


In this paper "Rapid Accuracy Loss Evaluation for Quantized Neural Networks Using Attention-Based Multifactor Modeling", This paper proposes a multifactor modeling method based on attention mechanisms, 
which aims to analyse and simulate the relationship between quantization factors and neural network performance, thereby providing a method to quickly and accurately assess post-training quantization 
accuracy loss. Experimental results show that this method can quickly predict the accuracy of different neural network models on various computational tasks without relying on extensive test data, 
with a prediction error of only about 2%, effectively supporting rapid model development and iterative optimization.

## Implement

Result.py for Execute Script, to Reproduce experimental results.

```sh
$ python Vit_accuracy_Loss_evaluation.py
```


## Experiment
Classification Application

We consider convolutional neural networks (CNNs) trained on standard datasets for the popular task of image classification. The neural networks adopted in the experiments are MobileNetV2, ResNet50 and VGG16. These neural networks are quantized to INT8, INT4, INT2, and a mixture of them.

| Model | label Accuracy | Prediction accuracy | Prediction error  |
| ------ | ------ | ------ | ------ |
| MobileNetV2_1 | 82.86% | 84.28% | 1.42% | 
| MobileNetV2_2 |	83.81% | 87.53% | 3.72% |
| MobileNetV2_3 | 80.48% | 81.84% | 1.36% |
| MobileNetV2_4 |  82.86% | 84.38% | 1.52% |
| MobileNetV2_5 | 81.43% | 83.67% | 2.24% |
| Average | - | - | 2.05% |

| Model | label Accuracy | Prediction accuracy | Prediction error  |
| ------ | ------ | ------ | ------ |
| ResNet50_1 | 88.58% | 89.95% | 1.37% | 
| ResNet50_2 |	87.21% | 88.59% | 1.38% |
| ResNet50_3 | 86.38% | 83.64% | 2.74% |
| ResNet50_4 |  83.31% | 85.46% | 2.15% |
| ResNet50_5 | 85.13% | 83.20% | 1.93% |
| Average | - | - | 1.91% |

| Model | label Accuracy | Prediction accuracy | Prediction error  |
| ------ | ------ | ------ | ------ |
| VGG16_1 | 87.06% | 86.62% | 0.44% | 
| VGG16_2 |	87.55% | 86.63% | 0.92% |
| VGG16_3 | 85.45% | 86.56% | 1.11% |
| VGG16_4 | 85.69% | 85.47% | 0.22% |
| VGG16_5 | 86.67% | 86.64% | 0.03% |
| Average | - | - | 0.54% |

## License

[Xi’an Microelectronics Technology Institute](LICENSE) © ycjcy
