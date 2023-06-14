## The MegNIST Dataset

The dataset can be downloaded directly as a Python `dict` serialised using `pickle` [here](https://drive.google.com/file/d/1doqjgglgDWIBcy2BUsbwyitDsBc0cqY7/view?usp=sharing) (6.84 GB). 

The pickle file can be loaded in the usual way:
```python
import pickle

with open('megnist.pickle', 'rb') as f:
    megnist = pickle.load(f)
```

The dictionary `megnist` has the following keys: `X_train`, `y_train`, `X_val`, `y_val`, `X_test`, `y_test`. For example, `megnist['X_train']` is a 3-dimensional numpy array of floats with shape (10,000 examples, 306 channels, 250 time steps). `megnist['y_train']` is a 1-dimensional numpy array of integers (0, ..., 9) with 10,000 examples.

A dimensionality reduced version of the dataset (64 channels) can be downloaded [here](https://drive.google.com/file/d/1J1Fnd1ie5L9ffpRN5os_1vBxzJ3L6PCx/view?usp=sharing) (1.43 GB). 
