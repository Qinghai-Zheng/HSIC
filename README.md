# Hilbert-Schmidt independence Criterion (HSIC)

Python version of the original MATLAB code of [Hilbert-Schmidt independence Criterion](http://papers.nips.cc/paper/3201-a-kernel-statistical-test-of-independence.pdf) (HSIC).

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites
* NumPy
* SciPy

We test the code using **Anaconda 4.3.0 64-bit for python 2.7** on windows. Any later version should still work perfectly.

## Apply on your data

### Usage

Import IGCI using

```
from HSIC import hsic_gam
```

Apply IGCI on your data
```
testStat, thresh = hsic_gam(x, y, alph = 0.05)
```
**If testStat < thresh, x and y are independent;
If testStat > thresh, x and y are not independent.**

### Notes

Input of function **hsic_gam()**

| Argument  | Description  |
|---|---|
|x | Data of the first variable. L by dim_x numpy array.|
|y | Data of the second variable. L by dim_y numpy array.|
|alph | lebel of the test |

Output:Output of function **igci()**

| Argument  | Description  |
|---|---|
|testStat  |test threshold for level alpha test|
|thresh| test statistic|


## Authors

* **Shoubo Hu** - shoubo.sub@gmail.com

See also the list of [contributors](https://github.com/amber0309/HSIC/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
