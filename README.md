# R-DLRHyIn
Implementation of the paper "Robust Hyperspectral Inpainting via Low-Rank Regularized Untrained Convolutional Neural Network", IEEE GRSL, 2023,

[[Paper]](https://ieeexplore.ieee.org/abstract/document/10032531)

___

**Abstract:** 

Over the past decade, many low-rank models, factorizations, or approximations have been applied to the restoration of hyperspectral images (HSIs) (e.g., denoising, inpainting, and super-resolution) from their incomplete and/or noisy measurements. Recently, deep learning (DL) has been shown to be a powerful method for solving inverse problems (including HSI restoration), but a large amount of training data is required. Since this is not possible for HSIs, unlike red green blue (RGB) images, in this work, a novel unsupervised framework for hyperspectral inpainting (HI) is proposed that can be implemented using an untrained convolutional neural network (CNN) for deep image prior (DIP), together with a recently reported differentiable regularization for the data rank and ℓ2 -norm squared loss function. Based on the proposed framework, we come up with a novel HI algorithm [denoted as deep low-rank hyperspectral inpainting (DLRHyIn)] and a robust DLRHyIn (denoted as R-DLRHyIn) which is robust against outliers, where the latter differs from the former only in the Huber loss function (HLF) (which has been justified robust to mixed noise) used instead. Then some simulation results and real-data experiments are provided to demonstrate the effectiveness of the proposed DLRHyIn and R-DLRHyIn. Finally, we draw some conclusions.

___

**Requirements**:

- PyTorch 1.8
- NumPy
- SciPy
- scikit-image
- Matplotlib

___

**Getting Started:**

You just need to run `demo.ipynb` to reproduce the result on the Washington DC Mall dataset. For using your own dataset, you need to copy your dataset to the "data" folder and change the `file_name  = 'data/WDC_Painted.mat'` in the notebook.

___

This implementation is based on [[1]](https://github.com/DmitryUlyanov/deep-image-prior) and [[2]](https://github.com/acecreamu/deep-hs-prior#deep-hyperspectral-prior-single-image-denoising-inpainting-super-resolution).

