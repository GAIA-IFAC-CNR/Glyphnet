# Glyphnet

*Glyphnet* is a repository that includes an example of a deep learning approach to ancient Egyptian hieroglyphs classification, ...

If you use this repository, please cite it as:

A. Barucci, C. Cucci, M. Franci, M. Loschiavo and F. Argenti, **A Deep Learning Approach to Ancient Egyptian Hieroglyphs Classification**. IEEE Access, vol. 9, pp. 123438-123447, 2021, doi: 10.1109/ACCESS.2021.3110082, [IEEE DIRECT LINK](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9528382&isnumber=9312710)

@ARTICLE{9528382,  author={Barucci, Andrea and Cucci, Costanza and Franci, Massimiliano and Loschiavo, Marco and Argenti, Fabrizio},  journal={IEEE Access},   title={A Deep Learning Approach to Ancient Egyptian Hieroglyphs Classification},   year={2021},  volume={9},  number={},  pages={123438-123447},  doi={10.1109/ACCESS.2021.3110082}}

This document provides a quick introduction to the SCRIPT NAME HERE to help new users get started. In addition to the source code, we also provide a [link](https://en.wikipedia.org/wiki/Pyramid_of_Unas) to the dataset containing 4210 manually annotated images of Egyptian hieroglyphs found in the Pyramid of Unas. The dataset can be dowloaded [here](http://iamai.nl/downloads/GlyphDataset.zip).

Authors wishes to express their gratitute for the [seminal work of Franken](https://github.com/morrisfranken/glyphreader).


Please read the [LICENSE.md](./LICENSE.md) file before using *Glyphnet*.

## Abstract
Nowadays, advances in Artificial Intelligence (AI), especially in machine and deep learning, present new opportunities to build tools that support the work of specialists in areas apparently far from the information technology field. One example of such areas is that of ancient Egyptian hieroglyphic writing. In this study, we explore the ability of different convolutional neural networks (CNNs) to classify pictures of ancient Egyptian hieroglyphs coming from two different datasets of images. Three well-known CNN architectures (ResNet-50, Inception-v3 and Xception) were taken into consideration and trained on the available images. The paradigm of transfer learning was tested as well. In addition, modifying the architecture of one of the previous networks, we developed a specifically dedicated CNN, named Glyphnet, tailoring its complexity to our classification task. Performance comparison tests were carried out and Glyphnet showed the best performances with respect to the other CNNs. In conclusion, this work shows how the ancient Egyptian hieroglyphs identification task can be supported by the deep learning paradigm, laying the foundation for information tools supporting automatic documents recognition, classification and, most importantly, the language translation task.

![plot](./Features2_running.png)
![plot](./Glyphnet.tiff)

## Usage
To set up your system and use Glyphnet, follow the instruction in the [installation](https://github.com/GAIA-IFAC-CNR/Glyphnet/blob/main/INSTALL.md) file.

About the notebooks:
- [model](https://github.com/GAIA-IFAC-CNR/Glyphnet/blob/main/model.ipynb) keeps all the model we used, such as Xception, InceptionV3, Glyphnet etc.
- [util](https://github.com/GAIA-IFAC-CNR/Glyphnet/blob/main/util.ipynb) holds a set of useful functions that will be used along the entire code, e.g. to load the dataset, to plot the loss over training etc.
- [util_img](https://github.com/GAIA-IFAC-CNR/Glyphnet/blob/main/util_img.ipynb) has a bunch of useful functions to work on images, e.g. resize, background elaboration, getting some statistical indicator such as mean, variance etc.
- [dataset_preprocessing](https://github.com/GAIA-IFAC-CNR/Glyphnet/blob/main/dataset_preprocessing.ipynb) is the code dedicated to image preprocessing. It strongly uses util_img and outputs the datasets with resized and "cleaned" images.
- [classification_VFinal](https://github.com/GAIA-IFAC-CNR/Glyphnet/blob/main/classification_VFinal.ipynb) is the main code. Here Glyphnet's magic happens.
```
python Schizotypy_group_prediction.py --help

Usage: Schizotypy_group_prediction.py [-h] XLSX_file

A machine learning predicitive model, optimized in a nested stratified cross-validation loop repeated 1000 times

positional arguments:
  XLSX_file   XLSX file including data

optional arguments:
  -h, --help  show this help message and exit
```

## Testing (TO DO)

## Ouputs (TO DO)
The outputs are stored in two different folders: *Figures* contains the ROC curve plot and *csv\_results* includes all the csv files. Specifically:

* *CombsSelected.csv* reports the number of times each feature combination has been selected
* *Scores.csv* includes average and standard deviation values of balanced accuracy, area under the ROC curve, sensitivity and specificty obtained both in the training and test sets
* *tpr.csv* reports average true positive rate values (among repetitions and nested CV splits)

## Authors
* **Andrea Barucci, MSc, PhD** - *Researcher at the Institute of Applied Physics "Nello Carrara" (IFAC) – National Council of Research (CNR), Sesto Fiorentino, Italy.* Email address: <a.barucci@ifac.cnr.it>
* **Fabrizio Argenti, MSc, PhD** - *Associate Professor at the Department of Information Engineering (DINFO), University of Florence, Florence, Italy*. Email address: <fabrizio.argenti@unifi.it>
* **Tommaso Guidi, BSc** - *Master Degree student in Artificial Intelligence and Automation Engineering - Department of Information engineering and mathematics, University of Siena, Siena, Italy. Email address: <t.guidi@student.unisi.it>
* **Chiara Marzi, MSc, PhD** - *Postdoctoral Research Fellow at the Institute of Applied Physics "Nello Carrara" (IFAC) – National Council of Research (CNR), Sesto Fiorentino, Italy.* Email address: <c.marzi@ifac.cnr.it>
