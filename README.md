## Pretraining with Random noise for Fast and Robust Learning without Weight Transport

Advances in Neural Information Processing Systems 37 **(NeurIPS 2024)**  
Jeonghwan Cheon*, Sang Wan Lee, Se-Bum Paik†

\* First author: jeonghwan518@kaist.ac.kr  
† Corresponding author: sbpaik@kaist.ac.kr  


### Associated article

This repository contains the implementation and demo codes for the paper "**Pretraining with Random Noise for Fast and Robust Learning without Weight Transport**," which was published as a conference paper at the 38th Annual Conference on Neural Information Processing Systems (**NeurIPS 2024**).

[![arXiv](https://img.shields.io/badge/arXiv-2405.16731-b31b1b.svg)](https://arxiv.org/abs/2405.16731) [![OpenReview](https://img.shields.io/badge/OpenReview-81261b.svg)](https://openreview.net/forum?id=DNGfCVBOnU)  [![Slides](https://img.shields.io/badge/NeurIPS-Slides-68448b.svg)](https://neurips.cc/media/neurips-2024/Slides/96093.pdf) [![Poster](https://img.shields.io/badge/NeurIPS-Poster-68448b.svg)](https://neurips.cc/virtual/2024/poster/96093)

#### Abstract

The brain prepares for learning even before interacting with the environment, by refining and optimizing its structures through spontaneous neural activity that resembles random noise. However, the mechanism of such a process has yet to be understood, and it is unclear whether this process can benefit the algorithm of machine learning. Here, we study this issue using a neural network with a feedback alignment algorithm, demonstrating that pretraining neural networks with random noise increases the learning efficiency as well as generalization abilities without weight transport. First, we found that random noise training modifies forward weights to match backward synaptic feedback, which is necessary for teaching errors by feedback alignment. As a result, a network with pre-aligned weights learns notably faster and reaches higher accuracy than a network without random noise training, even comparable to the backpropagation algorithm. We also found that the effective dimensionality of weights decreases in a network pretrained with random noise. This pre-regularization allows the network to learn simple solutions of a low rank, reducing the generalization loss during subsequent training. This also enables the network robustly to generalize a novel, out-of-distribution dataset. Lastly, we confirmed that random noise pretraining reduces the amount of meta-loss, enhancing the network ability to adapt to various tasks. Overall, our results suggest that random noise training with feedback alignment offers a straightforward yet effective method of pretraining that facilitates quick and reliable learning without weight transport.

#### Research highlights

- Weight alignment to synaptic feedback during random noise training
- Pretraining random noise enables fast learning during subsequent data training
- Pre-regularization by random noise training enables robust generalization
- Task-agnostic fast learning for various tasks by a network pretrained with random noise

### Simulations and experiments

Each simulation and experimental result can be replicated by running the corresponding demo files in the ```\demo``` directory. The detailed and core implementation of the model can be found in the ```\src``` directory.

#### Prerequisites

- Python 3.11 (Python software foundation)
- Pytorch 2.1 + CUDA 11.8
- NumPy 1.26.0
- SciPy 1.11.4


### Citation

```bibtex
@article{cheon2024pretraining
    title={Pretraining with Random Noise for Fast and Robust Learning without Weight Transport},
    author={Cheon, Jeonghwan and Lee, Sang Wan and Paik, Se-Bum},
    journal={Advances in Neural Information Processing Systems},
    volume={37},
    year={2024}
}
```
