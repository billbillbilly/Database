# Multisensory perception - [1st Annual SEAS Hackathon@the SEAS Sustainable Future Hub](https://sites.google.com/umich.edu/hackathon/home)
## Overview
Team will make use of provided datasets, scripts, and other resources to explore innovative method to extract information from vison and auditory.  

Team can think of some potential focuses:
- Photo-based viewshed analysis
- Training soundscape prediction based on pairwised comparison labels
- Predicting soundscape using sounds and photos

## Datasets
Provided datasets include photos and sounds/spectrograms collected from 200 locations across the city core of Ann Arbor, MI.

- Spatial points of [200 locations](https://github.com/billbillbilly/Database/tree/main/viewscape_data)
- 360-degree photos 
- Spectrograms extracted from outdoor sounds recordings
- Pretrained model for sematic segmentation based on CamVid dataset
- Pretrained model for soundscape emotional response prediction based on [Emo-soundscpes](https://metacreation.net/emo-soundscapes/) dataset
- other data source: 
	- [PlacePlus 2.0](https://www.dropbox.com/s/grzoiwsaeqrmc1l/place-pulse-2.0.zip?dl=0)
	- [KITTI dataset](http://www.cvlibs.net/datasets/kitti/eval_object.php?obj_benchmark=3d)

## Potential Packages 
- ```fastai``` a python package for training neuralnetwork
- ```viewscape``` an R package for computing land information within viewshed

## Scripts
- Semantic segmetation
- Visible greeness extraction
- Soundscape emotion prediction
- Image depth estimation

## Recommanded Readings
- [Salesses, P., Schechtner, K., & Hidalgo, C. A. (2013). The collaborative image of the city: mapping the inequality of urban perception. PloS one, 8(7), e68400.](https://link.springer.com/chapter/10.1007/978-3-319-46448-0_12#Tab1)
- [Tabrizian, P., Baran, P. K., Van Berkel, D., Mitasova, H., & Meentemeyer, R. (2020). Modeling restorative potential of urban environments by coupling viewscape analysis of lidar data with experiments in immersive virtual environments. Landscape and Urban planning, 195, 103704.](https://www.sciencedirect.com/science/article/pii/S016920461930831X)
- [Ono, Y., Hara, S., & Abe, M. (2022). Prediction method of Soundscape Impressions using Environmental Sounds and Aerial Photographs. arXiv preprint arXiv:2209.04077.](https://arxiv.org/pdf/2209.04077.pdf)

## Usage of this instruction
1. Get a Google account and set up a folder in your Google Drive. 
In this case, let's assume you create a folder called 'multisensory_data'

2. Create a new Google [Colab](https://colab.research.google.com/) file (jupyter notebook) in the folder.
In Colab, you should connect to your Google Drive and set up the work directory.

Here is what you run in your first code cell:

```
from google.colab import drive
drive.mount('/content/drive')
# setup working directory to a folder in Google Drive
import os 
root_dir = "/content/drive/My Drive/"
# set folder name (this folder should exist in 'root_dir')
project_folder = "multisensory_data/"

def set_working_directory(project_folder):
  # change the OS to use your project folder as the working directory
  os.chdir(root_dir + project_folder)
  print('\nYour working directory was changed to ' + root_dir + project_folder + \
        "\n\nYou can also run !pwd to confirm the current working directory." )

set_working_directory(project_folder)
```

Then, you can clone this repo in your work directory with the code below in your second code cell:

```
! git clone https://github.com/billbillbilly/Database.git
```
Well done! Now you are able to start!
