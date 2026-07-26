# improving-ai-svg-understanding

Exploring methods to enhance AI's ability to understand and generate accurate SVGs for diagrams, icons, and progression visuals like leveling castles.

## Overview

AIs often struggle with SVGs because they are code rather than images. Long coordinate paths and complex structures get fragmented across tokens, leading to inaccurate or broken outputs. This project collects and experiments with techniques to improve that.

## Key Techniques

### 1. Fine-tuning on SVG-Text Pairs
Train a model on paired examples of natural language descriptions and corresponding SVG code. This teaches the model the direct mapping between intent and vector output.

### 2. Chain-of-Thought Prompting
Break down diagram creation into explicit reasoning steps: identify shapes, define coordinates, assemble paths, add styling. This guides the model through structured generation instead of one-shot output.

### 3. Structured Intermediate Formats
Convert SVGs to JSON or other hierarchical representations before processing. This makes the data more token-friendly and easier for the model to parse and manipulate.

### 4. Hybrid Approaches
Combine the above: use structured JSON for reasoning, then render to final SVG. Or fine-tune with chain-of-thought examples.

### 5. Tool-Augmented Generation
Let the model output high-level instructions that are executed by a reliable SVG rendering library, reducing direct code errors.

## Project Goals
- Document and benchmark these methods
- Build datasets of SVG-text pairs for common diagrams and icons
- Create progression visuals (e.g., castle levels) as clean, editable vectors
- Share reproducible experiments and results

## Getting Started
Clone the repo and start adding your datasets or experiment notebooks. Contributions welcome!