# Meta-Learning

Large, diverse data lead to better generalization

- What if you don’t have a large dataset?
	medical imaging; robotics; personalized education; translation for rare languages; recommendations
- What if you want a general-purpose AI system in the real world?
- What if your data has a long tail?

- Can we explicitly learn priors from previous experience that lead to efficient downstream learning?


{{TOC}}

## Problem statement
Supervised learning:
$$\argmax_\phi \log p(\phi|\mathcal{D})$$
$$=\argmax_\phi\sum_i\log p(y_i|x_i,\phi)+\log p(\phi)$$
where $\mathcal{D}=\{(x_1,y_1),\cdots,(x_k,y_k)\}$

What is wrong with this?
1. The most powerful models typically require large amounts of labeled data
2. Labeled data for some tasks may be very limited

Can we incorporate additional data?
$$\argmax_\phi \log p(\phi|\mathcal{D}, \mathcal{D}_{meta-train})$$
where $\mathcal{D}_{meta-train}=\{\mathcal{D}_1,\cdots,\mathcal{D}_n\}$ and $\mathcal{D}_i=\{(x^i_1,y^i_1),\cdots,(x^i_k,y^i_k)\}$

What if we don’t want to keep $\mathcal{D}_{meta-train}$ around forever?
- learn *meta-parameters* $\theta: p(\theta|\mathcal{D}_{meta-train})$

$$\log p(\phi|\mathcal{D}, \mathcal{D}_{meta-train})=\log \int_\Theta p(\phi|\mathcal{D}, \theta)p(\theta|\mathcal{D}_{meta-train})d\theta$$
$$\approx\log p(\phi|\mathcal{D}, \theta^*)+\log p(\theta^*|\mathcal{D}_{meta-train})$$

- meta-learning: $\theta^* = \argmax\limits_{\theta} \log p(\theta^*|\mathcal{D}_{meta-train})$
- adaptation $\phi^* = \argmax\limits_\phi \log p(\phi|\mathcal{D}, \mathcal{D}_{meta-train})\approx \argmax\limits_\phi \log p(\phi|\mathcal{D}, \theta^*)$

How do we train this?
- key idea: our training procedure is based on a simple machine learning principle: test and train conditions must match

**The complete meta-learning optimization**
- meta-learning: $\theta^* = \argmax\limits_{\theta} \log p(\theta^*|\mathcal{D}_{meta-train})$
- adaptation $\phi^* = \argmax\limits_\phi \log p(\phi|\mathcal{D}, \theta^*)$, abbr. $\phi^*=f_{\theta^*}(\mathcal{D}^{tr})$

Learn $\theta$ s.t. $\phi=f_\theta(\mathcal{D}^{tr})$

## Meta-learning algorithms

### Black-box adaptation
### Optimization-based inference
### Non-parametric methods
- Bayesian meta-learning
- Meta-learning applica2ons

— 5 min break —

- Meta-reinforcement learning

- Challenges & fron=ers