# Senior Embedded Software Engineer | C/C++ | Embedded Linux/RTOS | AI Inference & Performance Optimization

I develop **embedded C/C++ software** across **embedded Linux, RTOS, and bare-metal systems**, targeting Arm Cortex-M/A, ESP32, and RISC-V platforms. My background includes real-time software, Linux device drivers, DSP, multithreading, memory-efficient design, hardware/software integration, and performance optimization, including work on aerospace and industrial systems.

My recent work focuses on **embedded AI inference engineering**: architecture-specific INT8 kernels, multicore execution, compact Transformer/Conformer enablement and acceleration, and FPGA-based neural processing. I contribute to semiconductor-vendor-maintained open-source libraries and validate optimizations on physical microcontroller hardware.

### Open-source contributions

- **[Espressif ESP-DL — PR #347](https://github.com/espressif/esp-dl/pull/347)** — **Submitted** benchmark-driven AUTO-mode dual-core scheduling for large batched GEMM on **ESP32-S3 and ESP32-P4**. Reuses the existing multicore execution path for eligible **INT8, INT16, and W8A16** workloads while keeping smaller shapes on one core. Hardware benchmarks show up to **1.36× faster INT8** and **1.91× faster W8A16** GEMM execution; these are operator-level, not measured end-to-end model gains.
- **[Espressif ESP-DL — PR #346](https://github.com/espressif/esp-dl/pull/346)** — **Submitted** ESP32-S3 INT8 Attention query–key optimization using Xtensa hardware accumulation (QACC) for eligible symmetric INT8 tiles. Measured **1.74× faster full Attention execution** with identical outputs in the tested hardware workload; unsupported shapes retain the existing scalar fallback.
- **[Espressif ESP-NN — PR #46](https://github.com/espressif/esp-nn/pull/46)** — **Merged** batched INT8 fully connected acceleration using optimized **1×1 convolution** and multicore execution, with safe fallback behavior and API compatibility. Measured up to **4.0× on ESP32-S3** and **40.7× on ESP32-P4** versus the prior batched-FC paths.
- **[Espressif ESP-NN — Issue #54](https://github.com/espressif/esp-nn/issues/54)** — **Proposed and prototyped** accelerated INT8 `BATCH_MATMUL` attention using the 1×1 convolution path with nonzero zero-point correction. In an **experimental Espressif TFLite Micro runtime**, integrated accelerated FC and attention paths plus GELU and rank-5 strided-slice operator support, enabling complete compact Transformer inference and measuring up to **3.8× faster end-to-end execution** on embedded hardware. This integration was a prototype, not a merged runtime contribution.
- **Google TensorFlow Lite Micro (TFLM) & Arm CMSIS-NN** — **Upstream contributions in development**, focused on embedded inference runtimes and optimized neural-network kernels.
- **[MemKit](https://github.com/NetKit-Labs/memkit) — Creator & Maintainer** — Open-source embedded **C++26 container library with C++/C23 APIs**, comprising 14 C containers and 32 C++ utilities. Includes ring buffers, lock-free queues, maps, and pools with static/arena, heap, and virtual-memory backing for MCUs and embedded Linux. Earned **56 GitHub stars and 8 forks** soon after release.

### External contributor report card

<img src="External%20Contributor%20Report%20Card%20Infographic.png" alt="AI-generated external contributor report card covering ESP-NN PR #46, ESP-DL PRs #347 and #346, and ESP-NN Issue #54" width="750">

*AI-generated assessment of the technical work, not an official review or endorsement by Espressif or its maintainers.*

### Selected engineering projects

#### Embedded software & firmware

- **[KWSKit](https://github.com/NetKit-Labs/kwskit)** — Multithreaded **Zephyr RTOS** firmware on Cortex-M4F, with streaming audio, DSP, and measured hardware timing and memory usage.
- **[adxl345](https://github.com/NetKit-Labs/adxl345)** — I²C accelerometer **Linux kernel driver** with interrupt-driven acquisition, C++ userspace library, automated tests, and hardware validation on Arm Cortex-A53.
- **[uartcom](https://github.com/NetKit-Labs/uartcom)** — Register-level STM32F446RE USART **peripheral driver** and bare-metal C++ firmware, with interrupt-driven I/O, custom startup/clock configuration, and automated tests.

#### Embedded AI & inference optimization

- **[NetKit](https://github.com/NetKit-Labs/netkit)** — Portable C++ FP32/INT8 neural-network inference runtime for MCUs and embedded Linux, integrating CMSIS-NN, ESP-NN, and XNNPACK, with selected INT8 kernels up to **10× faster** than TensorFlow Lite Micro reference implementations.
- **[NPUKit](https://github.com/NetKit-Labs/npukit)** — FPGA-based INT8 neural-network accelerator on Zynq-7020, featuring an 8×8 SystemVerilog systolic GEMM array, AXI DMA tiling, and hardware/software integration validated on physical hardware.

### More projects & professional profile

[NetKit Labs](https://github.com/NetKit-Labs) · [Personal repositories](https://github.com/jameslavrenz?tab=repositories) · [LinkedIn](https://www.linkedin.com/in/jameslavrenz/)

