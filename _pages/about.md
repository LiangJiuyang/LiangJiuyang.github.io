---
permalink: /
title: "Jiuyang Liang (梁久阳)"
excerpt: "Computational mathematics, fast algorithms, and machine-learning potentials for long-range systems."
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

My research spans applied and computational mathematics as well as scientific machine learning. I develop fast algorithms and machine learning interatomic potentials for systems with long-range interactions. My work combines mathematical analysis, algorithm development, and high-performance computing, with applications ranging from molecular dynamics and Monte Carlo simulation to wideband Helmholtz problems that arise in computational electromagnetics.

I am an Assistant Research Fellow at [Shanghai Jiao Tong University](https://www.sjtu.edu.cn/) and a visiting scholar at the [Center for Computational Mathematics, Flatiron Institute](https://www.simonsfoundation.org/people/jiuyang-liang/), where I work with [Shidong Jiang](https://www.simonsfoundation.org/people/shidong-jiang/) and [Leslie Greengard](https://www.simonsfoundation.org/people/leslie-greengard/). I received my Ph.D. in computational mathematics from Shanghai Jiao Tong University in 2023, advised by [Zhenli Xu](https://math.sjtu.edu.cn/faculty/xuzl/), and my B.S. in mathematics from Zhiyuan College, Shanghai Jiao Tong University, in 2017.
{: #academic-background}

[Talks and posters]({{ '/activities/' | relative_url }}#talks-and-posters){: #talks-and-posters} · [Mentoring]({{ '/activities/' | relative_url }}#mentoring){: #mentoring} · [Honors and awards]({{ '/funding-and-recognition/' | relative_url }}#honors-and-awards){: #honors-and-awards-2017-} · [Grants]({{ '/funding-and-recognition/' | relative_url }}#research-grants-and-talent-programs){: #research-grants-and-talent-programs} · [Patents]({{ '/activities/' | relative_url }}#patents){: #patent} · [Journal refereeing]({{ '/activities/' | relative_url }}#journal-refereeing){: #journal-referees}

## Research interests

- **Fast algorithms for particle systems.** I develop kernel approximations, spectral methods, and randomized algorithms for efficient long-range calculations, including electrostatics in bulk and at interfaces.
- **Machine learning for long-range interactions.** I study how to represent nonlocal interactions in interatomic potentials, with an emphasis on electrostatics and polarization.
- **Fast solvers for PDEs.** I develop fast algorithms for the Poisson equation and kernel-splitting methods for wideband Helmholtz problems.
- **High-performance computing.** I design scalable CPU and GPU implementations of numerical algorithms, with an emphasis on reducing communication and memory costs in large simulations.

## Selected publications
{: #publications}

- **Ewald summation with prolates (ESP).** We use prolate spheroidal wave functions to reduce the grid and communication costs of long-range electrostatics in molecular dynamics. [**Nature Communications**, 2026](https://doi.org/10.1038/s41467-026-73232-8)
- **Machine-learning interatomic potentials for long-range systems (SOG-Net).** We use a sum-of-Gaussians representation to learn long-range interactions in molecular and condensed-phase systems. [Physical Review Letters, 2025](https://doi.org/10.1103/ssp9-7s81) (Editors’ Suggestion)
- **Spectral electrostatics in quasi-2D systems.** We develop a fast sum-of-Gaussians method with spectral accuracy for systems periodic in two directions and nonperiodic in the third. [Numerische Mathematik, 2026](https://doi.org/10.1007/s00211-025-01518-y)
- **Fast Monte Carlo for periodic Coulomb systems.** We develop an algorithm with logarithmic cost per Monte Carlo step for periodic systems with long-range Coulomb interactions. [SIAM Journal on Scientific Computing, 2026](https://doi.org/10.1137/26M1841938)
- **Error analysis of the u-series method.** The u-series is used to compute electrostatics on D. E. Shaw Research’s Anton 2 and Anton 3 supercomputers. Our error bounds show how the number of Gaussian terms and the real-space cutoff affect energy and force accuracy, helping users choose parameters that meet a target tolerance. [Applied and Computational Harmonic Analysis, 2025](https://doi.org/10.1016/j.acha.2025.101759)

[Full publication list]({{ '/publications/' | relative_url }}) · [Preprints]({{ '/publications/' | relative_url }}#preprints){: #preprints}

## Research software
{: #software}

- **Ewald summation with prolates:** available in [LAMMPS as `kspace_style esp`](https://docs.lammps.org/kspace_style.html) ([development repository](https://github.com/LiangJiuyang/Ewald-Splitting-with-Prolates)). See also the [GROMACS implementation](https://github.com/lu1and10/Ewald-Splitting-with-Prolates). The [OpenMM integration of NVIDIA cuPotential](https://docs.nvidia.com/cuda/cupotential/theory/splitting) uses prolate splitting by default.
- **Automatic slab sizing in LAMMPS:** [`kspace_modify slab auto`](https://docs.lammps.org/kspace_modify.html) selects the slab extension for quasi-2D Ewald and PPPM electrostatics from the force tolerance and box geometry.
- **Random batch Ewald (RBE):** high-performance parallel implementations for long-range electrostatics in molecular dynamics. [LAMMPS code](https://github.com/randbatch-md/lammps-rbe) · [GROMACS code](https://github.com/randbatch-md/gromacs-rbe)
- **SOE and SOG kernel approximations:** [VPMR](https://github.com/LiangJiuyang/VPMR) provides MATLAB tools for approximating kernels by sums of exponentials or Gaussians. [SumOfExponentials.jl](https://github.com/LiangJiuyang/SumOfExponentials.jl) implements the SOE method in Julia. The [C++ implementation](https://github.com/TLCFEM/vpmr) also supports SOE approximations and provides Python bindings.
- **SOG-Net:** [code and examples](https://github.com/DuktigYajie/SOG-Net) for learning long-range interactions in machine learning interatomic potentials, including Deep-SOG and CACE-SOG.
