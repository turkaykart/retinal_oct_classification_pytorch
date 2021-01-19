

### English version: basic_deep_learning_model_in_medical_imaging.ipynb
### Turkce versiyon: medikal_goruntulemede_derin_ogrenme.ipynb 
Asagida yazilan bilgilerin Turkce cevirisini notebook icinde (medikal_goruntulemede_derin_ogrenme.ipynb) bulabilirsiniz.

---

# Building a Basic Deep Learning Model in Medical Imaging: Classification of Retinal OCT Images in PyTorch

In this notebook, we present the basic building blocks of deep learning in medical imaging. Our goal is to provide a high-level introduction for those interested in medical deep learning with PyTorch. Our task is to classify retinal OCT images as diabetic retinopathy or healthy. 

## Development Environment and Tools

You can run this notebook on [Google Colab](https://colab.research.google.com/) which includes [PyTorch](https://pytorch.org/). Alternatively, you can run this notebook in your local environment by configuring a [Jupyter Notebook](https://jupyter.org/) or [Lab](https://jupyter.org/) with [PyTorch](https://pytorch.org/).

## Imaging Data

We use a public dataset called "OCTID: Optical Coherence Tomography Image Database" [1] and can be downloaded with the following: 

1) [Download Link 1](https://dataverse.scholarsportal.info/dataverse/OCTID)
2) [Download Link 2](http://doi.org/10.3886/E108503V1)


[[1]](https://arxiv.org/ftp/arxiv/papers/1812/1812.07056.pdf) Peyman Gholami, Priyanka Roy, Mohana Kuppuswamy Parthasarathy, Vasudevan Lakshminarayanan, "OCTID: Optical Coherence Tomography Image Database", arXiv preprint arXiv:1812.07056, (2018)

## Data Organization

After obtaining the data, you should divide your dataset into 3 directories:

```
demo_retinal_oct/train/
```
```
demo_retinal_oct/val/
```
```
demo_retinal_oct/test/
```

Each of these 3 directories should have subdirectories that are named with your label names and have the corresponding retinal OCT images. For example,

```
demo_retinal_oct/train/diabetic_retinopathy/      (80% of diabetic retinopathy images)
demo_retinal_oct/train/healthy/                   (80% of healthy images)
```
```
demo_retinal_oct/val/diabetic_retinopathy/        (10% of diabetic retinopathy images)
demo_retinal_oct/val/healthy/                     (10% of healthy images)
```
```
demo_retinal_oct/test/diabetic_retinopathy/       (10% of diabetic retinopathy images)
demo_retinal_oct/test/healthy/                    (10% of healthy images)
```

You are free to change this directory structure. If you change it, you should also update the section of the code where we load these datasets with PyTorch.

## Next Step

After setting up your environment and organizing your datasets, you are all set to run the code!


### **Author: Turkay Kart** 

* **Email**:    t.kart@imperial.ac.uk
* **Twitter**:  [@turkaykart](https://twitter.com/turkaykart)


If you use the notebook for your research or teaching, please consider citing this Github repo:

```
Turkay Kart, "Building a Basic Deep Learning Model in Medical Imaging: Classification of Retinal OCT Images in PyTorch", (2021), GitHub repository, https://github.com/turkaykart/retinal_oct_classification_pytorch
```
```
@misc{kart2021retinal,
  author = {Kart, Turkay},
  title = {Building a Basic Deep Learning Model in Medical Imaging: Classification of Retinal OCT Images in PyTorch},
  year = {2021},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/turkaykart/retinal_oct_classification_pytorch}}
}
```
