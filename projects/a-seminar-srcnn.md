---
layout: post
title: Image Super Resolution using CNN - in Lasagne on jupyter notebook
thumbnail: img/seminar-srcnn.png
buttons:
  - CODE: https://github.com/BardOfCodes/SRCNN-Lasagne-Jupyter-Notebook
  - LATEX: https://www.overleaf.com/read/wtrfhfgykrbf
  - PDF: ../../pdf/seminar-srcnn.pdf
category: Stochastic
excerpt: For my Final-Year Seminar I reviewed the paper "Image Super-Resolution Using Deep Convolutional Networks" and made a narrative code in jupyter notebook implementing the SRCNN.
type: project
date: 2016/10/25
featured: true
anchors:
  - Introduction: introduction
  - Introduction to Image Super-Resolution: introduction-to-image-super-resolution
  - The Model: the-model
  - Training: training
  - Links: links
---
### Introduction
 For my Final-Year Seminar I reviewed the paper "Image Super-Resolution Using Deep Convolutional
 Networks" and made a narrative code in jupyter notebook implementing the SRCNN. I also made a
 presentation, where I talk about the regularization theory, and this paper. My super-ambitious plan
 was to work towards extending the Regularization theory to Image Super-resolution.

This is a notebook on theano based Image-super resolution based on this [paper](https://arxiv.org/abs/1501.00092).
This implementation is based on the implementation of ['corochann'](https://github.com/corochann).
The original codes of this implementation can be found [here](https://github.com/corochann/theanonSR).
The images used have been taken from [here](https://github.com/jbhuang0604/SelfExSR)
This is all work of the original authors of the papers. The purpose of this notebook is only to make the process
easier to comprehend and give a toy example of how to implement it.

### Introduction to Image Super-Resolution

Single image super-resolution (SR), which aims at recovering a high-resolution image from a
single low-resolution image, is a classical problem in computer vision. This problem is inherently
ill-posed since a multiplicity of solutions exist for any given low-resolution pixel.

Such a problem is typically mitigated by constraining the solution space by strong prior information.
To learn the prior,recent state-of-the-art methods mostly adopt example-based strategy. These methods
either exploit internal similarities of the same image or learn mappingfunctions from external
low- and high-resolution exemplar pairs.

In this paper a Deep Convolutional Neural Network has been developed to solve this problem.
The proposed Super-Resolution-convoluted-neural-network, SRCNN, has several appealing properties.
First, its structure is intentionally designed with simplicity in mind, and yet provides superior
accuracy.Secondly, with morderate numbers of filters and layers, this method achieves fast speed
for practical on-line usage even on a CPU.

### The model

Consider a single low-resolution image, we first upscale it to the desired size using bicubic
interpolation, which is the only pre-processing we perform. Let us denote the interpolated
image as $$Y$$. Our goal is to recover from $$Y$$ an image $$F(Y)$$ that is as similaras possible
to the ground truth high-resolution image $$X$$. For the ease of presentation, we still call
$$Y$$ a “low-resolution” image, although it has the same size as $$X$$. We wish to learn a
mapping $$F$$, which conceptually consists of three operations:

1) <b>Patch extraction and representation:</b> this operation extracts (overlapping) patches from the
low-resolution image $Y$ and represents each patch as a high-dimensional vector. These vectors
comprise a set of feature maps, of which the number equals to the dimensionality of the
vectors.

2) <b>Non-linear mapping:</b> this operation nonlinearly maps each high-dimensional vector
onto another high-dimensional vector. Each mapped vector is conceptually the representation
of a high-resolution patch. These vectors comprise another set of feature maps.

3) <b>Reconstruction:</b> This operation aggregates the above high-resolution patch-wise
representations to generate the final high-resolution image. This image is expected to be
similar to the ground truth $$X$$.

<img src ="../../img/seminar-srcnn.png" style="margin-left:auto;margin-right:auto;" />

This can be mathematically be represented as

1)

$$
\begin{equation}
F_1 (Y) = max(0,W_1*Y +B_1)
\end{equation}
$$

where $$W_1$$ and $$B_1$$ represent the filters and biases respectively, and ’*’ denotes
the convolution operation. Here, $$W_1$$ corresponds to $$n_1$$ filters of support $$c\times f_1 \times f_1$$,
where $$c$$ is the number of channels in the input image, $$f_1$$ is the spatial size of a
filter.

2)

$$
\begin{equation}
F_2 (Y) = max(0,W_2*F_1(Y) +B_2)
\end{equation}
$$

Here, $$W_2$$ contains $$n_2$$ filters of size $$n_1\times f_2 \times f_2$$, and $$B_2$$ is
$$n_2$$-dimensional.

3)

$$
\begin{equation}
F(Y) = W_3*F_2(Y) +B_3
\end{equation}
$$

Here $$W_3$$ corresponds to $$c$$ filters of a size $$n_2 \times f_3\times f_3$$, and $$B_3$$
is a $$c$$-dimensional vector.

### Training

Learning the end-to-end mapping function $$F$$ requires the estimation of network parameters $$\Theta = \{ W_1;W_2;W_3;B_1;B_2;B_3\} $$.
This is achieved through min-imizing the loss between the reconstructed images $$F(Y; \Theta)$$
and the corresponding ground truth high-resolution images $$X$$. Given a set of high-resolution
images $$\{Xi\}$$ and their corresponding low-resolution images $$\{Yi\}$$, we use Mean Squared
Error (MSE) as the loss function:


$$
\begin{equation}
L(\Theta) = \frac{1}{n} \sum_{i=1}^{n}{ {|| F(Y_i,\Theta) - X_i ||}^2},
\end{equation}
$$


where $$n$$ is the number of training samples

### Links

The code for simulation of the solution has been written in python.You can,

* Download the code from [here](https://github.com/BardOfCodes/SRCNN-Lasagne-Jupyter-Noteboo)

* Download the Presentation PDF [here](../../pdf/seminar-srcnn.pdf)

* View the Latex files [here](https://www.overleaf.com/read/wtrfhfgykrbf)
