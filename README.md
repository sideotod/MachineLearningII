# MachineLearningII
## Training Algorithm in SVM
```markdown
Training Algorithm (minibatch of size m; learning rate α)
initialize all parameters W, b
repeat
    pick a minibatch Xm from X
    forward: compute all activations A
    compute cost J = 1/m Σ L(Ŷ(i), Y(i))
    backward: compute all gradients
    update parameters:
        W[l] <- W[l] - αdW[l]
        b[l] <- b[l] - αdb[l]
until it is time to stop (validation loss has converged)
return final parameters W*, b*
```