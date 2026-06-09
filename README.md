# Low-Latency Quasi-Static Modeling of UAV Tether Aerodynamics

[![Paper](https://img.shields.io/badge/Paper-arXiv-red?style=flat&logo=arxiv)](https://arxiv.org/pdf/2512.22588)  [![Citations](https://img.shields.io/badge/dynamic/json?label=Citations&query=$[2512.22588].citations&url=https://gist.githubusercontent.com/tommaier123/377d793a6ca2cb79e588d8781d76b521/raw/citation_counts.json&color=blue&logo=semanticscholar)](https://arxiv.org/abs/2512.22588)

## Abstract

One of the main limitations of multirotor UAVs is their short flight time due to battery constraints. A practical solution for continuous operation is to power the drone from the ground via a tether. While this approach has been demonstrated for stationary systems, scenarios with a fast-moving base vehicle or strong wind conditions require modeling the tether forces, including aerodynamic effects.

In this work, we propose two complementary approaches for low-latency quasi-static tether modeling with aerodynamics. The first is an analytical method based on catenary theory with a uniform drag assumption, achieving very fast solve times below 1 ms. The second is a numerical method that discretizes the tether into segments and lumped masses, solving the equilibrium equations using CasADi and IPOPT. By leveraging initialization strategies, such as warm starting and analytical initialization, low-latency performance was achieved with a solve time of 5 ms, while allowing for flexible force formulations.

Both approaches were validated in real-world tests using a load cell to measure the tether force. The results show that the analytical method provides sufficient accuracy for most tethered UAV applications with minimal computational cost, while the numerical method offers higher flexibility and physical accuracy when required. These approaches form a lightweight and extensible framework for low-latency tether simulation, applicable to both offline optimization and online tasks such as simulation, control, and trajectory planning.

## Resources
- [Paper (arXiv)](https://arxiv.org/pdf/2512.22588)

## Citation
If you use this work in your own research, please cite:

```bibtex
@inproceedings{2512.22588,
  author={Beffert, Max and Zell, Andreas},
  booktitle={2026 International Conference on Unmanned Aircraft Systems (ICUAS)}, 
  title={Low-Latency Quasi-Static Modeling of UAV Tether Aerodynamics}, 
  year={2026}
}
