# APRN 

> 🚧 **Note:** The detailed training and inference code is currently being organized and will be released soon.

This repository contains the (upcoming) official implementation of **APRN**, a method for Few-Shot Semantic Segmentation.

Once the code is fully released, this repository will include:


## 🔧 Requirements

We recommend the following environment configuration:

```bash
Python = 3.7
Pytorch = 1.8.0
CUDA = 11.1
```

Install other dependencies via:

```bash
pip install -r requirements.txt
```

---

## 📁 Data Preparation

### 🔹 PASCAL VOC 2012

We follow **[MaskContrast](https://github.com/wvangansbeke/Unsupervised-Semantic-Segmentation)** to prepare the data.

1. Download **PASCAL VOC 2012** from:
   [https://drive.google.com/file/d/1pxhY5vsLwXuz6UHZVUKhtb7EJdCg2kuH/view](https://drive.google.com/file/d/1pxhY5vsLwXuz6UHZVUKhtb7EJdCg2kuH/view)

2. Unzip the dataset and organize it as:

```shell
VOCSegmentation
├── images
├── SegmentationClassAug
├── saliency_supervised_model
└── sets
```

---

### 🔹 COCO 2014

1. Download **COCO 2014** from:
   [https://cocodataset.org/#download](https://cocodataset.org/#download)

2. Preprocess the dataset:

```bash
cd data/data_preprocess
python coco.py train2014
python coco.py val2014
```
3. Ensure the directory structure:

```shell
coco
├── train2014
├── val2014
├── masks_train2014
├── masks_val2014
├── saliency_supervised_model
├── val2014.txt
└── train2014.txt
```


## 📬 Contact

If you have any questions before the full release, feel free to open an issue or contact the repository maintainer.


