# AI-VISION


A complete AI-powered system designed to bridge the gap between visual media and accessibility. This project converts uploaded images into detailed text descriptions and speaks them out loud in audio format, serving as an assistive technology for visually impaired individuals.

Project Overview
Visual content is often inaccessible to people with vision loss. This tool solves that by automatically analyzing any image, extracting its context, translating it into Georgian, and synthesizing audio output.

How It Works
Visual Scene Understanding: The model inspects the image and generates a descriptive text summary in English.

Translation Pipeline: Converts the generated text into natural-sounding Georgian.

Speech Synthesis: Generates audio playback from the text description.

Interactive Web App: A simple UI built with Gradio where users can upload any image and get real-time text and audio outputs.

Technical Architecture & Workflow
The system is built as a sequential multi-stage pipeline combining modern Computer Vision and Natural Language Processing (NLP) frameworks:

Image Captioning & Scene Analysis: Uses Google's Gemini multimodal model as a backbone for primary scene recognition, extended with custom feature-extraction functions to deliver deeper, more fine-grained contextual descriptions.

Model Testing & Benchmarking: Evaluated on the COCO (Common Objects in Context) dataset across a sample size of 100 images, alongside training insights from Flickr30k.

Language Translation: Uses the deep-translator library to translate the detailed English descriptions into accurate Georgian.

Audio Generation: Integrates Google Vertex AI Text-to-Speech (TTS) capabilities to convert text into speech.

Interface & Deployment: Wrapped into an interactive demo using Gradio, allowing direct image input and rendering both English and Georgian captions alongside the generated audio track.
