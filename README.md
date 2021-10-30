# ViX     
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/vision-xformers-efficient-attention-for-image/image-classification-on-cifar-10)](https://paperswithcode.com/sota/image-classification-on-cifar-10?p=vision-xformers-efficient-attention-for-image)
## Vision Xformers: Efficient Attention for Image Classification

We use Linear Attention mechanisms to replace quadratic attention in ViT for image classification. We show that models using linear attention and CNN embedding layers need less parameters and low GPU requirements for achieving good accuracy. These improvements can be used to democratize the use of transformers by practitioners who are limited by data and GPU.

Hybrid ViX uses convolutional layers instead of linear layer for generating embeddings

Rotary Postion Embedding (RoPE) is also used in our models instead of 1D learnable position embeddings

Nomenclature:
We replace the X in ViX with the starting alphabet of the attention mechanism used
Eg. When we use Performer in ViX, we replace the X with P, calling it ViP (Vision Performer)

'Hybrid' prefix is used in models which uses convolutional layers instead of linear embeddding layer. 

We have added RoPE in the title of models which used Rotary Postion Embedding

The code for using all for these models for classification of CIFAR 10/Tiny ImageNet dataset is provided

### Models

- Vision Transformer (ViT)
- Vision Linformer (ViL)
- Vision Performer (ViP)
- Vision Nyströmformer (ViN)
- FNet
- Hybrid Vision Transformer (HybridViT)
- Hybrid Vision Linformer (HybridViL)
- Hybrid Vision Performer (HybridViP)
- Hybrid Vision Nyströmformer (HybridViN)
- Hybrid FNet
- LeViN (Replacing Transformer in LeViT with Nyströmformer)
- LeViP (Replacing Transformer in LeViT with Performer)
- CvN (Replacing Transformer in CvT with Nyströmformer)
- CvP (Replacing Transformer in CvT with Performer)
- CCN (Replacing Transformer in CCT with Nyströmformer)
- CCP(Replacing Transformer in CCT with Performer)

We have adapted the codes for ViT and linear transformers from @lucidrains 

More information about these models can be obtained from our paper : https://arxiv.org/abs/2107.02239

If you wish to cite this paper please use:
```
@misc{jeevan2021vision,
      title={Vision Xformers: Efficient Attention for Image Classification}, 
      author={Pranav Jeevan and Amit Sethi},
      year={2021},
      eprint={2107.02239},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
