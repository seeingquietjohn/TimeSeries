Fun experiments related to time series forecasting/analysis, manifold learning, and chaos theory/dynamics. 

ForecastingBench: Oftentimes an observed equidistant 1-dimensional time series $\{x_t\}_{t=1, 2, \dots, N}$ is believed to be a *measurement* of some $d$-dimensional dynamical system described by 
$$x_k = h(s_k) = h(f^k(s_0))$$
where $f^k$ denotes the $k$-fold iteration of a smooth dynamical system $f: M \to M$ and $h: M \to \mathbb{R}$ the *measurement function*. By *state space reconstruction* we mean the problem of recreating the states $s_i$ only given the measurements $x_i$. Even though it is typically impossible to reconstruct the states in its original coordinates as both $f$ and $h$ are unknown, we may be able to estimate $\hat{s}_i$ that is mathematically equivalent (diffeomorphic) to the original form. The notebook below implements and benchmarks a few different data-driven approaches to state space reconstruction and related methods. 
