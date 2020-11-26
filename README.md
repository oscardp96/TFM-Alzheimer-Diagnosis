# Alzheimer Diagnosis with Deep Learning
## MASTER DEGREE'S FINAL PROJECT

This repository contains all code snippets and reports for a master's degree thesis focused on automatic Alzheimer diagnosis using Deep Learning and MRI images. The files and folder structure are organized in the following way:

* `Memoria(SPANISH).pdf` is a complete, 79 pages report with all the information about the project. It is written in Spanish, and contains every detail about the current state of the art and the development of the project.
* `JournalArticle.pdf` is a more condensed, less detailed report that resembles a journal article. It is written in English, and contains an overview of the entire project.

Then, the `Code` folder contains the jupyter notebooks used in Google Colaboratory for the development of the deep learning models. It contains the following notebooks:

* `ImagePreprocessing`. Several experiments and organization of the MRI images. Image registration and skull-stripping is performed in this notebook, as well as other experiments useful for familarizing with the image format (`.nii`).
* `BuildingTFRecordsDB`. Using the preprocessed images, several TFRecords files are created in this notebook. This file format is much faster to read than native Python generators, and does not consume as much RAM as loading all images in memory.
* `Fine-tuning of InceptionV3`. First model built. Fine-tuning an InceptionV3 network trained with ImageNet for classifiying between healthy, demented and MCI patients.
* `Using a ResNet3D`. Second model built. Training a 3-dimensional residual network for classifiying between healthy, demented and MCI patients.

The data used for the development of this project could not be placed on this repository, since the MRI images are private and were obtained from the Alzheimer's Disease Neuroimaging Initiative (ADNI) database. As such, the investigators within the ADNI contributed to the design and implementation of ADNI and/or provided data, but did not participate in this project.
