# Senior Software Engineer | Embedded Systems | C/C++ | Embedded Linux/RTOS | AI Inference

I develop **embedded C/C++ software** across **embedded Linux, RTOS, and bare-metal systems**, targeting Arm Cortex-M/A, ESP32, and RISC-V platforms. My background includes real-time software, Linux device drivers, DSP, multithreading, memory-efficient design, hardware/software integration, and performance optimization.

More recently, I've focused on **Embedded AI and inference optimization**, including INT8 neural-network kernels, multicore acceleration, compact Transformer inference, and FPGA-based neural processing. My work includes independent engineering projects and upstream open-source contributions.

### Open-source contributions

- **[Espressif ESP-DL — PR #346](https://github.com/espressif/esp-dl/pull/346)** — Submitted ESP32-S3 INT8 attention query–key optimization using hardware accumulation, achieving **1.74× faster execution** in the tested workload.
- **[Espressif ESP-NN — Issue #54](https://github.com/espressif/esp-nn/issues/54)** — Proposed and prototyped accelerated INT8 attention BATCH_MATMUL using 1×1 convolution with nonzero zero-point correction; published benchmark results for ESP32-S3 and ESP32-P4.
- **[Espressif ESP-NN — PR #46](https://github.com/espressif/esp-nn/pull/46)** — Merged contribution accelerating batched INT8 fully connected layers using optimized 1×1 convolution and multicore execution. Achieved up to **4.0× on ESP32-S3** and **40.7× on ESP32-P4**.
- **[MemKit](https://github.com/NetKit-Labs/memkit) — Creator & Maintainer** — Open-source embedded **C++26 container library with C++/C23 APIs**, comprising 14 C containers and 32 C++ utilities. Includes ring buffers, lock-free queues, maps, and pools with static/arena, heap, and virtual-memory backing for MCUs and embedded Linux. Earned **56 GitHub stars and 8 forks** soon after release.

### Selected engineering projects

#### Embedded software & firmware

- **[KWSKit](https://github.com/NetKit-Labs/kwskit)** — Multithreaded **Zephyr RTOS** firmware on Cortex-M4F, with streaming audio, DSP, and measured hardware timing and memory usage.
- **[adxl345](https://github.com/NetKit-Labs/adxl345)** — Linux I²C accelerometer kernel driver with interrupt-driven acquisition, C++ userspace library, automated tests, and hardware validation on Arm Cortex-A53.
- **[uartcom](https://github.com/NetKit-Labs/uartcom)** — Register-level STM32F446RE USART driver and bare-metal C++ firmware, with interrupt-driven I/O, custom startup/clock configuration, and automated tests.

#### Embedded AI & inference optimization

- **[NetKit](https://github.com/NetKit-Labs/netkit)** — Portable C++ FP32/INT8 neural-network inference runtime for MCUs and embedded Linux, integrating CMSIS-NN, ESP-NN, and XNNPACK, with selected INT8 kernels up to **10× faster** than TensorFlow Lite Micro reference implementations.
- **[NPUKit](https://github.com/NetKit-Labs/npukit)** — FPGA-based INT8 neural-network accelerator on Zynq-7020, featuring an 8×8 SystemVerilog systolic GEMM array, AXI DMA tiling, and hardware/software integration validated on physical hardware.

### More projects & professional profile

[NetKit Labs](https://github.com/NetKit-Labs) · [Personal repositories](https://github.com/jameslavrenz?tab=repositories) · [LinkedIn](https://www.linkedin.com/in/jameslavrenz/)
