# Project: Mask and Age Classification 
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
With the rapid spread of COVID-19 we find ourselves plunged into a global health crisis where face masks are essential tool to limit the virus spread. As we already know, older people are less immune on this virus and it is crucial that more people should be wearing a face mask. Therefore, we have decided to create a model which will recognize those who are helping the public safety and those who don't, separating them in four groups:

* Old with Mask 
* Young with Mask
* Old without Mask
* Young without Mask

After trying several different pretrained models we found the one that gave the best results:heavy_check_mark:. <br/>
Scroll down :arrow_down: to see our model summary, screenshots of the predictions, video classification example :camera: and more details!

## Technologies & Setup
**Technologies**
* We used Keras for model architecture, training, and prediction.
* Model training was done in Google Colab.
* Video classification should be done on local machine and we used Spyder.

**Setup**
* There is no need to install any of the libraries used in the notebook if you use Colab as they are preinstalled for you. 
* When performing video classification on your local machine please refer to the Requirements.txt file in the main repository.  
* You would need to import all the libraries used in the notebook. All the libraries used are listed in the Project.ipynb file.


## Dataset
* Sometimes it could be quite difficult to find the correct dataset for launching a Machine Leaning project, especially when you have to use lots of faces. For that reason, we created our own dataset by generating synthetic faces using GAN, asking our friends for their permission for using their photos, as well as downloading images from free repositories available on the Internet. 
* Additionally, during the process of generating our dataset we implemented a simple [method :link:](https://github.com/FilipAngelov/Mask_and_Age_Classification/tree/master/code_mask_on_face) to augment a mask on a person's face. The result of a particular image pre and post augmentation is as follows:
![image](https://github.com/FilipAngelov/Mask_and_Age_Classification/blob/master/other/face_augmentation.png)

* Below is a summary of our [dataset :link:](https://drive.google.com/file/d/14RjXeKji5mtuWSB7Xbvnq4kWDeDpLGjj/view?usp=sharing)
<table>
<tr><th> Splitting between groups </th><th> Summary </th></tr>
<tr><td>

| No.  | Group name  | Number of files |
| ------------- | ------------- | ------------- |
|1 | old_with_mask  | 381 |
|2| old_without_mask |  355 |
|3| young_with_mask  | 346  |
|4| young_without_mask  | 369 |

</td><td>

|Train|Validation|Test| 
|--|:--:|--|
|1044|261|146|
</td></tr> </table>


* Dataset example pictures  

![image](https://github.com/FilipAngelov/Mask_and_Age_Classification/blob/master/other/download.png)

## Trained Model
* [:link: Clik here for our BEST model](https://drive.google.com/file/d/1gRgRUPW7TaYpF2wXa5eTRINbXx3vCs9n/view?usp=sharing)
 ![image](https://github.com/FilipAngelov/Mask_and_Age_Classification/blob/master/other/model_summaries.png)

## Image Classification Screenshots
![image](https://github.com/FilipAngelov/Mask_and_Age_Classification/blob/master/other/Presentation1.png)

## Video Classification
![image](https://github.com/FilipAngelov/Mask_and_Age_Classification/blob/master/other/gif-petar.gif)

## Code Examples
Show examples of usage:
`put-your-code-here`
Filip

## Features
List of features ready and ToDos for future development
* Image classification function ['predict_url' :link:](https://github.com/FilipAngelov/Mask_and_Age_Classification/blob/master/predict_url.ipynb) which can be used to classify a picture by inserting a picture URL from the internet.
  * Example: predict_url('https://i.pinimg.com/originals/db/00/0e/db000e66cc61d4f15a6c2b04916bfc9c.jpg')
* Video classification function which runs the web camera on you machine, locates a face on the video, and classifies between the four classes.

**To-do list:** :clipboard:
* Out of sample validation showed that classification errors occur mostly in the old with mask class which usually gets classified as young with a mask. We identified **two potential solutions to solve the problem**:<br/>
   :small_orange_diamond:Collecting more data could potentially improve the model's accuracy.<br/>
   :small_orange_diamond:Create two classifiers instead of currently using only one. The first classifier will classify between with_mask and without_mask, and the second one will classify between old and young.<br/>
:bulb: **Another** improvement to the overall model could be adding granularity to the age classification. Instead of binary classification between young and old we propose multiclass classification with the following classes as an example:

|**Age groups**  | 0-2 | 4-6 | 8-12|15-20|25-32|38-43|48-53|60-100|
| :------ | :-------- | :-------- | :------ | :------ | :------ | :------ | :------ | :------ |


## Inspiration
Add here credits. Project inspired by..., based on...
SRNA

## Contributors

Thanks to the following people who have contributed to this project: :raised_hands:

* [@FilipAngelov](https://github.com/FilipAngelov) 
* [@jolakoskip](https://github.com/jolakoskip) 
* [@gardnerska](https://github.com/gardnerska) 
* [@srnag](https://github.com/srnag)
* [@tonipesic](https://github.com/tonipesic)
