# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Environment Setup

This repository uses Python 3.11 and contains LLM/AI experimentation notebooks. Dependencies can be installed using either:

- **Conda environment**: `conda env create -f environment.yml`
- **pip requirements**: `pip install -r requirements.txt`

Both methods install the same core dependencies including PyTorch, Transformers, LangChain, OpenAI, Anthropic, and Google Generative AI libraries.

## Project Structure

The `src/` directory contains Jupyter notebooks for different AI experiments:

- `generate_image.ipynb`: DALL-E 3 image generation using OpenAI API
- `new_testament_expert.ipynb`: Multi-model chatbot comparing GPT-4o-mini and Claude responses with biblical expertise

## Environment Variables

Create a `.env` file with API keys:
- `OPENAI_API_KEY`: Required for image generation and GPT models
- `ANTHROPIC_API_KEY`: Required for Claude models  
- `GOOGLE_API_KEY`: Required for Google Generative AI models

## Running Notebooks

Launch JupyterLab: `jupyter lab`

The notebooks are designed to be run interactively and include Gradio interfaces for web-based interaction with the models.

## Development Commands

- Start Jupyter: `jupyter lab`
- Install dependencies: `conda env create -f environment.yml` or `pip install -r requirements.txt`
- Activate conda environment: `conda activate llms`