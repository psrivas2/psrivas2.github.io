## Programmable Deep In-Memory Computing (thesis)

Supervisors: Prof. Vikram Adve and Prof. Naresh Shanbhag

* Goal: Bring novel in-memory computing to mainstream by using analog computation for energy efficiency
* Designed PROMISE, a programmable analog accelerator for machine learning, its compiler and novel analog ISA
* PROMISE embeds computation deep in SRAM bit cell array, thus avoiding expensive data transfers
* PROMISE is orders of magnitude energy and delay efficient than CPUs and GPUs
* 4.2x lower energy and 2.2x higher throughput than state of art digital ASICs for Machine Learning kernels

## HPVM: Heterogeneous Parallel Virtual Machine

Supervisors: Prof. Vikram Adve and Prof. Sarita Adve

A compiler infrastructure and parallel program representation for heterogeneous parallel systems, with the goal of making it much easier to write performance-portable parallel programs.  A single program in the HPVM representation can be compiled to GPUs and to multicore CPUs (with and without) vector extensions, while achieving performance close to separately hand-tuned code for each of those systems.  The project is also exploring code generation for FPGAs, for specialized deep-in-memory compute hardware, and developing optimizing compilers for parallel languages like OpenMP and Domain Specific Languages


## Feasibility Study of Hessian Free Optimization Library for Deep Learning

Supervisor: Prof. Justin Sirignano

Current and emerging applications are increasingly relying on the ability to extract patterns from large data sets to  support  inference  and  decision  making  with  Deep  neural networks  (DNNs).  Such  DNNs  have  begun  to  offer  higher performance than humans in cognitive and decision making tasks. Learning the parameters of neural networks is a well studied problem within the field of machine learning. Typically an  extension  of  stochastic  gradient  descent  (SGD)  algorithm is  used  to  train  large  neural  networks  today.  However,  it  has been shown that SGD does not generalize well to deep large networks  or  networks  with  unconventional  architecture  such as  recurrent  neural networks (RNNs), which  exhibit  the vanishing gradient problem. Typically the experience has been that either SGD is too slow or gets stuck in a local minimum altogether. To tackle this the deep learning community has essentially proposed two  solutions: (a) modify  the  network  architecture to overcome the vanishing gradient problem, or (b) try second order optimization methods which model the local curvature  and  correct  for  it.  Due  to  the  success  of LSTMs, GRUs in  specific  domains, the  focus  of  the  community  has been  largely on former techniques of  modifying the network architecture than exploring training algorithms beyond SGD. In this work, we studied the second order optimization technique by Martens, and try to replicate their results. In the process we also proposed the design of a library of hessian free  optimization  technique  and  implement  it  using  numpy and  scipy.  Furthermore,  we  did  a  comparison  of  hessian  free optimization with SGD and present our findings along with the effect of hyper parameters on training networks with hessianfree optimization. The final report is available [here](reports/hf.pdf).
