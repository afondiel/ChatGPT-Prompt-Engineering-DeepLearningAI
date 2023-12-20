# Lesson 1: Introduction

## Overview

- A lot of material on the internet for prompting has been focused on the chatGPT `web user interface`, which many people are using to do specific and often one-off tasks
- The power of LLMs (Large Language Models), as a developer tool, that is using `API` calls 
- LLM APIs can enable developers to very quickly build software applications
  
## Course Plan

- Prompting best practices for software development 
- Some common `use cases` :  
  - summarizing 
  - inferring
  - transforming
  - expanding 
- Build a chatbot using an LLM

## Two types of LLMs

- `Base LLMs` : predicts next words, based on text training data (huge amount of text data from internet and another sources) to figure it out most likely word to follow
  - Ex : `what is the capital of France?`
    - What is France's largest city?
    - What is France's population?
    - What is the currency of France?
- `Instruction Tuned LLMs` : 
  - Tries to follow instructions. 
  - Fine-tune on instructions(input/outputs) and good attempts at following those instructions
  - Uses Reinforcement Learning with Human Feedback (RLHF) technique
  - Trained to be : Helpful, Honest , Harmless, safe*

    - Ex: `what is the capital of France?`
      - The capital of France is Paris

## TL;DR

The 6 Prompt engineering strategies to get the best results from Large Language Models (LLMs):

1. Write clear instructions
2. Provide reference text
3. Split complex tasks into simpler subtasks
4. Give the model time to "think”
5. Use external tools
6. Test changes systematically

## References

Main Course : 
- https://learn.deeplearning.ai/chatgpt-prompt-eng/lesson/1/introduction

Model index for researchers - openai: 
- https://platform.openai.com/docs/model-index-for-researchers/model-index-for-researchers

Generative Pre-trained Transformer Models : 

- GPT-1 : https://en.wikipedia.org/wiki/Generative_pre-trained_transformer
- GPT-2 : https://en.wikipedia.org/wiki/GPT-2 
  - paper : https://arxiv.org/ftp/arxiv/papers/1908/1908.09203.pdf
- GPT-3 : https://en.wikipedia.org/wiki/GPT-3
  - paper : https://arxiv.org/pdf/2005.14165.pdf
- GPT-4 :  https://en.wikipedia.org/wiki/GPT-4
  - paper : https://arxiv.org/pdf/2303.08774.pdf

- Codex : 
  - paper : https://arxiv.org/pdf/2107.03374.pdf
- InstructGPT (ChatGPT ancestor) : 
  - paper : https://arxiv.org/pdf/2203.02155.pdf

GPT Best Practices - openai : 
- https://platform.openai.com/docs/guides/gpt-best-practices 

What are Generative AI models? - IBM
- https://www.youtube.com/watch?v=hfIUstzHs9A

**Cohere** - Transform your products with LLMs : https://cohere.com/

**Langchains** : https://python.langchain.com/docs/get_started/introduction.html


**huggingface** - The AI community building the future - https://huggingface.co/

**anthropic** - AI research and products that put safety at the frontier
https://www.anthropic.com/

