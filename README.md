# GAN Image Generation Study

An educational PyTorch collection covering vanilla GAN, conditional GAN (cGAN), and DCGAN. The code, pretrained models, and examples come from the upstream project.

## Problem and approach

A generator maps latent vectors to synthetic images; a discriminator distinguishes generated samples from real data. The conditional variant adds class information, while DCGAN uses convolutional networks for image generation. Training scripts for the three variants are separate.

## Repository map

| Path | Purpose |
| --- | --- |
| `train_vanilla_gan.py`, `train_cgan.py`, `train_dcgan.py` | Training entry points |
| `models/`, `utils/` | Network definitions and supporting code |
| `generate_imagery.py` | Generate examples from upstream pretrained models |
| `data/examples/` | Existing samples, interpolation images, and training GIFs |
| `Vanilla GAN (PyTorch).ipynb` | Exploratory notebook |

## Existing upstream outputs

![Upstream DCGAN and other examples](data/examples/generated_samples/generated_vgan.jpg)

The repository includes sample images and training progress GIFs under `data/examples/`, plus pretrained models described in the [original documentation](UPSTREAM_README.md). These are upstream artifacts; no training or new evaluation was performed for this fork.

## Explore

Create the environment with `conda env create -f environment.yml`, then inspect `generate_imagery.py` for the generation options. See the original documentation for model-specific commands and examples.

## Source and license

Based on and adapted from [gordicaleksa/pytorch-GANs](https://github.com/gordicaleksa/pytorch-GANs). The [original README](UPSTREAM_README.md), original source files, and [MIT license](LICENCE) are retained. All example images and weights are credited to the upstream project.