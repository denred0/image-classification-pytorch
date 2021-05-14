# Image Classification PyTorch

Use pretrained models to train your data.





## :closed_book: Table of content
- [What's New](#whats-new)
- [Installation](#installation)
- [Quick start](#quick-start)
- [Prediction](#prediction)
- [Data preparation](#data-preparation)
- [Models](#models)
- [License](#license)

## :clipboard: What's New <a name="whats-new"></a>


## :computer: Installation <a name="installation"></a>

```python
pip install image-classification-pytorch
```
---

## ✨ Quick Start <a name="quick-start"></a>

```python
import image_classification_pytorch as icp

# add model
tf_efficientnet_b4_ns = {'model_type': 'tf_efficientnet_b4_ns', 'im_size': 380, 'im_size_test': 380, 'batch_size': 8, 'mean': [0.485, 0.456, 0.406], 'std': [0.229, 0.224, 0.225]}
models = [tf_efficientnet_b4_ns]

# create trainer
trainer = ICPTrainer(models=models, data_dir='my_data')
# start training
trainer.fit_test()
```

#### Example 
[Simple example of training and prediction](https://github.com/denred0/image_classification_pytorch/blob/master/examples/image_classification_pytorch_get_started.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1M7oJDizCOrFTDJz0CaDy-ClvDMUvmlnv?usp=sharing)

---

## :telescope: Prediction <a name="prediction"></a>

## :file_folder: Data Preparation <a name="data-preparation"></a>
Prepare data for training in the following format

    ├── animals                      # Data folder
        ├── dogs                     # Folder Class 1
        ├── cats                     # Folder Class 2
        ├── gray_bears               # Folder Class 3
        ├── zebras                   # Folder Class 4
        ├── ...
 
---
## :chart_with_downwards_trend: Models <a name="models"></a>



## 🛡️ License <a name="license"></a>
Project is distributed under [MIT License](https://github.com/denred0/image_classification_pytorch/blob/master/LICENSE.txt)
