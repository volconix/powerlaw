Presently none! Please submit any issues or patches to Github.


Fixed Issues:

_Truncated power law fitting of a discrete distribution takes too long. For anything other than the smallest of datasets, fitting can take hours. This is only during **fitting**, not subsequent calculations, and is because of the calculation of the incomplete gamma functions (presently implemented with mpmath's gammainc). Open to suggestions on how to improve this._