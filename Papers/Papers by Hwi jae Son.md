[Publications by Hwi jae Son]

### 1. Deep Neural Network Approach to Forward-Inverse Problems

<https://www.aimsciences.org/article/doi/10.3934/nhm.2020011>

- PINN is the method to solve the pde using neural network.
- (studied basic settings before)
- How to use this in Inverse problem? ... Estimating operator's parameter together with loss convergence.
- typo) TP equation IC, coefficients. 10/4, not 0.25
- typo) Figure says (alpha, beta, delta, gamma) = (1, 0.4, 0.1, 0.4) (convergence points)
but the below statement is told as (1, 0.4, 0.4, 0.1)
I followed figure's guide, (1, 0.4, 0.1, 0.4)


### 2. Enhanced Physics-Informed Neural Networks with Augmented Lagrangian Relaxation Method (AL-PINNs)

<https://www.sciencedirect.com/science/article/pii/S0925231223005477>

- Optimization method: 1) Lagrangian 2) penalty method.
- Augmented Lagrangian method: Combining two and define the min-max problem


### 3. Traveling Wave Solutions of Partial Differential Equations Via Neural Networks

<https://link.springer.com/article/10.1007/s10915-021-01621-w>

- PINN + Inverse problem: (To approximate traveling wave solution with Neural Networks, wave speed with Inverse problem's parameter.)
- Keller–Segel equation: our interested equation.
- Anjats


### 4. Lagrangian dual framework for conservative neural network solutions of kinetic equations

<https://arxiv.org/abs/2106.12147>

- 
-
-


### 5. Continuous probabilistic solution to the transient self-oscillation under stochastic forcing: a PINN approach

<https://link.springer.com/article/10.1007/s12206-023-0707-z>

- 
-
-


### 6. SOBOLEV TRAINING FOR PHYSICS INFORMED NEURAL NETWORKS

<https://arxiv.org/abs/2101.08932>

- Sobolev-training: Use the 'sobolev-norm' instead.
- Although it is not fully supervised, 
-


### 7. The deep minimizing movement scheme

<https://www.sciencedirect.com/science/article/pii/S0021999123006137>

- Recently, optimization of a functional defined on a space of probability measures equipped with 𝐿2-Wasserstein
distance arises as an important problem. Therefore, Wasserstein gradient flow plays an important role in studying the steepest
descent of a target functional in the space of probability measures
-
-


### 8. Physics-Informed Neural Networks for Microprocessor Thermal Management Model

<https://ieeexplore.ieee.org/abstract/document/10305161>

- 
-
-


[Publication by Sung woong Cho]

 
### 1. The monotone traveling wave solution of a bistable three-species competition system via unconstrained neural networks

<https://www.aimspress.com/aimspress-data/mbe/2023/4/PDF/mbe-20-04-309.pdf>

- With competitive model, travelin wave equation has an unique solution.
-
-


### 2. HyperDeepONet: learning operator with complex target function space using the limited resources via hypernetwork

<https://arxiv.org/abs/2312.15949>

- HyperDeepONet relieves the complexity of DeepONet(compx frm discont, nonsmooth) using hypernetwork.
- It facilitates learning an operator with a small number of parameters in the target network
- It replaces branch net with the hypernetwork.
- Therefore, the main idea is to use the hypernetwork, which takes an input function u and produces the weights of the target network
- (Non-linear Banach to Banach) (At the page 4, DeepONet framework is explained well)
- 



[Notes]

- Gradient flow: On (M, g), u: (0, inf) -> M and F: M -> R satisfies du/dt = -grad_M(F(u(t))).
For example, Heat equation is the gradient flow of dirichlet energy.
