---
title: "Stable Diffusion"
feed: show
date: "2023-06-08"
tags: 
---

## Background
A text to image diffusion model. "AI generated art"

## Samples
prompt: *"flying yellow piper airplane sunset"*
![200](notes/software/stablediffusion/images/stable1.png)
![200](notes/software/stablediffusion/images/stable2.png)
![200](notes/software/stablediffusion/images/stable3.png)
The tri-wing is an interesting concept...How to get off the ground though?
## Details
- Open source
- Concepts/Extensions:
	- Outpainting: expanding the edges of an image
	- LORA
	- ControlNET
		- pretty QR codes
- use negative prompt for things you don't want in the image
- there is the open source plugin of stable diffusion for photoshop
- check out r/stablediffusion

### How to get it
1. stability.ai/stablediffusion
2. Check out and run locally 
3. access web server on port 127.0.0.1:7860
4. OR the playground
	1. https://stablediffusionweb.com/#demo

### Models

- huggingface
- civitai

#### Comparing Models
daniel.von-appen.org/stable-diffusion-model-comparison/

#### LORAs 
- smaller file size, easier to train on. can download a LORA for a particular style and then apply it. available as a plugin.

### Use Cases
- presentations
- icons
	- there are models for pixel art
- modifying images