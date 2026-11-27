---
permalink: /
title: "Jiuyang Liang (梁久阳)"
excerpt: "Computational mathematics, fast algorithms, and machine-learning potentials for long-range systems."
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

My research focuses on computational mathematics and machine learning for scientific computing. I develop fast algorithms and interatomic potentials for systems with long-range interactions. My work combines mathematical analysis, algorithm development, and high-performance computing for molecular dynamics, Monte Carlo simulation, and numerical PDEs.

I am an Assistant Research Fellow at [Shanghai Jiao Tong University](https://www.sjtu.edu.cn/) and a visiting scholar at the [Center for Computational Mathematics, Flatiron Institute](https://www.simonsfoundation.org/people/jiuyang-liang/), where I work with [Shidong Jiang](https://www.simonsfoundation.org/people/shidong-jiang/) and [Leslie Greengard](https://www.simonsfoundation.org/people/leslie-greengard/).

## Research interests

- **Fast algorithms for particle systems.** I develop kernel approximations, spectral methods, and randomized algorithms for efficient long-range calculations, including electrostatics in bulk and at interfaces.
- **Machine learning for long-range interactions.** I study how to represent nonlocal interactions in interatomic potentials, with an emphasis on electrostatics and polarization.
- **Fast solvers for PDEs.** I work on kernel splitting and fast convolution for wave and potential problems.

## Selected publications
{: #publications}

- **Ewald summation with prolates (ESP).** We use prolate spheroidal wave functions to reduce the grid and communication costs of long-range electrostatics in molecular dynamics. [Nature Communications, 2026](https://doi.org/10.1038/s41467-026-73232-8)
- **Machine-learning interatomic potentials for long-range systems (SOG-Net).** We use a sum-of-Gaussians representation to learn long-range interactions in molecular and condensed-phase systems. [Physical Review Letters, 2025](https://doi.org/10.1103/ssp9-7s81) (Editors’ Suggestion)
- **Spectral electrostatics in quasi-2D systems.** We develop a fast sum-of-Gaussians method with spectral accuracy for systems periodic in two directions and nonperiodic in the third. [Numerische Mathematik, 2026](https://doi.org/10.1007/s00211-025-01518-y)
- **Fast Monte Carlo for periodic Coulomb systems.** We develop an algorithm with logarithmic cost per Monte Carlo step for periodic systems with long-range Coulomb interactions. [SIAM Journal on Scientific Computing, 2026](https://doi.org/10.1137/26M1841938)

[Full publication list]({{ '/publications/' | relative_url }}) · [Preprints]({{ '/publications/' | relative_url }}#preprints){: #preprints}

## Research software
{: #software}

- **Ewald summation with prolates:** available in [LAMMPS as `kspace_style esp`](https://docs.lammps.org/kspace_style.html) ([development repository](https://github.com/LiangJiuyang/Ewald-Splitting-with-Prolates)). See also the [GROMACS implementation](https://github.com/lu1and10/Ewald-Splitting-with-Prolates). The [OpenMM integration of NVIDIA cuPotential](https://docs.nvidia.com/cuda/cupotential/theory/splitting) uses prolate splitting by default.
- **Automatic slab sizing in LAMMPS:** [`kspace_modify slab auto`](https://docs.lammps.org/kspace_modify.html) selects the slab extension for quasi-2D Ewald and PPPM electrostatics from the force tolerance and box geometry.

## Academic background

I received my Ph.D. in computational mathematics from Shanghai Jiao Tong University in 2023, advised by [Zhenli Xu](https://math.sjtu.edu.cn/faculty/xuzl/), and my B.S. in mathematics from Zhiyuan College, Shanghai Jiao Tong University, in 2017.

[Talks and posters]({{ '/activities/' | relative_url }}#talks-and-posters){: #talks-and-posters} · [Mentoring]({{ '/activities/' | relative_url }}#mentoring){: #mentoring} · [Honors and awards]({{ '/activities/' | relative_url }}#honors-and-awards){: #honors-and-awards-2017-} · [Grants]({{ '/activities/' | relative_url }}#research-grants-and-talent-programs){: #research-grants-and-talent-programs} · [Patents]({{ '/activities/' | relative_url }}#patents){: #patent} · [Journal refereeing]({{ '/activities/' | relative_url }}#journal-refereeing){: #journal-referees}
