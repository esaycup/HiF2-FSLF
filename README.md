# HiF2-FSLF
Pytorch = 2.4.0 

Python = 3.12.4

## dataset
1. target domain data set:

Taking Trento as an example, use the left half of the Trento image as the target domain dataset, and move the files to `./datasets` folder.

2. source domain data set:
   
Use the right half of the Trento image as the source domain dataset, and move the files to `./datasets` folder.

An example dataset folder has the following structure:
```
datasets
├── imdb_128.pickle
├── Trento
│   ├── hsi-right.mat
│   ├── hsi-left.mat
│   ├── lidar-right.mat
│   ├── lidar-left.mat
│   ├── gt-right.mat
|   ├── gt-left.mat

```

## Usage:
Take HiF2-FSLF method on the Trento dataset as an example: 
1. Download the required data set and move to folder`./datasets`.
2. If you down the source domain data set (Trwnto-RightPart) in mat format,you need to run the script `imdb_128.py` to generate preprocessed source domain data. 
3. Taking 5 labeled samples per class as an example, run `main-Trento.py`. 

