# Verified Instruction-Level Energy Consumption Measurement for NVIDIA GPUs

1. Energy consumption measurement for the different instructions that can execute in modern NVIDIA GPUs

2. Accurate measurement of any GPU kernel's energy consumption using **Multi-Threaded Synchronized Monitoring (MTSM)**

## Hardware Dependencies

* A GPU device with cc=30+ (Kepler architecture)

## Software Dependencies

* Cuda v.10.1 or later
* GCC v.7 or later
* make

## In this Repository

* **Instructions_Microbenchmarks:** PTX microbenchmarks to stress the GPU and compute the energy consumption of each instruction using MTSM technique

* **SMA:** Query the GPU's onboard power sensors to read the instantaneous power usage of the GPU device using NVML - Sampling Monitoring Approach running in the background

* **MTSM:** Compute the energy consumption of any GPU Kernel using Multi-Threaded Synchronized Monitoring (MTSM)


## Paper

* [CF ’20] Verified Instruction-Level Energy Consumption Measurement for NVIDIA GPUs

* If you find this code useful in your research, please consider citing as:

```
@inproceedings{Arafa2020GPUEnergy,
  author = {Y. {Arafa} and A. {ElWazir} and A. {ElKanishy} and Y. {Aly} and A. {Elsayed} and A. {Badawy} 
  and G. {Chennupati} and S. {Eidenbenz} and N. {Santhi}},
  title = {Verified Instruction-Level Energy Consumption Measurement for NVIDIA GPUs},
  year = {2020},
  booktitle = {Proceedings of the 17th ACM International Conference on Computing Frontiers},
  series = {CF’20},
  url = {https://doi.org/10.1145/3387902.3392613},
  doi = {10.1145/3387902.3392613},
  publisher = {Association for Computing Machinery},
  address = {New York, NY, USA}
}
```


### Classification

GPUs-Energy is part of the original PPT (https://github.com/lanl/PPT) and is Unclassified and contains no Unclassified Controlled Nuclear Information. It abides with the following computer code from Los Alamos National Laboratory

  * Code Name: Performance Prediction Toolkit, C17098
  * Export Control Review Information: DOC-U.S. Department of Commerce, EAR99
  * B&R Code: YN0100000

### License

&copy 2017. Triad National Security, LLC. All rights reserved.

This program was produced under U.S. Government contract 89233218CNA000001 for Los Alamos National Laboratory (LANL), which is operated by Triad National Security, LLC for the U.S. Department of Energy/National Nuclear Security Administration.

All rights in the program are reserved by Triad National Security, LLC, and the U.S. Department of Energy/National Nuclear Security Administration. The Government is granted for itself and others acting on its behalf a nonexclusive, paid-up, irrevocable worldwide license in this material to reproduce, prepare derivative works, distribute copies to the public, perform publicly and display publicly, and to permit others to do so.

Recall that this copyright notice must be accompanied by the appropriate open source license terms and conditions. Additionally, it is prudent to include a statement of which license is being used with the copyright notice. For example, the text below could also be included in the copyright notice file: This is open source software; you can redistribute it and/or modify it under the terms of the Performance Prediction Toolkit (PPT) License. If software is modified to produce derivative works, such modified software should be clearly marked, so as not to confuse it with the version available from LANL. Full text of the Performance Prediction Toolkit (PPT) License can be found in the License file in the main development branch of the repository.
