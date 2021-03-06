# Support Vector Machine
A practice of linear/polynomial/gaussian SVM.

## How to run

Start the program
```
python LinearSVM.py TrainData TestData
```
```
python PolynomialSVM.py TrainData TestData
```
```
python GaussianSVM.py TrainData TestData
```
```
python GaussianSVMwithValidation.py TrainData TestData
```

## Description

### Data set

The Data set are download from the processed
US Postal Service Zip Code data set with extracted features of intensity and symmetry for training and testing.


The format of each row is:
```
digit intensity symmetry
```

### LinearSVM.py

Run linear SVM on the data set for the binary classification problem "2" versus "not 2". Then plot ||w|| versus log<sub>10</sub>C

### PolynomialSVM.py

Run polynomial SVM with the kernel K(x<sub>n</sub>, x<sub>m</sub>) = (1 + x<sub>n</sub><sup>T</sup>x<sub>m</sub>)<sup>2</sup> on the data set for the binary classification problem "4" versus "not 4". Then plot E<sub>in</sub> versus log<sub>10</sub>C.

### GaussianSVM.py

Run Gaussian SVM with &#947; = 80 on the data set for the binary classification problem "0" versus "not 0". Then plot the margin versus log<sub>10</sub>C.

### GaussianSVMwithValidation.py

Run Gaussian SVM with a validation proccess that randomly samples 1000 examples from the training set for validation and leave the other examples for training. C is fixed at 0.1, and use the validation proccess to choose the best &#947; from {0.01, 0.1, 1, 10, 100}. Then plot a histogram for the number of times each &#947; is choosed.

## Built With

* Python 3.6.0 :: Anaconda custom (64-bit)

## Authors

* **SaKaTetsu** - *Initial work* - [SaKaTetsu](https://github.com/SaKaTetsu)