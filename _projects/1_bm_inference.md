---
layout: page
title: BM Inference Accelerator
description: Hardware-efficient implementation of N-BEATS using block minifloat arithmetic.
img: assets/img/publication_preview/bm_inference_arch.jpg
importance: 1
category: PhD Research
---

Performance is crucial for the evolution of Deep Neural Networks (DNNs), particularly as computational requirements are surging. This research investigates block arithmetic as a promising technique that reduces precision requirements and power consumption, using shared exponents to expand the dynamic range of elements.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/publication_preview/BM_inference_gemm-mac.png" title="BM Arithmetic Unit" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/publication_preview/BM_inference_gemm-Systolic_array.png" title="Inference Accuracy" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Hardware architecture of the block minifloat (BM) arithmetic unit; Right: Accuracy comparison of BM versus integer and floating-point on N-BEATS.
</div>

### Key Contributions

- **First BM Implementation for Inference:** We propose the block minifloat (BM) implementation for inference, the first implementation of an FPGA-based accelerator using BM arithmetic during publication.
- **Hardware Efficiency and Accuracy:** We demonstrate hardware efficiency and accuracy benefits over integer and floating-point on N-BEATS.
- **Accuracy Parity with Lower Precision:** This research demonstrates that block arithmetic can offer the same accuracy as contemporary approaches using integer and floating point, with lower precision leading to lower resource utilization.
