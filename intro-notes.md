#  Introduction - Notes

## Overview

- A lot of material on the internet for prompting has been focused on the chatGPT `web user interface`, which many people are using to do specific and often one-off tasks
- The power of LLMs (Large Language Models), as a developer tool, that is using `API` calls 
- LLM APIs can enable developers to very quickly build software applications
  
## Course Plan 
- Some prompting best practices for software development 
- Some common `use cases` :  
  - summarizing 
  - inferring
  - transforming
  - expanding 
- Build a chatbot using an LLM

## Two types of LLMs

- `Base LLMs` : predicts next words, based on text training data
  - Ex : `what is the capital of France?`
    - What is France's largest city?
    - What is France's population?
    - What is the currency of France?
- `Instruction Tuned LLMs` : Tries to follow instructions. Fine-tune on instructions and good attempts at following those instructions
  - Ex: `what is the capital of France?`
    - The capital of France is Paris
  
  - Base LLM + instruction fine-tuning (input/outputs)
  - Instruction Tuned LLMs uses Reinforcement Learning with Human Feedback (RLHF) technique
  - trained to be : Helpful, Honest , Harmless, safe*


# References

Main Course : 
- https://learn.deeplearning.ai/chatgpt-prompt-eng/lesson/1/introduction
