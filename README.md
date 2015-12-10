# python-steenzout
`steenzout` namespace package.

Namespace packages and regular packages are very similar.
The differences are:

Portions of namespace packages need not all come from the same directory structure, or even from the same loader.
Regular packages are self-contained: all parts live in the same directory hierarchy.

* namespace packages have no __file__ attribute.
* namespace packages' __path__ attribute is a read-only iterable of strings,
  which is automatically updated when the parent path is modified.
* namespace packages have no __init__.py module.
* namespace packages have a different type of object for their __loader__ attribute.

Taken from [Differences between namespace packages and regular packages](https://www.python.org/dev/peps/pep-0420/#differences-between-namespace-packages-and-regular-packages).
