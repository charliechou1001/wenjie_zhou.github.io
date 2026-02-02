---
layout: page
title: 4-bit Training Accelerator
description: Mixed-precision neural network training using 4-bit block minifloat.
importance: 2
category: PhD Research
---

Along with increasing DNN model scale, the training cost is becoming a new problem for energy-efficient AI. This project develops an improved block arithmetic algorithm and implementation methodology for training, specifically examining kernel design under different block arithmetic implementations. We utilize an N-BEATS based training accelerator to demonstrate the advantages of block arithmetic in handling gradient updates at extremely low bit-widths.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/publication_preview/BMGEMM-intro.png" title="introduction" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/publication_preview/BMGEMM-multiblock.png" title="BM GEMM for the local block" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   Left: Summary of the main ideas; Right: the BM systolic array for Mixed-Precision & Cross-block GEMM computation.
</div>

### Key Contributions:
- **4-bit Training Implementation:** Proposed the first FPGA implementation of a 4-bit BM, mixed-precision neural network training system for time-series forecasting.
- **Mixed-Precision & Cross-block Strategy:** propose a novel cross-block BM MAC unit that allows independent block and tile sizes and utilizes a higher precision buffer to improve accuracy.
- **GEMM Kernel Design:** BM GEMM kernel that supports runtime configuration of precision for forward and back-propagation computation.
- **DSP Packing for Training:** A novel, packed 4-bit BM MAC unit that can compute six independent multiplications per DSP is presented.

The results of this research were published in **TRETS 2024**.
