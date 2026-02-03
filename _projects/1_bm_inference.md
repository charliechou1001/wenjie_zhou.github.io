---
layout: page
title: BM Inference Accelerator
description: Hardware-efficient implementation of N-BEATS using block minifloat arithmetic.
img: assets/img/publication_preview/bm_inference_arch.jpg
importance: 1
category: PhD Research
---

[cite_start]Performance is crucial for the evolution of Deep Neural Networks (DNNs), particularly as computational requirements are surging. [cite_start]This research investigates block arithmetic as a promising technique that reduces precision requirements and power consumption, using shared exponents to expand the dynamic range of elements.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/publication_preview/bm_unit.jpg" title="BM Arithmetic Unit" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/publication_preview/inference_results.jpg" title="Inference Accuracy" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    [cite_start]Left: Hardware architecture of the block minifloat (BM) arithmetic unit; [cite_start]Right: Accuracy comparison of BM versus integer and floating-point on N-BEATS.
</div>

### Key Contributions

- [cite_start]**First BM Implementation for Inference:** We propose the block minifloat (BM) implementation for inference, the first implementation of an FPGA-based accelerator using BM arithmetic during publication.
- [cite_start]**Hardware Efficiency and Accuracy:** We demonstrate hardware efficiency and accuracy benefits over integer and floating-point on N-BEATS.
- [cite_start]**Accuracy Parity with Lower Precision:** This research demonstrates that block arithmetic can offer the same accuracy as contemporary approaches using integer and floating point, with lower precision leading to lower resource utilization.
