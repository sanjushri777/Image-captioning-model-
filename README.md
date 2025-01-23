

# **Stable Diffusion Image Generator with Gradio**

This project allows you to generate images using the **Stable Diffusion** model. By providing a text prompt, you can create detailed images powered by artificial intelligence.

## **Features**:
- **Text-to-Image Generation**: Generate images from text prompts.
- **User Control**: Adjust the number of inference steps and guidance scale for finer control over the generated image quality.
- **Interactive Interface**: A Gradio web interface for easy use.

## **Requirements**:
- Python 3.x
- PyTorch (with CUDA support for GPU)
- Diffusers (by Hugging Face)
- Gradio (for the interactive web interface)

Install the necessary dependencies:
```bash
pip install torch diffusers gradio
```

## **Setup**:

### 1. **Install PyTorch**:
If you haven't installed PyTorch yet, follow the installation instructions based on your system's setup:
- [PyTorch Installation Guide](https://pytorch.org/get-started/locally/)

For CUDA support (if you have an Nvidia GPU), ensure you select the correct version of CUDA.

### 2. **Clone this Repository**:
```bash
git clone https://github.com/sanjushri777/Image-captioning-model-.git
cd Image-captioning-model
```

### 3. **Run the Script**:
```bash
python app.py
```

### 4. **Gradio Web Interface**:
Once the script is running, it will launch a Gradio interface in your browser. You can input the text prompt, adjust the number of inference steps and guidance scale, and click "Generate Image" to create the image.

## **Usage**:

### Input:
- **Text Prompt**: Describe the image you'd like to generate (e.g., "A sunset over the ocean").
- **Number of Inference Steps**: Controls the number of inference steps during the image generation process. Higher values can result in more detailed images but may take longer to generate.
- **Guidance Scale**: Controls how closely the generated image follows the input prompt. A higher value increases adherence to the prompt.

### Output:
- **Generated Image**: After generating the image, it will be displayed on the interface for you to view and download.

---

## **How the Model Works**:

1. **Model Loading**: The Stable Diffusion model is loaded using the `StableDiffusionPipeline` from Hugging Face's Diffusers library.
   
2. **Image Generation**: The text prompt is fed into the model, and based on the prompt, the model generates an image.

3. **Adjustable Parameters**: You can modify the number of inference steps and guidance scale for more control over the quality and accuracy of the generated image.

---

## **Pros**:
- Create highly detailed images from simple text prompts.
- Easily adjustable settings for fine-tuning image generation.
- Fast and efficient with GPU support (CUDA enabled).

## **Cons**:
- The model requires a decent GPU for optimal performance.
- Image generation time can increase with higher inference steps.

---

## **License**:
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
