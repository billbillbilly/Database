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
- [Deep Learning the City: Quantifying Urban Perception at a Global Scale](https://link.springer.com/chapter/10.1007/978-3-319-46448-0_12#Tab1)
- [Modeling restorative potential of urban environments by coupling viewscape analysis of lidar data with experiments in immersive virtual environments](https://www.sciencedirect.com/science/article/pii/S016920461930831X)
- [Prediction method of Soundscape Impressions using Environmental Sounds and Aerial Photographs](https://arxiv.org/pdf/2209.04077.pdf)
