# Yolo_FCNN_dev_pengos
Developing Computer Vision for counting penguins in Antarctica

This marks the beginning of the development of methods for counting Chinstrap, Adelie and Gentoo penguin colony sizes along the WAP and Scotia Sea (South Orkney Islands). Ultimate goal is to roll some of these models out into CCAMLR as part of the enhanced CEMP monitoring program and for the trial of the new Krill Fishery Management Approach (KFMA). 

The two Faster RCNN (train and test) are deveoped in Jupyterlab notebooks on a macbook pro 2017 model.  The YOLOv8 script was created in Google Colab on the same laptop. 

Both rely on annotated , versioned data (test and train) from Roboflow and utilise the roboflow-provided download scripts (choose Yolo8 formats for each model).

The "raw" (pre-annotated) data are available open source from the Australian Antarctic Division: 

https://data.aad.gov.au/metadata/PENGUIN_DET_VAPCOL

There are additional files here - "Roldan_train" and "Roldan_test".  These are Faster RCNN modified to work with ringed seal annotated datasets for Alberto Roldans Masters thesis in Roboflow.  The "training" file needs modifying such that the polygon labels used in Roboflow are converted to box labels, and used for training. 

Further - the model is not trained with distractors, only positive labelled objects.  Future iterations of the Roldan_train should include significant distrators.  For this, the code needs altering to include the treatment of training images with no labels. 

The "test" model relies on the trained model being saved to google drive, then recalled back into a fresh Colab session. 

