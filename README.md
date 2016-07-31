# SGCRFpy: Sparse Gaussian Conditional Random Fields in Python

A Gaussian CRF models conditional probability density of y given x as

![equation](http://latex.codecogs.com/svg.latex?p(y|x\\Lambda\\Theta) = \\frac{e^{-y^\\top \\Lambda y -2 x^\\top \\Theta y}}{Z(x)})

where Z(x) = c * |Λ|^-1 * exp(x' * Θ * Λ^-1 * Θ' * x)

This is equivalent to:

![equation](http://latex.codecogs.com/svg.latex?p(y|x)\\sim\\mathcal{N}(\\Theta \\Lambda^{-1}x,\\Lambda^{-1}))

![alt tag](https://github.com/dswah/sgcrfpy/blob/master/images/scgrf_random_graph.png)
