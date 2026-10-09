---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

I am currently a Master’s student in Electronic Engineering at Nanyang Technological University. I once served as a research assistant at the Institute of Microelectronics (IME), A*STAR, supervised by Prof. <a href="https://dr.ntu.edu.sg/entities/person/Goh-Wang-Ling" target="_blank">Wang Ling Goh</a> and Dr. <a href="https://ieeexplore.ieee.org/author/37408673900" target="_blank">Anh-Tuan Do</a>. I received the Bachelor of Engineering degree in Electronic Information Engineering from Wuhan University, Wuhan, China, in Jun. 2024. My research interest is hardware–software co-design to improve system efficiency. You can find more information through my <a href="files/CV_YuntianLiu.pdf" target="_blank">CV</a>.

# 🧭 Research Tracks

Research interests in high-performance computing architectures, efficient hardware acceleration, and task scheduling.

# 📝 Publications 
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICCAD 2027</div><img src='images/publication/pace.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[A CGRA with SIMD and AGU]

R. Harish, V. P. Nambiar, **<u>Y. Liu</u>**, Y. S. Chong, W. L. Goh, R. Dutta, A. T. Do

*International Conference on Computer-Aided Design (ICCAD), 2027 (manuscript completed, to be submitted)*

<details>
<summary>Abstract</summary>
Coarse-Grained Reconfigurable Arrays (CGRAs) balance low power and flexible computation, making them ideal for edge devices. Traditional CGRAs allocate some Processing Elements (PEs) for memory-access tasks, reducing compute utilization. Our design introduces a Memory Address Generation Unit (AGU) to handle data fetch/store operations, freeing PEs and improving hardware utilization. Simulations show AGU integration can double CGRA utilization, depending on workload. The architecture also supports SIMD for parallel computation, boosting energy efficiency by up to 3.96×. Implemented in 12 nm FinFET, post-layout simulations achieve 1 GHz and a peak energy efficiency of 1.31 TOPS/W, 3.4× higher than state-of-the-art designs.

</details>

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ISCA 2027</div><img src='images/publication/fractal.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Tree-Inspired Techniques for Diffusion Models]

**<u>Y. Liu</u>**, C. Zhou

*International Symposium on Computer Architecture (ISCA), 2027 (manuscript completed, to be submitted)*

<details>
<summary>Abstract</summary>
We propose an adaptive block-dropout framework for diffusion-model denoisers that removes 95.1% of SDXL denoiser FLOPs via tree-structured sparsity, achieving a 15.9× denoising speedup over an NVIDIA L40S GPU dense baseline. We design a sparse diffusion SoC accelerator built around this framework, achieving 2.19×, 2.67×, and 1.56× higher energy efficiency than Cambricon-D, Ditto, and DSTAR respectively, with only 0.63% area overhead. The design is implemented in SystemVerilog and verified via RTL simulation, synthesis, and FPGA validation.
</details>

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TCAS-II 2026</div><img src='images/publication/cntfps.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Distance-Free Farthest Point Sampling Accelerator for Point-Cloud Networks]

**<u>Y. Liu</u>**, X. Zheng, Z. Guo, C. Zhou

*IEEE Transactions on Circuits and Systems II: Express Briefs (TCAS-II), 2026 (in preparation)*

<details>
<summary>Abstract</summary>
Farthest Point Sampling (FPS) is the de-facto down-sampling operator in point-cloud neural networks, but it is inherently sequential and hardware-unfriendly. We propose a counting-based reformulation that eliminates the point-to-sample distance computation of conventional FPS. The method adaptively partitions the point cloud with a fractal, density-aware grid and selects representatives using block occupancies and sub-cell priority logic as a distance-free proxy for spatial coverage, removing the serial arg-max dependency and enabling a parallel streaming schedule. In an algorithm-level model, it is 26× faster than exact FPS at 64k points.
</details>

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ISCAS 2025</div><img src='images/publication/qubit.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Qubit-State Discrimination using Neural Networks with Rapid and Energy-Efficient Compute Arrays]

**<u>Y. Liu</u>**, Y. S. Chong, B. Lienhard, M. Fan, W. L. Goh, V. P. Nambiar, and A. T. Do

*IEEE International Symposium on Circuits and Systems (ISCAS), 2025*

<details>
<summary>Abstract</summary>
Neural networks (NNs) implemented on field-programmable gate arrays (FPGAs) provide fast, high-fidelity solutions for processing readout signals from quantum information processors. However, application-specific integrated circuits (ASICs) instead of FPGAs hold the potential for improved performance, a largely unexplored path. This work proposes specialized hardware for NN-based qubit-state discrimination. We optimize the NN architecture to minimize resource requirements by reducing the layer width, employing linear activation functions, and weight quantization. Quantization-aware training is used to preserve accuracy despite these optimizations. Next, a compute array employing output stationary dataflow is chosen to process the NN workload. The compute array with abundant multipliers and adders can complete one NN inference in 63 ns, which makes it a good candidate for real-time qubit-state discrimination.

</details>

</div>
</div>

# 🔬 Project
<div class='paper-box'><div class='paper-box-image'><div><img src='images/publication/Fornax.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Nebula: Dependency-Aware Task Scheduler for a Point-Cloud NPU]

Task Scheduler Engineer, Nebula Point-Cloud NPU (ISSCC 2025)

<details>
<summary>Abstract</summary>
Built a dependency-aware task scheduler for the Nebula point-cloud NPU (ISSCC 2025) that plans data transfers for task graphs with up to 19k nodes. The scheduler allocates on-/off-chip storage and generates data-transfer instructions on the fly, and is deployed on the Nebula chip.

</details>

</div>
</div>


# 🎖 Honors and Awards
- *2023.08* Second prize, National Undergraduate Electronics Design Contest.
- *2022.08* Second prize, National College Student Integrated Circuit Innovation and Entrepreneurship Competition (Hubei Division).

# 📖 Educations
- *2024.09 - 2026.06 (expected)*, Master of Electronics, Nanyang Technological University, Singapore.
- *2020.09 - 2024.06*, Bachelor of Engineering in Electronic Information Engineering, Wuhan University, Wuhan, China.

# 💻 Internships
- *2025.09 - 2026.01*, Institute of Microelectronics (IME), A*STAR, Singapore.