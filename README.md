# Swash Zone Tracing SAI2020
Trace the swash front in timestacks automatically. This is a competition for UQ's summer of AI, use my code as a starting point and see if you can improve the performance!

**Computer requirements:**
  * You need to have anaconda
  * A GPU will be helpful but not necessary to start acheiving satisfactory results

**Files you need to download:**
  * Github:
    * (uploads the images, trains the model and evaluates performance on a validation set)
    * (my best tensorflow model. The above script will compare this with the manually picked points and your model's points for each timestack)
    
  * Cloudstor:
    * (labelled training dataset - about 31,000 snapshots of timestacks with shoreline position labelled with a value between 0 and 1)
    * (evaluation dataset - labelled data from 6 different beaches used for evaluating the performance of you model)
    
When the competition finishes, I will test your submitted model against a different dataset which has data from some of the same beaches but also from some very different beaches. Therefore your model's ability to generalise will be put to the test!

To submit your .model file, upload it to this github repository in the following format:
  * firstnameLastname_imgSize_[insert your square image size number in pixels].model 
    
**Code Structure:**

![alt text](https://github.com/mikeyt120/swash_zone_tracing_SAI2020/blob/main/code_architecture.PNG?raw=true)

You will be working on just the convolutional neural network part of the diagram.
