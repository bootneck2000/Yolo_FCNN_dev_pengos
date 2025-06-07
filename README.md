# Yolo_FCNN_dev_pengos
Developing Computer Vision for counting penguins in Antarctica

This marks the beginning of the development of methods for counting Chinstrap, Adelie and Gentoo penguin colony sizes along the WAP and Scotia Sea (South Orkney Islands). Ultimate goal is to roll some of these models out into CCAMLR as part of the enhanced CEMP monitoring program and for the trial of the new Krill Fishery Management Approach (KFMA). 

The two Faster RCNN (train and test) are deveoped in Jupyterlab notebooks on a macbook pro 2017 model.  The YOLOv8 script was created in Google Colab on the same laptop. 

Both rely on annotated , versioned data (test and train) from Roboflow and utilise the roboflow-provided download scripts (choose Yolo8 formats for each model).
