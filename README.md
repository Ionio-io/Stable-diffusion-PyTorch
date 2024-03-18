# Stable-Diffusion
### Overview
Welcome to the Stable Diffusion PyTorch repository! This project leverages the power of PyTorch to implement the Stable Diffusion model, enabling high-quality image generation from textual descriptions. Built with efficiency and scalability in mind, our implementation supports various customizations and advanced features, making it suitable for both research and practical applications.

### Features
- High-quality image generation with Stable Diffusion
- Support for custom prompts and image editing
- Efficient PyTorch implementation optimized for GPU acceleration
- Extensible architecture for further customization and research
  
### Prerequisites
Before you begin, ensure you have the following installed:

- Python 3.8 or newer
- PyTorch 1.8 or newer
- CUDA Toolkit (for GPU acceleration)
- Other dependencies listed in requirements.txt
  
### Installation
To set up the project, follow these steps:<br>

Clone the repository:<br>

```
git clone https://github.com/Ionio-io/Stable-diffusion-PyTorch.git
cd Stable-diffusion-PyTorch
```
#### Install the required Python packages:

```
pip install -r requirements.txt
```

### Download weights and tokenizer files:
- Download `vocab.json` and `merges.txt` from https://huggingface.co/runwayml/stable-diffusion-v1-5/tree/main/tokenizer and save them in the data folder
- Download `v1-5-pruned-emaonly.ckpt` from https://huggingface.co/runwayml/stable-diffusion-v1-5/tree/main and save it in the data folder
  
#### Usage
To generate images with Stable Diffusion, use the following command:

```
python generate.py --prompt "A text description of the image you want to generate"
```

Advanced Options <br>
`--uncond_prompt`: Specify an unconditional prompt for more abstract generations. <br>
`--strength`: Control the influence of the conditional prompt on the generated image. <br>
`--n_inference_steps`: Specify the number of diffusion steps. <br>
Refer to `pipeline.py` for more details and options. <br>

### Customization
This implementation allows for easy customization and extension. You can modify the generation parameters, integrate new models, or experiment with different diffusion techniques by editing the corresponding Python scripts.

### License
This project is released under the MIT License. See LICENSE for more details.

### Acknowledgments
Special thanks to the original creators of the Stable Diffusion model and the PyTorch community for their invaluable resources and support.
