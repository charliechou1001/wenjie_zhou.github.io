---
layout: page
title: Delay Update Scheme
description: Efficient block arithmetic rescaling for neural network training acceleration.
img: assets/img/publication_preview/clipping-intro.png
importance: 3
category: work
---

One of the most significant challenges in block arithmetic for DNN training is the **rescaling** computation. To maintain numerical stability, a common approach is **maximum calibration**, which requires scanning all elements in a block to determine the block scale. However, this introduces critical data dependencies and significant hardware overhead, such as the need for large buffers and pipeline stalls.

In this work, we propose a lightweight delay update scheme, **Delay Update**, that simplifies the rescaling process while maintaining high training accuracy. This is the first delayed scaling method optimized for both the global and local block (flexible block) configurations, offering the resource-efficient rescaling logic to date.

<div class="row justify-content-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <img src="{{ '/assets/img/publication_preview/clipping-intro.png' | relative_url }}" alt="Delay Update Logic" class="img-fluid rounded z-depth-1">
    </div>
</div>
<div class="caption">
    Rescaling computation. (a) Maximum calibration method. It has a high latency and high buffer cost. (b) Delayed scaling method. These methods get a better hardware performance, but the rescaling logic is complicated, and only supports the global block. (c) Delay update method. It has a simpler rescaling logic and supports flexible blocks.
</div>

### Key Contributions:

- **Probabilistic Delay Update:** We propose a novel, hardware-efficient delay update scheme scheme based on probabilistic estimation. For scenarios where simple delay updates may drift, we introduce an optimized Weighted Moving Average predictor.
- **Hardware Performance Analysis:** We establish the first performance model to quantify the hardware overhead of data dependency in MX-based GEMM accelerators. Our modeling, validated on FPGA synthesis, reveals that the efficacy of delayed scaling is highly sensitive to block size.
- **Empirical Validation:** Our results show that the proposed scheme achieves near-zero accuracy loss in various network training tasks. And our performance estimation demonstrates that the delayed scaling methods can improve hardware latency by approximately 40% in Transformer or LLM.
