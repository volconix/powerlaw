`powerlaw` is hosted on [PyPI](http://pypi.python.org/pypi/powerlaw), so installation is straightforward. The easiest way to install type this at the command line (Linux, Mac, or Windows):

```
easy_install powerlaw
```

or, better yet:

```
pip install powerlaw
```

easy\_install or pip just need to be on your PATH, which for Linux or Mac is probably the case.  [Here](http://pypi.python.org/pypi/powerlaw) is the Windows installer on PyPI (untested).

`pip` should install all dependencies automagically. These other dependencies are `numpy`, `scipy`, and `matplotlib`. These are all present in Enthought. To fit truncated power laws or gamma distributions, `mpmath` is also required, which is not in Enthought and is installable with:

```
pip install mpmath
```

This last requirement will change if/when Scipy's `gamma`, `gammainc` and `gammaincc` functions have numerical accuracy for negative numbers.

You can also build from source from the code here on Google Code or on [github](https://github.com/jeffalstott/powerlaw), though it may be a development version slightly ahead of the PyPI version.