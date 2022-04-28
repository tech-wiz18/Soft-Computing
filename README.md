<h1 align="center">Face Recognition using Neural Evolution</h1>
<h4 align="center"> Aman Mishra (ECE), Megha Garg (SMST) </h4>

### ABSTRACT

pass

### NOVEL TECHNIQUES USED :-

 - **WAVELET TRANSFORMATION** - To reduce computational complexity for PCA Calculations

    Result :-

    <img src= "assets/gray_64X64.png"> </br>
    <img src= "assets/wavelet_35X35.png"> </br>


## Requirements

 - python>3.7</br>
 - OpenCV
 - numpy
 - torch>=1.8.0 (With CUDA 11.1)

## Instructions

 * Clone this Repo
```bash
git clone https://github.com/tech-wiz18/Soft-Computing.git
```

### Dataset

We used **LFW-Cropped**(Labelled Faces in the Wild Cropped) dataset as our standard face recognition dataset.

```bash
## run following commands to download dataset in the folder (Colored version)

cd Soft-Computing
wget https://conradsanderson.id.au/lfwcrop/lfwcrop_color.zip 
unzip lfwcrop_color.zip
```

### DATA-STRUCTURING

TO properly arrange dataset in train-test we used [THIS NOTEBOOK](notebooks/data_prepare.ipynb)

 - Used (80-20) Splitting ratio.
 - Keep only those person which are having more than one images.


## References
 * [WHAT ARE WAVELET TRANSFORMS?](https://en.wikipedia.org/wiki/Wavelet_transform)
 * [pywavelet docs](https://pywavelets.readthedocs.io/en/latest/ref/2d-dwt-and-idwt.html#ref-dwt2) - Wavelet Transformation Library for python.
 * [Sklearn PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)