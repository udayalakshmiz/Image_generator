**Diffusion Image Generator**

A simple **Text-to-Image Generation Web App** built using **Stable Diffusion**, **Hugging Face Transformers**, and **Gradio**.

This project allows users to generate high-quality images from natural language prompts and download them directly from the interface.

**Features**

* Generate images from text prompts
* Uses **Stable Diffusion v1.4**
* Interactive UI built with **Gradio**
* Supports GPU acceleration (CUDA)
* Download generated images
* Easy to use and beginner-friendly

**Tech Stack**

* Python
* PyTorch
* Hugging Face Transformers
* Diffusers
* Gradio
* PIL (Python Imaging Library)

**Installation**

Install required libraries:

```bash
pip install transformers diffusers gradio torch pillow
```

**Usage**

**Option 1: Run in Google Colab**

1. Open the notebook in Google Colab
2. Run all the cells step by step
3. Enter a text prompt
4. Generate and download the image

**Option 2: Run locally (optional)**

1. Convert the notebook into a Python file (`app.py`)
2. Run:

```bash
python app.py
```

3. Open the Gradio link in your browser

**How It Works**

1. User enters a text prompt
2. The prompt is processed using a tokenizer
3. Stable Diffusion generates an image using:

   * VAE (Variational Autoencoder)
   * UNet model
   * Scheduler (PNDM)
4. The generated image is displayed in the UI
5. User can download the generated image

**Example Prompts**

* "A futuristic city at sunset"
* "A dragon flying over mountains"
* "A robot painting a portrait"
  
**Requirements**

* Python 3.8+
* CUDA-enabled GPU (recommended for faster generation)

**Notes**

* First run may take time (model download ~4GB)
* Works on CPU but slower
* Ensure enough RAM/VRAM is available

**Project Structure**

│── diffusion_image_generator.ipynb

│── README.md

│── requirements.txt

**Future Improvements**

* Add multiple image generation options
* Improve UI design
* Add prompt history
* Deploy using Hugging Face Spaces

**Contributing**

Feel free to fork this repository and improve it!

**License**

This project is open-source and available under the MIT License.

**Acknowledgements**

* Hugging Face
* Stability AI (Stable Diffusion)

---
