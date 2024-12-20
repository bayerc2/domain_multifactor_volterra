# State spaces of multifactor approximations of nonnegative Volterra processes

We provide code for the numerical example of the above paper.

## Background

We consider stochastic Volterra equations of the form
$$Y_t = Y_0 + \int_0^t K(t-s) b(Y_s) d s + \int_0^t K(t-s) \sigma(Y_s) d W_s$$,
where we assume that the solution remains non-negative - allowing $\sigma(x) = \sqrt{x}$, for instance.
For many important examples of the kernel $K$, e.g., the fractional kernel $K(r) \simeq r^{H-1/2}$,
the corresponding Volterra process $Y$ poses both theoretical and numerical challenges.
It is sometimes advantageous to replace $K$ by an approximation consisting of sums of exponentials, 
i.e., $\widehat{K}(r) = \sum_{i=1}^N w_i \mathrm{e}^{-x_i r}$.
Indeed, the solution $\widehat{Y}$ of the stochastic Volterra equation obtained by replacing $K$ with
$\widehat{K}$ can be represented by $\widehat{Y}_t = \sum_{i=1}^N w_i Y^{(i)}_t$, for an (explicitly given)
$N$-dimensional diffusion process $\mathbf{Y}_t := (Y^{(i)}_t)_{i=1}^N$.

In the paper (link to be added), we address the question about the natural state space of the process $\mathbf{Y}_t$.
Clearly, non-negativity of $\widehat{Y}_t$ implies that $\mathbf{Y}_t$ lies in a half-space contained in $\mathbb{R}^N$.
However, it turns out that the actual state space is, in fact, a cone contained in that halfspace.

## The numerical example
