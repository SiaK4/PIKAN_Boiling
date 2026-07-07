# Physics-informed Kolmogorov–Arnold networks (PIKANs) for noise-robust reconstruction of boiling heat flux from infrared measurements

This is the official GitHub repository for the paper:
> **"Physics-informed Kolmogorov–Arnold networks (PIKANs) for noise-robust reconstruction of boiling heat flux from infrared measurements"** > by Siavash Khodakarami, Parimala Vardhan Vydyula, Aniruddha Bora, Justin A. Weibel, and George Em Karniadakis

---

## 📢 Code Availability

⚠️ **All codes, models, and datasets will be made available right after official publication.** We are currently putting the finishing touches on the repository to ensure it is clean, well-documented, and easy to reproduce. **Stay tuned!** 🚀

---

## 📑 Abstract

*Recovering a noise-amplified inverse quantity from corrupted boundary data is a recurring problem in physics-informed learning for real-world applications. 
Specifically,  small perturbations in the measured field are magnified through the spatial derivatives needed to reconstruct the target, and hence conventional discretization solvers turn them into large unphysical oscillations. 
We study this problem through the reconstruction of local time-resolved nucleate-boiling heat flux, which cannot be measured directly and must be inferred from infrared surface temperatures by solving an unsteady three-dimensional heat-conduction problem with sharp and rapidly evolving liquid–vapor interface gradients. We show that neither network architecture nor optimizer alone overcomes the spectral bias that smooths away these interface-scale features, and that the two must be addressed jointly. Our approach combines a Chebyshev physics-informed Kolmogorov–Arnold network (PIKAN) backbone, a quasi-second-order (SOAP) optimizer, and a temperature-annealed residual-based resampling scheme that concentrates collocation points at high-residual interface regions. Trained directly on experimental infrared measurements imposed as a boundary condition, the network resolves high-frequency bubble signatures and the high-flux distribution tail much better than a Fourier-feature PINN of equal size and training budget. In particular, it selectively filters measurement noise while preserving the physically meaningful high-frequency features, suppressing the spurious oscillations that contaminate finite-volume reconstructions and yielding more physically consistent heat-flux estimates from noisy experimental data.*

---

## ✉️ Contact

If you have any questions or would like to chat about the paper ahead of publication, feel free to reach out:
* **Name:** Siavash Khodakarami
* **Email:** siavash_khodakarami@brown.edu
