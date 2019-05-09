# LR Finder
`Learning rate` is a very important hyperparameter for `gradient` based optimization algorithms like `SGD` and variants for 
training deep neural networks successfully.  Set the learning too low and the training time becomes huge as the parameters update very slowly. Set it too high and the updates will skip over optimal solutions, or worse the optimizer might not converge at all!

**Leslie Smith** from the `U.S. Naval Research Laboratory`, presented two papers for addressing this problem. The first paper was [`Cyclic Learning Rates`](https://arxiv.org/abs/1506.01186) and the second paper was [`Super Convergence`](https://arxiv.org/abs/1708.07120). Here we will be focusin on the first paper. The second one is just an iterative improvement with the same idea applied to multiplt hyperparams. 
