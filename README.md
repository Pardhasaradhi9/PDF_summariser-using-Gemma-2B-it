# PDF Summarizer using Gemma-2B-IT

A PDF summarizer created using the open model LLM (Gemma-2B-IT) that runs locally on M1-Apple Silicon.

## Overview

Gemma: Open Models Based on Gemini Research and Technology. This LLM model consists of 2 models: 2B & 7B, which were trained on up to 6T tokens. When it was released, I wanted to run these models locally on my Apple Silicon. So, in this project, I've used the quantized version of Gemma-2B-IT to create a PDF summarizer using MLX. Thanks to "prince-canuma" for contributing this model to the MLX community on Hugging Face. Using the model "mlx-community/quantized-gemma-2b-it," I was able to create a PDF summarizer that runs locally on Apple Silicon.

The results produced by Gemma-2B-IT are very impressive, and I can't wait to create many more projects using "Gemma."

## Shoutout

A big shoutout to "prince-canuma" for his contribution to the MLX community. Do check out his other models as well.

## How This Project Works

### Installation

To install the necessary dependencies, run:

### The code explains the process i followed to create this summariser 

### Usage Summary:
- Load the Model and Tokenizer: Initialize the Gemma-2B-IT model and tokenizer.
- Load and Split the PDF Document: Use PyPDFLoader and RecursiveCharacterTextSplitter to load and split the PDF into chunks.
- Generate Summaries: Apply a chat template to generate summaries for the specified sections.
- Clean and Combine Summaries: Clean the generated summaries and combine them into a cohesive document.
- Rewrite the Combined Summary: Rewrite the combined summary to ensure it is grammatically correct and cohesive.
