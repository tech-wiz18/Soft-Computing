# Soft-Computing

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
