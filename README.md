# Analysing Contemporary Diffusion Models for Generating Images

**Bachelor's Thesis**

## Abstract

Diffusion models have recently demonstrated powerful synthesis capabilities for various types of data, including images. Producing highly realistic samples and introducing a guidance mechanism to control the generation process, these models have initiated new areas of research. The latter includes an ongoing field of study focused on utilizing pre-trained diffusion models to modify real images with consideration to a given textual prompt. Although existing methods have shown considerable results, they still require thorough investigation. In this paper, we analyse a recently introduced approach, Null-Text Inversion for Editing Real Images using Guided Diffusion Models, and propose significant improvements, targeting its challenging domains.

## Code base

This repository provides the code, written and used while working on the thesis.

Our work heavily relies on the authors' implementation of Null-text Inversion with Prompt-to-Prompt: [source](https://github.com/google/prompt-to-prompt/#null-text-inversion-for-editing-real-images)

## Structure

Refer to the folder `notebooks`.

### Base approaches

- ```null_text_w_ptp.ipynb```

  reproducing results of Null-text Inversion with Prompt-to-Prompt: [paper](https://arxiv.org/abs/2211.09794)

- ```imagic.ipynb```

  our implementation of Imagic: [paper](https://arxiv.org/abs/2210.09276)

### Null-text Inversion with Learned Embedding

- ```null_text_imagic.ipynb```

  basic version
	
- ```null_text_imagic_e_opt_regularization.ipynb```

  with regularization in embedding optimization

- ```null_text_imagic_interpolation_step.ipynb```

  with interpolation steps

- ```null_text_imagic_interpolation_step_and_reg.ipynb```

  with regularization and interpolation steps

### Null-text Inversion with Null-text Embeddings Finetuning

- ```null_text_null_embeds_for_tgt_prompt.ipynb```
