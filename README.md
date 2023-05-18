# baesyan-opt-test
Implementation of Bayesian Optimization to find the optimal learning rate of a deep neural network (CV)
* Please look at _bo.ipynb

## Brief description
* Here I have implemented two solutions 
  + "optimizer out of the box" (https://github.com/bayesian-optimization)
  + "optimizer from scratch"
* The code, results and figures are presented in the corresponding sections.
* Note that the presented solution is only a simple but working solution, it does not provide `the best optimal learning rate`, since it uses one learning epoch for the ResNet model.

## Full task description
Objective: Find the optimal learning rate of a deep neural network for CV
Optimizer: 
* Implement Bayesian Optimization (BO) as a global optimization approach
 + use a Gaussian Process as a predictive model (you can use any existing GP library)
 + implement expected improvement (EI) as an acquisition function
 + use an optimization budget of 10 function evaluations

* For the deep neural network, please follow the specifications below:
 + A rather small ResNet (details can be chosen by you, but you should implement it on your own)
 + Optimizer: SGD 
 + Deep learning framework: PyTorch or JAX
 + Dataset: Fashion-MNIST

* Plotting:
 + Starting with the second iteration of Bayesian Optimization, plot all observations, the posterior mean, the uncertainty estimate, and the acquisition function after each iteration.
 + See here for an exemplary plot (on a different task): https://towardsdatascience.com/shallow-understanding-on-bayesian-optimization-324b6c1f7083

* Programming language: Python; minimal coding standards:
 + PEP8 
 + Doc-Strings
 + README with instructions how to run it
