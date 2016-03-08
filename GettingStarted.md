`powerlaw` has streamlined tools for quickly calculating all the relevant statistics, with both function-based and class-based methods available. The basics, however, require just a few lines of code:

```
import powerlaw
data = array([1.7, 3.2 ...]) #data can be list or Numpy array
results = powerlaw.Fit(data)
print results.power_law.alpha
print results.power_law.xmin
R, p = results.distribution_compare('power_law', 'lognormal')
```

For the simplest, typical use cases, that tells you everything you need to know. See this [working paper illustrating all of powerlaw's features, with figures](https://powerlaw.googlecode.com/files/powerlaw.pdf) for more explanation and understanding. For details of the math, see [Clauset et al. 2007](http://arxiv.org/abs/0706.1062), which developed these methods.