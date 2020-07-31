# Project: Mask and Age Classification 

## Table of Contents
* [General info](#general-info)
* [Technologies & Setup](#technologies-&-setup)
* [Dataset](#dataset)
* [Trained Model](#trained-model) 
* [Image Classification Screenshots](#image-classification-screenshots)
* [Video Classification](#video-classification)
* [Features](#features)
* [Inspiration](#inspiration)
* [Contributors](#contributors)


## General Info
With the rapid spread of COVID-19 we find ourselves plunged into a global health crisis where face masks are essential tool to limit the virus spread. As we already know, older people are less immune on this virus and it is crucial that more people are taking wearing a face mask into practice. Therefore, we have decided to create an algorithm which will recognize those who are participating and helping the public safety and those who do not, separating them in four groups:






## Technologies & Setup
Technologies
* We used Keras for model architecture, training, and prediction.
* Model training was done in Google Colab.
* Video classification should be done on local machine and we used Spyder.

Setup
* There is no need to install any of the libraries used in the notebook if you use Colab as they are preinstalled for you. 
* When performing video classification on your local machine please refer to the Requirements.txt file in the main repository.  
* You would need to import all the libraries used in the notebook. All the libraries used are listed in the Project.ipynb file.


## Dataset
* Sometimes it could be quite difficult to find the correct dataset for launching a Machine Leaning project, especially when you have to use lots of faces. For that reason, we created our own dataset by generating synthetic faces using GAN, asking our friends for their permission for using their photos, as well as downloading images from free repositories available on the Internet. 
* Below is a summary of our dataset.

| No.  | Group name  | Number of files |
| ------------- | ------------- | ------------- |
|1 | old_with_mask  | 381 |
|2| old_without_mask |  355 |
|3| young_with_mask  | 346  |
|4| young_without_mask  | 369 |

* [Link to dataset](https://drive.google.com/file/d/14RjXeKji5mtuWSB7Xbvnq4kWDeDpLGjj/view?usp=sharing) 

## Trained Model
* Link to model 
 * https://drive.google.com/file/d/1gRgRUPW7TaYpF2wXa5eTRINbXx3vCs9n/view?usp=sharing

## Image Classification Screenshots
![Example screenshot](./img/screenshot.png)
isto kako i tie pogornite :)
Toni

## Video Classification
![image](https://github.com/FilipAngelov/Mask_and_Age_Classification/blob/master/other/gif-petar.gif)

## Code Examples
Show examples of usage:
`put-your-code-here`
Filip

## Features
List of features ready and ToDos for future development
* Image classification function 'predict_url' which can be used to classify a picture by inserting a picture URL.
  * Example: predict_url('https://i.pinimg.com/originals/db/00/0e/db000e66cc61d4f15a6c2b04916bfc9c.jpg')
* Video classification function which runs the web camera on you machine, locates a face on the video, and classifies between the four classes.

To-do list:
* Out of sample validation showed that classification errors occur mostly in the old with mask class which usually gets classified as young with a mask. We identified two potential solutions to solve the problem:
  * Collecting more data could potentially improve the model's accuracy. 
  * Create two classifiers instead of currently using only one. The first classifier will classify between with_mask and without_mask, and the second one will classify between old and young.


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
