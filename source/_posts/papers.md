---
title: Publications
thumbnail: 
- /img/pub.png

---

Some papers about Computer Architecture and Operating System.
<!-- more -->

#### Isolation work is not publicly available now.

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