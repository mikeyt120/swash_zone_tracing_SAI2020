# Swash Zone Tracing SAI2020
This is a competition for UQ's summer of AI, use my code as a starting point and see if you can improve the performance! Your task is to trace the swash front (where the water meets the shore) in timestacks automatically.

**Computer requirements:**
  * You need to have anaconda
  * A GPU will be helpful but not necessary to start acheiving satisfactory results

**Files you need to download:**
  * Github:
    * Timestack_Swash_Front_Tracing_SAI2020.ipynb (uploads the images, trains the model and evaluates performance on a validation set)
    * MThompson_best.model (my best tensorflow model, you can visualize the results with the above script)
    
  * Cloudstor:
    * /labelled_timestacks (labelled training dataset - about 31,000 snapshots of timestacks with shoreline position labelled with a value between 0 and 1)
    * /test_timestacks (evaluation dataset - labelled data from 6 different beaches used for evaluating the performance of you model)
    
Put all the above files into a folder accesible by anaconda distribution. Open up "Timestack_Swash_Front_Tracing_SAI2020.ipynb" and run each code cell to train and evaluate a lightweight model. The model will be evaluated against some **seen** labelled timestacks. Experiment with different hyperparameters and deeper networks to try and beat the performance of my best model, "MThompson_best.model".

When the competition finishes, I will test your submitted model against the **seen** labelled timestacks and some **unseen** labelled timestacks which have data from some of the same beaches but also from some very different beaches. Therefore your model's ability to generalise will be put to the test! **The model with the best averaged MSE from the seen timestacks and unseen timestacks will win. If you win and your averaged MSE is less than 0.0003, then if you are keen to write a page or two about your implementation you will be a co-author to a planned journal paper with myself and a few coastal engineering researchers.**

To submit your .model file, upload it to this github repository in the following format:
  * firstnameLastname_imgSize_[insert your square image size number in pixels].model 
    
**Code Structure:**

![alt text](https://github.com/mikeyt120/swash_zone_tracing_SAI2020/blob/main/code_architecture.PNG?raw=true)

You will be working on just the convolutional neural network part of the diagram.

**Acknowledgements:**
*Prof. Tom Baldock - supervisor of the coastal aspects of this project
*Assoc. Prof. Marcus Gallagher - supervisor of the ML aspects of this project
*Dr. Hannah Power - provider of many of the timestacks
*Dr. Caio Stringari - provider of many of the timestacks
