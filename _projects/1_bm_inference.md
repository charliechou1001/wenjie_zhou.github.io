---
layout: page
title: BM Inference Accelerator
description: Hardware-efficient implementation of N-BEATS using block minifloat (BM) arithmetic.
importance: 1
category: PhD Research
---

Performance is crucial for the evolution of Deep Neural Networks (DNNs), particularly as computational requirements surge. This project investigates block arithmetic as a promising technique to reduce precision requirements and power consumption by using shared exponents to expand dynamic range. We specifically demonstrate these advantages through an N-BEATS based inference accelerator implemented on FPGA hardware.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/publication_preview/BM_inference_gemm-mac.png" title="BM MAC Unit" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/publication_preview/BM_inference_gemm-Systolic_array.png" title="BM Systolic Array for the global block" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   Left is the BM MAC unit, right is the BM systolic array for the global block.
</div>

### Key Contributions:
- **First BM Accelerator:** We proposed the BM implementation for inference, which marks the first FPGA-based accelerator using BM arithmetic at the time of publication.
- **Hardware Efficiency:** The design demonstrates significant hardware efficiency and accuracy benefits over traditional integer and floating-point implementations when applied to N-BEATS.
- **Practical Validation:** The research outcomes show that block arithmetic offers the same accuracy as contemporary approaches but with lower resource utilization.
 
The results of this research were published in **IEEE APCCAS 2022**.
