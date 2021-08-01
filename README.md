# ViX
## Vision Xformers: Efficient Attention for Image Classification

We use Linear Attention mechanisms to replace quadratic attention in ViT for image classification. 

Hybrid ViX uses convolutional layers instead of linear layer for generating embeddings

Rotary Postion Embedding (RoPE) is also used in our models instead of 1D learnable position embeddings

Nomenclature:
We replace the X in ViX with the starting alphabet of the attention mechanism used
Eg. When we use Performer in ViX, we replace the X with P, calling it ViP (Vision Performer)

'Hybrid' prefix is used in models which uses convolutional layers instead of linear embeddding layer. We have added CNN in the title for hybrid models

We have added RoPE in the title of models which used Rotary Postion Embedding

The code for using all for these models for classification of CIFAR 10 dataset is provided

### Models

- Vision Transformer (ViT)
- Vision Linformer (ViL)
- Vision Performer (ViP)
- Vision Nyströmformer (ViN)
- Hybrid Vision Transformer (ViT)
- Hybrid Vision Linformer (ViL)
- Hybrid Vision Performer (ViP)
- Hybrid Vision Nyströmformer (ViN)

We have adapted the codes for ViT and linear transformers from @lucidrains 

If you wish to cite this paper please use:

@misc{jeevan2021vision,
      title={Vision Xformers: Efficient Attention for Image Classification}, 
      author={Pranav Jeevan and Amit Sethi},
      year={2021},
      eprint={2107.02239},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
