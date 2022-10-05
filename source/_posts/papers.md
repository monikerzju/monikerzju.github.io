---
title: Publications
thumbnail: 
- /img/pub.png

---

Some papers about Computer Architecture and Operating System.
<!-- more -->

#### The hypervisor work is not available for now...

#### [VDom: Fast and Unlimited Virtual Domains on Multiple Architectures.]()
- Proceedings of the 2023 Conference on Architectural Support for Programming Languages and Operating Systems (**ASPLOS 2023**).
- New findings. We find that a large number of domains are needed in real-world applications, and the challenges to provide fast domain virtualization are how to reduce the overhead caused by waiting for free domains and excessive TLB flushes.
- Efficient domain virtualization with unlimited domains. We leverage separate address spaces to map different groups of virtual domains to the hardware domains in each page table. We propose a domain virtualization algorithm that switches page global directory, and puts a thread in a private address space before domain evictions to reduce unnecessary TLB invalidation.
- Real platform evaluation. We implement a prototype for X86 and ARM based on Linux, and evaluate VDom on real platforms. The results show VDom is fast, compatible, and secure when providing unlimited domains. On server applications, the overheads are less than 2.19% and 2.65% on X86 and ARM, respectively. On random domain access tests, VDom is 4.4-40x faster than libmpk.

#### [RegVault: Hardware Assisted Selective Data Randomization for Operating System Kernels.](/papers/dac22-regvault.pdf)
- Proceedings of the 59th The Design Automation Conference (**DAC 2022**).
- New Hardware Primitives. We design and implement novel hardware primitives, providing cryptographically strong confidentiality and integrity protection supports for register-grained data. We further propose the cryptographic lookaside buffer to reduce the performance overhead.
- New Protection Techniques. We propose chain-based interrupt context protection to protect interrupt contexts. We also propose register spilling protection to safeguard sensitive data spilling via static analysis.
- Prototype and Evaluation. We implement a prototype of RegVault on Linux kernel v5.8.18, protecting six types of sensitive data. Our evaluations show that RegVault can defend against kernel data attacks effectively with a minimal performance overhead.

#### [H2Cache: Building a Hybrid Randomized Cache Hierarchy for Mitigating Cache Side-Channel Attacks.](/papers/seed21-h2cache.pdf)
- 2021 International Symposium on Secure and Private Execution Environment Design (**SEED 2021**).
- We propose a defense scheme against cache side-channel attacks from the perspective of the whole cache hierarchy, including both L1 and L2 caches.
- We present a hybrid randomized cache hierarchy, which leverages the benefits of both table-based and computation-based randomization schemes to meet security and performance needs.
- We design and implement a cache system, H2Cache, on a self-designed RISC-V processor, and perform extensive evaluation including security, performance, and resource utilization on the FPGA platform.