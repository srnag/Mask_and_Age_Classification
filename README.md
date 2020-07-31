# Project: Mask and Age Classification 

## Table of Contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Dataset](#dataset)
* [Trained Model](#trained-model) 
* [Setup](#setup)
* [Image Classification Screenshots](#image-classification-screenshots)
* [Video Classification](#video-classification)
* [Features](#features)
* [Inspiration](#inspiration)
* [Contributors](#contributors)


## General Info
With the rapid spread of COVID-19 we find ourselves plunged into a global health crisis where face masks are essential tool to limit the virus spread. As we already know, older people are less immune on this virus and it is crucial that more people are taking wearing a face mask into practice. Therefore, we have decided to create an algorithm which will recognize those who are participating and helping the public safety and those who do not, separating them in four groups:

| No.  | Group name  | Number of files |
| ------------- | ------------- | ------------- |
|1 | old_with_mask  | 381 |
|2| old_without_mask |  355 |
|3| young_with_mask  | 346  |
|4| young_without_mask  | 369 |

Sometimes it could be quite difficult to find the correct dataset for launching a Machine Leaning project, especially when you have to use lots of faces. For that reason, we created our own dataset by generating synthetic faces using GAN, asking our friends for their permission for using their photos, as well as downloading images from free repositories available on the Internet. 


## Technologies
* Tech 1 - version 1.0
(prvo da probame koj model ke funkcionira posle toa ke stavam koj model i sto tehnologii se koristeni)
Toni

## Dataset
* Link to dataset
https://drive.google.com/file/d/14RjXeKji5mtuWSB7Xbvnq4kWDeDpLGjj/view?usp=sharing (ova e link so view na datasetot (neznam dali e dobra opcijata edit na istiot da ja stavam))

## Trained Model
* Link to model (prvo da probame koj model ke funkcionira posle toa ke stavam link od modelot)
Toni

## Setup
Describe how to install / setup your local environement / add link to demo version.
Filip

## Image Classification Screenshots
![Example screenshot](./img/screenshot.png)
isto kako i tie pogornite :)
Toni

## Video Classification

![](https://github.com/FilipAngelov/Mask_and_Age_Classification/tree/master/other/gif-petar.gif)

## Code Examples
Show examples of usage:
`put-your-code-here`
Filip

## Features
List of features ready and ToDos for future development
* Image classification function 'predict_url' which can be used to classify a picture by inserting the url.
** Example: predict_url('https://i.pinimg.com/originals/db/00/0e/db000e66cc61d4f15a6c2b04916bfc9c.jpg')
* Video classification function which runs the web camera, locates face on video, and classifies between the four classes. 
**

To-do list:
* Out of sample validation showed that the classification errors occur mostly in the old with mask class which usually gets classfied as young with mask. Collecting more data could potentialy improve model's accuracy on this error. Another possible solution is to have two classifiers instead of currently only one. The first classifier will classify between with_mask and without_mask, and the second one will classify between old and young. 


## Inspiration
Add here credits. Project inspired by..., based on...
SRNA

## Contributors

Thanks to the following people who have contributed to this project:

* [@FilipAngelov](https://github.com/FilipAngelov) 
* [@jolakoskip](https://github.com/jolakoskip) 
* [@gardnerska](https://github.com/gardnerska) 
* [@srnag](https://github.com/srnag)
* [@tonipesic](https://github.com/tonipesic)
