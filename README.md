# course-lab_finn

## About This Project
**"From AI to Gate"** project is a tutorial project based on the [Xilinx FINN](https://xilinx.github.io/finn/) framework. FINN is an experimental framework from Xilinx Research Labs to explore deep neural network inference on FPGAs. It specifically targets quantized neural networks, with emphasis on generating dataflow-style architectures customized for each network. It is not intended to be a generic DNN accelerator, but rather a tool for exploring the design space of DNN inference accelerators on FPGAs.

We studied the Xilinx FINN open source code and try to provide more detailed explainations about the **binarized nueral network hardware** part. Since the [FINN framework](https://github.com/Xilinx/finn) consists of several repositories such as [finn-base](https://github.com/Xilinx/finn-base), [finn-hls](https://github.com/Xilinx/finn-hlslib), [finn-examples](https://github.com/Xilinx/finn-examples) and [Brevitas](https://github.com/Xilinx/brevitas), we arrange the tutorials into 7 chapters in the textbook "[From AI to Gate](https://www.boledu.org/)". We hope that readers can have a big picture of the whole framework after reading this tutorial.

For more fundamental introduction and tutorials, please refer to the textbooks in [BOLEDU website](https://www.boledu.org/).

**※Credits:** We greatly appreciate the Xilinx FINN team to opensource this project, as well as the detailed documentations. What we would like to do is to organize the full work into a textbook format and add more studies about the high-level-synthesis hardware part. Any comments or advises are welcomed. Again, we would like to thank for this outstanding work.


## What You Will Learn in This Lab
In this lab , readers are able to define and train a custom(with some restrictions) quantized neural network as well as the deployment of this neuaral network to edge devices. Since we are focusing on the binarized neural network, readers are also capable of explaining the detailed binarized hardware architecture and the dataflow of the overall system.


## Who is This Book For

**"From AI to Gate"** textbook is for those who are interested in end-to-end neural network model defining, training, hardware designing and network deployment. We will go through the detailed binarized neural network hardware design using High-Level-Synthesis methodology. In this case, here are some prerequisites.

## Prerequisites

* Classical Deep Learning

We assume that readers are familiar with classical deep learning commponents such as fully-connected layers (mlp: multilayer perceptron), 2D convolution layers, max-pooling and batch normalization. Classical neural network architectures such as AlexNet will be helpful. 

* High-Level-Synthesis Concept, C/C++

Additionally, since the hardware implementation is based on HLS, C/C++ coding language is a requirement as well as basic High-Level-Synthesis concepts. The HLS tool we will be using is Xilinx Vivado HLS, however general HLS concepts such as unroll, pipeline pragma is enough.

* Python

We will use Jupyter Notebook to run the example python codes. The deep learning framework and APIs we will be using is python. The FINN compiler itself also uses python backend. The compiling APIs are also written in python. Here, the code explaination in [Compiler](../3-compiler/README.md) and [Verification](../4-verification/README.md) chapters are mostly python.

* (Pytorch) optional

The deep learning framework is [Brevitas](https://github.com/Xilinx/brevitas) (PyTorch based rather than Tensorflow based). However, all the network define and training process are similar and should not be a barrier for those using different deep learning frameworks.

* (Docker) optional

Due to the high library dependency of FINN, the FINN team provides a [docker](https://docs.docker.com/get-started/) to simplify the environment setup process. Again, this should not be a barrier for those who has no experience to it. 


## References

Most of the references of this textbook are listed here. Readers are encouraged to dive into these pages for greater details.

* Xilinx Official Github Pages: https://xilinx.github.io/finn/

*  Xilinx Official Documents: https://finn.readthedocs.io/en/latest/

* Xilinx FINN Repositories: 
    * FINN framework: https://github.com/Xilinx/finn
    * finn-base: https://github.com/Xilinx/finn-base
    * finn-hls: https://github.com/Xilinx/finn-hlslib

* Xilinx Brevitas: https://github.com/Xilinx/brevitas


* Xilinx FINN Examples:
    * FINN Examples: https://github.com/Xilinx/finn-examples
    * BNN-PYNQ: https://github.com/Xilinx/BNN-PYNQ

* Xilinx FINN Publications: https://xilinx.github.io/finn/publications
    * [FINN: A Framework for Fast, Scalable Binarized Neural Network Inference](https://arxiv.org/abs/1612.07119)
    * [FINN-R: An End-to-End Deep-Learning Framework for Fast Exploration of Quantized Neural Networks](https://arxiv.org/abs/1809.04570)

* Xilinx Vitis HLS Pragmas: https://www.xilinx.com/html_docs/xilinx2021_1/vitis_doc/hls_pragmas.html


