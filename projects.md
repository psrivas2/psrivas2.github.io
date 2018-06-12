## Programmable Deep In-Memory Computing (thesis)

Supervisors: Prof. Vikram Adve and Prof. Naresh Shanbhag

Deep in-memory computing results show that they can provide orders of magnitude improvement (energy-delay product) over conventional digital accelerators (GPUs) as well as ASICs.
We aim to solve the programmability challenges in order to bring these highly unconventional novel architectures to mainstream.

Recently, we collaborated with architects of Compute Memory (CM, a deep in-memory computing architecture) to compile machine learning (ML) algorithms written in Julia programming language to CM. The outcome was the first programmable mixed signal accelerator for machine learning based on deep in-memory computing, called PROMISE. 

Encouraged by our results, we will extend this work to port widely used ML DSLs like TensorFlow, PyTorch or MXNet to a system on a chip (SoC) comprised of multicore CPUs, multiple GPUs, and PROMISE.

We plan to leverage our prior experience in designing HPVM, a parallel program representation for heterogeneous systems, designed to enable performance portability across popular parallel hardware such as GPUs, vector instructions sets, muticore CPUs and potentially FPGAs.
We propose to extend HPVM to support mapping and code generation for an SoC with general purpose digital processors (multicore CPUs, and GPUs), and deep in-memory computing accelerator PROMISE. We propose to design novel scheduling algorithms at HPVM IR level to guarantee overall accuracy, throughput, and energy efficiency requirements of the application.

## HPVM: Heterogeneous Parallel Virtual Machine

Supervisors: Prof. Vikram Adve and Prof. Sarita Adve

A compiler infrastructure and parallel program representation for heterogeneous parallel systems, with the goal of making it much easier to write performance-portable parallel programs.  A single program in the HPVM representation can be compiled to GPUs and to multicore CPUs (with and without) vector extensions, while achieving performance close to separately hand-tuned code for each of those systems.  The project is also exploring code generation for FPGAs, for specialized deep-in-memory compute hardware, and developing optimizing compilers for parallel languages like OpenMP and Domain Specific Languages


## Feasibility Study of Hessian Free Optimization Library for Deep Learning

Supervisor: Prof. Justin Sirignano

Current and emerging applications are increasingly relying on the ability to extract patterns from large data sets to  support  inference  and  decision  making  with  Deep  neural networks  (DNNs).  Such  DNNs  have  begun  to  offer  higher performance than humans in cognitive and decision making tasks. Learning the parameters of neural networks is a well studied problem within the field of machine learning. Typically an  extension  of  stochastic  gradient  descent  (SGD)  algorithm is  used  to  train  large  neural  networks  today.  However,  it  has been shown that SGD does not generalize well to deep large networks  or  networks  with  unconventional  architecture  such as  recurrent  neural networks (RNNs), which  exhibit  the vanishing gradient problem. Typically the experience has been that either SGD is too slow or gets stuck in a local minimum altogether. To tackle this the deep learning community has essentially proposed two  solutions: (a) modify  the  network  architecture to overcome the vanishing gradient problem, or (b) try second order optimization methods which model the local curvature  and  correct  for  it.  Due  to  the  success  of LSTMs, GRUs in  specific  domains, the  focus  of  the  community  has been  largely on former techniques of  modifying the network architecture than exploring training algorithms beyond SGD. In this work, we studied the second order optimization technique by Martens, and try to replicate their results. In the process we also proposed the design of a library of hessian free  optimization  technique  and  implement  it  using  numpy and  scipy.  Furthermore,  we  did  a  comparison  of  hessian  free optimization with SGD and present our findings along with the effect of hyper parameters on training networks with hessianfree optimization. The final report is available [here](reports/hf.pdf).
