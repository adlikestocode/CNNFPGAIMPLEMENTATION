Below is a sample README document that integrates your notes and covers both the application of CNNs for pancreatic cancer screening via EUS and non‐trivial FPGA implementation aspects, including benchmarking with pretrained models.

---

# FPGA-Based CNN Accelerator for Pancreatic Cancer Screening via EUS  
### & Benchmarking Pretrained Models for FPGA Deployment

## About  
This repository is for research focusing on implementing CNNs on FPGAs—developing or adopting a proper workflow and methodology and identifying the various challenges in this process. Our project has two main objectives:  
1. **Application:** Develop an automated system to screen pancreatic cancer from Endoscopic Ultrasonography (EUS) images, addressing the tedious and error-prone nature of manual evaluation.  
2. **Innovation:** Explore non-trivial FPGA implementation of CNNs by optimizing model deployment for low cost, low power, and real-time performance.

## Synopsis  
**FPGA-Based Low-Cost, Real-Time Microbial Screening System**  
In response to healthcare challenges, especially during pandemics, there is a demand for rapid and cost-effective diagnostic tools. Conventional tests (like PCR or culture) are accurate but slow and expensive. Our solution proposes an FPGA-based CNN accelerator integrated with standard microscopes to perform real-time microbial screening, with the current focus on pancreatic cancer detection via EUS.

## Methodology  
### 1. Model Development & Application  
- **Data Acquisition & Preprocessing:**  
  Collect and preprocess EUS images, organizing them into train/validation/test splits.
- **CNN Training:**  
  Train a CNN to classify healthy vs. non-healthy pancreatic tissue.  
- **Benchmarking Pretrained Models:**  
  - **EfficientNet-Lite:** Offers high accuracy with low computational cost, optimized for INT8 quantization, making it ideal for FPGA deployment.  
  - **MobileNet (V2/V3):** Renowned for its lightweight architecture and proven efficiency in edge environments, serving as a strong baseline.
  
### 2. FPGA Implementation  
- **Hardware Selection:**  
  Utilize a cost-effective FPGA (e.g., Nexys DDR with Xilinx Artix-7).
- **Design & Optimization:**  
  Map the CNN using Vivado HLS/hls4ml or custom RTL design, focusing on low latency, dynamic precision scaling, sparsity-aware computation, and DVFS.
- **Integration:**  
  Develop interfaces to connect directly with conventional microscopes, enabling real-time image capture and processing.

## Expected Outcomes  
- **Rapid, On-Site Screening:** A portable system for fast preliminary diagnostics.  
- **Cost-Effective Deployment:** Lower power consumption and overall cost.  
- **Enhanced Diagnostic Workflow:** Reduced need for expensive confirmatory tests by accurately flagging suspect samples.

## References & Citations  
- Ruano, J., Jaramillo, M., Gómez, M., & Romero, E. (2022). *Robust descriptor of pancreatic tissue for automatic detection of pancreatic cancer in endoscopic ultrasonography*. Ultrasound in Medicine & Biology, 48(8), 1602–1614.  
- [Additional relevant literature and dataset citations]

## Copyright  
To our knowledge, all materials and datasets used in this project are either under public domain, available for research under fair use, or accessed with proper permissions. All external content is cited appropriately.

---

Feel free to adjust any sections or add further details as needed!
