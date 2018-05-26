

### Gaussian basis functions[](https://pythondatasciencehandbook-vikas-g.notebooks.azure.com/nb/notebooks/notebooks/05.06-Linear-Regression.ipynb#Gaussian-basis-functions)

Of course, other basis functions are possible. For example, one useful pattern is to fit a model that is not a sum of polynomial bases, but a sum of Gaussian bases. The result might look something like the following figure:

![](https://pythondatasciencehandbook-vikas-g.notebooks.azure.com/nb/notebooks/notebooks/figures/05.06-gaussian-basis.png)[figure source in Appendix](https://pythondatasciencehandbook-vikas-g.notebooks.azure.com/nb/notebooks/notebooks/05.06-Linear-Regression.ipynb#Gaussian-Basis)

The shaded regions in the plot are the scaled basis functions, and when added together they reproduce the smooth curve through the data. These Gaussian basis functions are not built into Scikit-Learn, but we can write a custom transformer that will create them, as shown here and illustrated in the following figure (Scikit-Learn transformers are implemented as Python classes; reading Scikit-Learn's source is a good way to see how they can be created):
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTI4NTg5ODk3MiwxODYwNjEwNjc0XX0=
-->