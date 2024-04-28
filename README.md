# TCAV
Quantitative Testing with Concept Activation Vectors in PyTorch

Unizip

## Environment
- Ubuntu 16.04
- NVIDIA GeForce 1080
- CUDA 10.1
torch==1.8.1

## Download and preprocess data
```
cd imagenet
# Download broden dataset
curl -O http://netdissect.csail.mit.edu/data/broden1_224.zip
mkdir "broden1_224"
unzip broden1_224.zip -d broden1_224
rm broden1_224.zip
```
```
python download_and_make_datasets.py
# three parameters: source_dir, number_of_images_per_folder, number_of_random_folders
# Look https://github.com/tensorflow/tcav/blob/master/Run_TCAV.ipynb
```
Copy these dirs (Concept dirs, label dir, random dirs) to Dir 'image_net_subsets'.

![img](img/fig1.png)

## Run
```
python run.py
```
