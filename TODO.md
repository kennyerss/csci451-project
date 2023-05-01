TODO Tasks

Algorithm
* Everyone should read the papers https://www.thelancet.com/journals/landig/article/PIIS2589-7500(22)00063-2/fulltext
* * In particular - what kind of models do they use? Seems Resnet or EfficientNetB4
* * What kind of logistic loss (I think AUC)
* Plot things that could distinguish - number of images/revisits by race, number of lateral/non-lateral images, age by race, gender in each race, etc., anything that could identify patients
* Reconfigure the chexpert DEMO csv and the train.csv so each patient id can be linked to their race - we may need to get rid of some data, namely the patients whose race is "Other", etc.
* Decide whether to do lateral or frontal scans only or do all scans
* Modify Dataset function so it will not run into issues when patient has no image or only has lateral image, etc
* Review class notes from week 9 and 10, implement some algorithm from these - either Logistic Regression or basic Convolution Neural Network
* Implement ResNet https://blog.paperspace.com/writing-resnet-from-scratch-in-pytorch/ or https://www.run.ai/guides/deep-learning-for-computer-vision/pytorch-resnet OR find other algorithm we can implement
* Analysis wise, could be interesting to do intersectional bias - black women, etc.

Ethics
* Find papers - would be helpful after each paper to put small summary on what paper is about, major findings

Finished
* Implemented DataLoader
* Most of data in shared drive
* By the paper, "White" is anything containing label White - "White", "White, non-Hispanic", "White Hispanic"
