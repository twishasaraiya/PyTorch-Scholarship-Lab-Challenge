# PyTorch-Scholarship-Lab-Challenge

## INDEX
 - [Load Data](load-data)
 - [Visualize](visualize-batch-of-images)
 - [Training](train-model)
 - [Testing](test-model)
 
### LOAD DATA
Download the [dataset](http://www.robots.ox.ac.uk/~vgg/data/flowers/102/index.html) and upload it to google drive. Mount the drive in your colab environment and access the data by specifying the path in `data_dir` variable. However this is not required while working on local machine
### VISUALIZE A BATCH OF IMAGES
The training set is divided into random batches of size 16(hyperparamater) and one batch of data can be visualized using `imshow()` function
### TRAIN MODEL
Training can be done in 2 environment
1. Google Colabratory(which I have used)
2. Local Machine(if GPU is avialable)

### Defing Model Architecture
Here I have used `resnet152` as pretrained model and modified the last fully connected layer to single Linear layer to get 102 output units. 

### TEST MODEL
The test data can be downloaded as follows
```
!wget -O flower_data_orginal_test.zip "https://www.dropbox.com/s/da6ye9genbsdzbq/flower_data_original_test.zip?dl=1"
!unzip flower_data_orginal_test.zip
```
