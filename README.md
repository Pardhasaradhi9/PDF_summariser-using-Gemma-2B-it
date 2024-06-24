# PDF Summarizer using Gemma-2B-IT

A PDF summarizer created using the open model LLM (Gemma-2B-IT) that runs locally on M1-Apple Silicon.

## Overview

Gemma: Open Models Based on Gemini Research and Technology. This LLM model consists of 2 models: 2B & 7B, which were trained on up to 6T tokens. When it was released, I wanted to run these models locally on my Apple Silicon. So, in this project, I've used the quantized version of Gemma-2B-IT to create a PDF summarizer using MLX. Thanks to "prince-canuma" for contributing this model to the MLX community on Hugging Face. Using the model "mlx-community/quantized-gemma-2b-it," I was able to create a PDF summarizer that runs locally on Apple Silicon.

The results produced by Gemma-2B-IT are very impressive, and I can't wait to create many more projects using "Gemma."

## Shoutout

A big shoutout to "prince-canuma" for his contribution to the MLX community. Do check out his other models as well.

## How This Project Works

### Features

- Load and split PDF documents into manageable chunks.
- Generate summaries for specified sections of the PDF.
- Clean and combine generated summaries into a cohesive document.
- Rewrite the combined summary to ensure grammatical correctness and continuity.

### Installation

To install the necessary dependencies, run:

### The code explains the process i followed to create this summariser 

### Usage Summary:
1) Load the Model and Tokenizer: Initialize the Gemma-2B-IT model and tokenizer.
2) Load and Split the PDF Document: Use PyPDFLoader and RecursiveCharacterTextSplitter to load and split the PDF into chunks.
3) Generate Summaries: Apply a chat template to generate summaries for the specified sections.
4) Clean and Combine Summaries: Clean the generated summaries and combine them into a cohesive document.
5) Rewrite the Combined Summary: Rewrite the combined summary to ensure it is grammatically correct and cohesive.
