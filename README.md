# Hardware Acceleration Circuit Design of Object Detection Network Based on FPGA
2020 xilinx summer school

# Instruction

&#8195;In this project, according to the construction principle of iSmart2, a lightweight convolutional neural network is designed to complete the target detection task, which is mainly composed of 3×3 channel convolution and 1×1 point convolution. Then, FPGA hardware acceleration circuit modules are designed for these two types of convolutions to improve the speed of convolution operation, and the development board resources are saved by multiplexing the convolution operation modules. 
  
&#8195;The hardware acceleration circuit designed on the PYNQ-Z2 development board can accomplish the target detection task well, and the output boundary box can accurately select the pedestrian or object in the picture.

# Improvements
&#8195;Summernet is improved on the basis of ismart2, with the following two main improvements：
- **Summernet has more 1*1 pointwise convolution calculation units than ismart2**
- **The bounding box can be read and marked on the input picture**

# organization
- HLS_summernet: The summernet model implemented using HLS.

- Host_summernet: The bit and tcl file for FPGA configuration.and host code run on CPU for FPGA control.

# Reference
- https://github.com/onioncc/iSmartDNN
