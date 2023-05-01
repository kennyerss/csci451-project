TODO Tasks

Algorithm
* Everyone should read the papers https://www.thelancet.com/journals/landig/article/PIIS2589-7500(22)00063-2/fulltext
* * What kind of loss function?
* Plot things that could distinguish - number of images/revisits by race, number of lateral/non-lateral images, age by race, gender in each race, etc., anything that could identify patients
* Modify Dataset function so it will not run into issues when patient has no image or only has lateral image, etc
* Review class notes from week 9 and 10, implement some algorithm from these - either Logistic Regression or basic Convolution Neural Network
* Implement ResNet https://blog.paperspace.com/writing-resnet-from-scratch-in-pytorch/ or https://www.run.ai/guides/deep-learning-for-computer-vision/pytorch-resnet OR find other algorithm we can implement
* Use pretrained EfficientNet and maybe do a self-implementation
* Do optimization of parameters - for now optimize learning rate, try learning rate schedules (which will change learning rate over time)
* Try doing image augmentation - random horizontal flips, random rotations (because some patients might be standing upright at slightly different angles), blurs/zooms
* Analysis wise, could be interesting to do intersectional bias - black women, etc.

Ethics
* Find papers - would be helpful after each paper to put small summary on what paper is about, major findings

Finished
* Implemented DataLoader
* Most of data in shared drive - AND check that data is actually loaded
* By the paper, "White" is anything containing label White - "White", "White, non-Hispanic", "White Hispanic"
* Decided to do lateral and frontal image scans
* Implemented ResNet34 via own implementation
* Made df_patients_race that have patient image link, patient id, patient race, patient race num (based on White, Black, Asian, Other)
