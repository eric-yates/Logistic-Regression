# Logistic-Regression
Contains an object-oriented model for logistic regression made from scratch using mathematical theory.

This model has not been optimized and is intended for educational purposes rather than maximum performance.

## Getting Started

These instructions will get a copy of the project up and running on your local machine.


### Prerequisites

Instructions for installing these software are listed in the next section: Installing. These are the software packages needed to run:

* Python **2.7**

These Python packages are also needed:

* numpy
* matplotlib
* pandas


### Installing

If your computer does not already have Python **2.7** installed, download it [here](https://www.python.org/downloads/).

By default, Python should come with pip (a package manager). Use it to install the following dependencies by opening the Terminal/command line and entering the commands as follows, each line as a separate command:

```
pip install numpy
pip install matplotlib
pip install pandas
```

## Usage

For all models, it is assumed that the model receives well-prepared and
cleaned input data X and targets T. Any feature engineering should be
done prior to creating a model.

### Basic

1) Clone/fork this repository
2) Open and run the 'example.py' file

### Advanced

1) Create a new Python script
2) Save it in the cloned/forked folder
2) Use a format similar to the following:
```     
from logistic_regression import LogisticRegression

X = ...   # input data
T = ...   # target data

model = LinearRegression(X=X,
                         T=T,
                         epochs=1000,
                         learn_rate=0.001,
                         reg_L1=0, # Lasso regularization coefficient
                         reg_L2=0) # Ridge regularization coefficient

for i in xrange(model.epochs):
            
    model.make_predictions()
    model.check_accuracy()
    model.cross_entropy()
    model.update_weights()
    
    if i % 100 == 0:
        print "Iteration: " + str(i) + " Error: ", model.errors[i]
        print "Accuracy:", model.accuracies[i]

model.plot_errors()
```

## Built With

* [Python](https://www.python.org/about/) - A programming language used here to create exploratory data graphs
* [Numpy](http://www.numpy.org/) - Python library for mathematical and matrix operations 
* [Matplotlib](https://matplotlib.org/) - Python library for graphing data
* [Pandas](https://pandas.pydata.org/pandas-docs/stable/) - Python library for data manipulation


## Authors

* **Eric Yates** - [Github Profile](https://github.com/eric-yates)

## License

This project is licensed under the MIT License - see the [LICENSE.md](/LICENSE.md) file for details.

## Acknowledgments

* **LazyProgrammer**: For his [courses](https://www.udemy.com/user/lazy-programmer/) on machine learning

