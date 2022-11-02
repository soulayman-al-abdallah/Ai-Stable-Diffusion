# Ai art generation using Stable Diffusion, with detailed explanation


**Stable Diffusion** is a text-to-image latent diffusion model created by the researchers and engineers from [CompVis](https://github.com/CompVis), [Stability AI](https://stability.ai/) and [LAION](https://laion.ai/). It's trained on 512x512 images from a subset of the [LAION-5B](https://laion.ai/blog/laion-5b/) database. This model uses a frozen CLIP ViT-L/14 text encoder to condition the model on text prompts. With its 860M UNet and 123M text encoder, the model is relatively lightweight and runs on a GPU with at least 10GB VRAM.
See the [model card](https://huggingface.co/CompVis/stable-diffusion) for more information.

This colab is inspired and adabted from the official notebook implementing Stable Diffusion by Hugging Face [here](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/stable_diffusion.ipynb), and the work done in this [video](https://www.youtube.com/watch?v=ltLNYA3lWAQ&t=413s&ab_channel=EdanMeyer).


What we do in this colab:
* **Text-2-Image** generation using a **ready-to-use** pipeline
* Understanding the parameters that lead to output variation
* **Text-2-Image** generation using a **customized** pipeline
* Visualizing the image denoising via a video
* Generating **similar images** by changing the latents
* **Image-2-Image** generation by fixing the original latents and listening to a prompt


---------------------------------------------------------------------------------------------
![download (4)](https://user-images.githubusercontent.com/75330691/199470322-27e86cb1-d189-4ad6-84de-b77168b22702.png)

---------------------------------------------------------------------------------------------
<p float="left">
  <img src="https://user-images.githubusercontent.com/75330691/199470605-9f07f8c2-970f-4e66-a2f3-fb1f9e303a8d.png" width="350" />
  <img src="https://user-images.githubusercontent.com/75330691/199470849-824ee6a0-c6e0-4c0b-8113-94fe482c350d.png" width="350" /> 
</p>

---------------------------------------------------------------------------------------------

<p float="left">
  <img src="https://user-images.githubusercontent.com/75330691/199471530-33170bf6-f0fe-46bb-8b9e-32a740c1b3b8.png" width="350" /> 
  <img src="https://user-images.githubusercontent.com/75330691/199469962-88ec0f90-cb01-4935-9628-9d4f5d7f8f66.png" width="350" />
</p>

