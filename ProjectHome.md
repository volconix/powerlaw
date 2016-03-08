# This project has moved to Github #
Go [to Github](https://github.com/jeffalstott/powerlaw).

## powerlaw: A Python Package for Analysis of Heavy-Tailed Distributions ##


`powerlaw` is a toolbox using the statistical methods developed in
[Clauset et al. 2007](http://arxiv.org/abs/0706.1062) and [Klaus et al. 2011](http://www.plosone.org/article/info%3Adoi%2F10.1371%2Fjournal.pone.0019779) to determine if a probability distribution fits a power law. Academics, please cite as:

Jeff Alstott, Ed Bullmore, Dietmar Plenz. (2014). powerlaw: a Python package
for analysis of heavy-tailed distributions. [PLoS ONE 9(1): e85777](http://www.plosone.org/article/info%3Adoi%2F10.1371%2Fjournal.pone.0085777)

Also available at [arXiv:1305.0215 [physics.data-an](http://arxiv.org/abs/1305.0215)]

### Basic Usage ###

For the simplest, typical use cases, this tells you everything you need to
know.

```
    import powerlaw
    data = array([1.7, 3.2 ...]) # data can be list or numpy array
    results = powerlaw.Fit(data)
    print results.power_law.alpha
    print results.power_law.xmin
    R, p = results.distribution_compare('power_law', 'lognormal')
```

For more explanation, understanding, and figures, see the paper,
which illustrates all of powerlaw's features. For details of the math,
see Clauset et al. 2007, which developed these methods.

### Quick Links ###

[Installation](http://code.google.com/p/powerlaw/wiki/Installation)

[Paper illustrating all of powerlaw's features, with figures](http://arxiv.org/abs/1305.0215)

[Code examples from manuscript, as an IPython Notebook](http://nbviewer.ipython.org/github/jeffalstott/powerlaw/blob/master/manuscript/Manuscript_Code.ipynb)

[Documentation](http://pythonhosted.org/powerlaw/)

[Known Issues](https://code.google.com/p/powerlaw/wiki/KnownIssues)

[Update Notifications, Mailing List, and Contacts](http://code.google.com/p/powerlaw/wiki/Interact)

This code was developed and tested for Python 2.x with the
[Enthought Python Distribution](http://www.enthought.com/products/epd.php),  and later amended to be
compatible with 3.x. The full version of Enthought is
[available for free for academic use](http://www.enthought.com/products/edudownload.php).

===Acknowledgements=11

Many thanks to Andreas Klaus, Mika Rubinov and Shan Yu for helpful
discussions. Thanks also to [Andreas Klaus](http://neuroscience.nih.gov/Fellows/Fellow.asp?People_ID=2709),
[Aaron Clauset, Cosma Shalizi,](http://tuvalu.santafe.edu/~aaronc/powerlaws/)
and [Adam Ginsburg](http://code.google.com/p/agpy/wiki/PowerLaw) for making
their code available. Their implementations were a critical starting point for
making `powerlaw`.