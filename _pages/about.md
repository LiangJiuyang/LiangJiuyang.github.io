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
- **Fast solvers for PDEs.** I develop fast Poisson solvers and fast solvers for wideband Helmholtz problems.
- **High-performance computing.** I design scalable CPU and GPU implementations of numerical algorithms, with an emphasis on reducing communication and memory costs in large simulations.

{% include litfsi-visualization.html %}

## Selected publications
{: #publications}

{% include selected-publications.html %}

[Full publication list]({{ '/publications/' | relative_url }}) · [Preprints]({{ '/publications/' | relative_url }}#preprints){: #preprints} · [Figure credits]({{ '/figure-credits/' | relative_url }})

## Research software
{: #software}

- **Ewald summation with prolates:** available in [LAMMPS as `kspace_style esp`](https://docs.lammps.org/kspace_style.html) ([development repository](https://github.com/LiangJiuyang/Ewald-Splitting-with-Prolates)). See also the [GROMACS implementation](https://github.com/lu1and10/Ewald-Splitting-with-Prolates). The [OpenMM integration of NVIDIA cuPotential](https://docs.nvidia.com/cuda/cupotential/theory/splitting) uses prolate splitting by default.
- **SOG-Net:** [code and examples](https://github.com/DuktigYajie/SOG-Net) for learning long-range interactions in machine learning interatomic potentials, including Deep-SOG and CACE-SOG.
- **Automatic slab sizing in LAMMPS:** [`kspace_modify slab auto`](https://docs.lammps.org/kspace_modify.html) selects the slab extension for quasi-2D Ewald and PPPM electrostatics from the force tolerance and box geometry.
- **Random batch Ewald (RBE):** high-performance parallel implementations for long-range electrostatics in molecular dynamics. [LAMMPS code](https://github.com/randbatch-md/lammps-rbe) · [GROMACS code](https://github.com/randbatch-md/gromacs-rbe)
- **SOE and SOG kernel approximations:** [VPMR](https://github.com/LiangJiuyang/VPMR) provides MATLAB tools for approximating kernels by sums of exponentials or Gaussians. [SumOfExponentials.jl](https://github.com/LiangJiuyang/SumOfExponentials.jl) implements the SOE method in Julia. The [C++ implementation](https://github.com/TLCFEM/vpmr) also supports SOE approximations and provides Python bindings.
