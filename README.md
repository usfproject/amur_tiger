# Amur Tiger Reidentification

### **Dataset Download**

Dataset was downloaded from [cvwc2019challenge.](https://cvwc2019.github.io/challenge.html)

### **Dataset Preparation to run:**

Run below command to preprocess the data. The following preprocessing function, flips the images and keypoints and saves the results to image folder, csv and json files. And then extracts the parts for 
all the images and stores in the designated parts folder. Finally it creates 4-folds of the dataset.

> python preprocessing.py

All the paths to save and retrieve the files can be changed in **config.ini** file

### **Run the training script on gaivi**

We submitted our training jobs on gaivi server. Bash script is available in **trainer.sh**
Submit the job by running below command:

> #sbatch trainer.sh

### **Evaluate the model**

Run the below command to evaluate the model

> python evaluation_script.py
