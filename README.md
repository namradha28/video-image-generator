# 🎬 AI Image & Video Generation with Colab + Gradio

A Generative AI project that enables **Text-to-Image** and **Text-to-Video** generation using Stable Diffusion models on Google Colab with an interactive Gradio interface.

This project leverages GPU acceleration in Colab to generate high-quality images and short videos from natural language prompts.

---

## 🚀 Live Demo

Run the notebook in Google Colab and generate a public Gradio link:

Runtime → Change runtime type → GPU  
Run all cells → Click the generated public URL  

---

## 📌 Project Overview

This project allows users to:

- 🖼️ Generate images from text prompts
- 🎬 Generate short videos from text prompts
- 🌐 Share results via public Gradio link
- ⚡ Use GPU acceleration without local setup

It demonstrates practical implementation of diffusion models in a cloud-based environment.

---

## 🏗️ Architecture

User Prompt
    ↓
Stable Diffusion Model (Diffusers)
    ↓
Generated Image / Video Frames
    ↓
Gradio Interface
    ↓
Public Shareable Link

---

## ⚙️ Tech Stack

- Python 3.x
- Google Colab (GPU: T4)
- Hugging Face Diffusers
- Transformers
- PyTorch
- Gradio
- ImageIO (for video export)

---

## 📂 Project Structure

image-video-generation/
│
├── image_app.py
├── video_app.py
├── requirements.txt
└── README.md

(Or implemented directly inside a Colab Notebook)

---

## 🖼️ Text-to-Image Generation

Model Used:
runwayml/stable-diffusion-v1-5

### How It Works

1. Load Stable Diffusion model
2. Move model to GPU
3. Pass prompt into pipeline
4. Return generated image
5. Display via Gradio UI

Example Prompt:

A futuristic cyberpunk city at night, neon lights reflecting on wet streets, cinematic wide shot, ultra detailed, 4K, smooth lighting

---

## 🎬 Text-to-Video Generation

Model Used:
damo-vilab/text-to-video-ms-1.7b

### How It Works

1. Load text-to-video diffusion pipeline
2. Generate sequence of frames
3. Convert frames to MP4 using ImageIO
4. Display video in Gradio interface

Example Prompt:

A majestic dragon flying over snowy mountains at sunrise, cinematic camera pan, dramatic lighting, ultra realistic, 4K, smooth motion

---

## 🖥️ Running on Google Colab

### Step 1: Enable GPU

Runtime → Change runtime type → GPU (T4 recommended)

### Step 2: Install Dependencies
!pip install diffusers transformers accelerate torch gradio imageio imageio-ffmpeg


### Step 3: Run the Notebook
Execute all cells and launch Gradio:


A public link will be generated.

---

## 📦 requirements.txt

diffusers  
transformers  
accelerate  
torch  
gradio  
imageio  
imageio-ffmpeg  

---

## 🎯 Key Features

- GPU-powered generation
- Interactive UI with Gradio
- Public shareable link
- Image and video support
- Cloud-based execution (no local GPU required)
- Modular architecture

---

## 💡 Future Improvements

- LoRA Fine-Tuning
- ControlNet Integration
- Image-to-Image Transformation
- Prompt Enhancement using LLM
- Deployment on Hugging Face Spaces
- Custom Model Hosting

---



