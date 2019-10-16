# Community Software Analysis Proposal

## Software: *NumPy*

NumPy is a matrix/array library for Python that allows for efficient representation of and computation with N-dimensional arrays.  Matrix/array operations in NumPy are implemented by calling into C (and BLAS for linear algebra) which allows NumPy to achieve high levels of performance in what is typically regarded as a slow language.  NumPy's audience is mainly scientists and engineers who would otherwise be using proprietary software such as MATLAB for both element-wise computations and linear algebra.  In my job as a tool developer for satellite data processing I use NumPy almost daily for it's element-wise processing speed.


### Stats

| Description | Your answer |
|---------|-----------|
| Repository URL | [https://github.com/numpy/numpy](https://github.com/numpy/numpy) (is the main repository)  |
| Main/documentation website | [https://docs.scipy.org/doc/numpy/index.html](https://docs.scipy.org/doc/numpy/index.html) |
| Year project was started | 2006 (but has roots in Numeric from 1995) |
| Number of contributors in the past year | 222 |
| Number of contributors in the lifetime of the project | 1023 (version history goes back to 2001-12-21)  |
| Number of distinct affiliations | >20 |
| Where do development discussions take place? | GitHub issues and a [mailing list](http://numpy-discussion.10968.n7.nabble.com/) |
| Typical number of emails/comments per week? | ~90 (issues/pull requests per week) |
| Typical number of commits per week? | 48 (average of last 32 weeks) |
| Typical commit size | average of 161 lines per commit (3 files changed) |
| How does the project accept contributions? | pull requests  |
| Does the project have an automated test suite? | yes |
| Does the project use continuous integration? | yes (Travis CI) |
| Are any legal/licensing steps required to contribute? | no |

### Install and run

Check the following boxes when complete or add a note below if you
encountered a problem.

- [x] I have installed the software
- [x] I have run at least one example
- [x] I have run the test suite
- [x] The test suite passes

### Notes/concerns/risks

There are a few open issues at the moment at which I could contribute.  One in particular is that the `log2` function does not properly make use of the AVX as it could.  My only concern is that NumPy mainly uses the Python/C API which I don't have any experience with (despite being both a C/C++ and Python developer).