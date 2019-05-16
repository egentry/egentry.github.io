---
title: "Galaxy cGAN"
excerpt: "Creating artificial galaxy images using conditional Generative Adversarial Networks<br/><img src='/files/portfolio/gan/animation.gif' width='75%'>"
collection: portfolio
date: 2018-04-01
---

**UC Santa Cruz, Theoretical Astrophysics**

A Generative Adversarial Network that generates images of galaxies for an input redshift and stellar mass. The motivation for this project is to develop a GAN that can create infinitely many, diverse training images for use in training a different classifier deep neural network. Inspired by work such as this paper by a team of researchers at Apple: [Learning Simulated and Unsupervised Images through Adversarial Training](https://arxiv.org/abs/1612.07828)

Unfortunately while the GAN _often_ gave realistic-looking images, there were key areas of the input (conditional) parameter space which led to non-physical images. As a result, the GAN is not yet helpful in training other neural networks. Two places to try to improve this would be by improving the "critic" network within the GAN to focus on those areas of parameter space more heavily, or to include more conditioning data (like a lower dimensional representation of the image, such as an auto-encoder's latent representation, rather than just the 2 numbers of distance and mass).

Code: [`galaxyCGAN`](https://github.com/egentry/galaxyCGAN)

Report: [GANs for Data Augmentation](https://docs.google.com/document/d/1b_hhbJe1BeYTPs-bdPF380XTENkypS9nfCQ3_uJaBXo/edit?usp=sharing)

[Presentation](https://docs.google.com/presentation/d/1xjLsMAiMoyPivnso6r9iNnvczVzGpb6Xe3NvX4osrRk/edit?usp=sharing)

Example of the different images generated, conditional on the total stellar mass of the galaxy:
<img src="/files/portfolio/gan/animation.gif"  width="80%"/>
