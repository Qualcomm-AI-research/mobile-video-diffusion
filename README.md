This repository contains the code for a GitHub pages site for the publication [Mobile Video Diffusion](http://arxiv.org/abs/2412.07583). The project page is hosted at https://qualcomm-ai-research.github.io/mobile-video-diffusion/.

This paper introduces the first mobile-optimized video diffusion model. By optimizing the spatio-temporal UNet from Stable Video Diffusion (SVD), we reduce memory and computational requirements. We achieve this by lowering the resolution to 512x256 px, incorporating multi-scale temporal representations, and introducing two novel pruning schema to reduce the number of channels and temporal blocks in the UNet. Furthermore, we employ adversarial finetuning to reduce the denoising to a single step. Our model, MobileVD, is 523x more efficient (1817.2 vs. 4.34 TFLOPs) with a slight quality drop (FVD 149 vs. 171), generating latents for a 14x512x256 px clip in 1.7 seconds on a Xiaomi-14 Pro.