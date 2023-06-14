## The MegNIST Dataset

The dataset can be downloaded directly as a Python `dict` serialised using `pickle` [here](https://drive.google.com/file/d/1doqjgglgDWIBcy2BUsbwyitDsBc0cqY7/view?usp=sharing) (6.84 GB). 

The pickle file can be loaded in the usual way:
```python
import pickle

with open('megnist.pickle', 'rb') as f:
    megnist = pickle.load(f)
```

The dictionary `megnist` has the following keys: `X_train`, `y_train`, `X_val`, `y_val`, `X_test`, `y_test`. 

`megnist['X_train']` is a 3-dimensional numpy array of floats with shape (10,000 examples, 306 channels, 250 time steps). `megnist['y_train']` is a 1-dimensional numpy array of integers (0, ..., 9) with 10,000 examples.

The validation and test splits have the same dimensions, except for the number of examples (1,000 instead of 10,000).

Dimensionality reduced versions of the dataset can be downloaded below:

* [16 channels](https://drive.google.com/file/d/1JEzD9GOSDNaHfHbHzcuJdQksBss4h2Rk/view?usp=sharing) (366.3 MB). 
* [32 channels](https://drive.google.com/file/d/1VkemXsFP0oxde-2Dbqo60Qs-_e3VYgJy/view?usp=sharing) (732.5 MB). 
* [64 channels](https://drive.google.com/file/d/1J1Fnd1ie5L9ffpRN5os_1vBxzJ3L6PCx/view?usp=sharing) (1.43 GB). 
* [128 channels](https://drive.google.com/file/d/1sixVpkDhlagEdwVuW9a3VaXD6npoBJwQ/view?usp=sharing) (2.86 GB). 
