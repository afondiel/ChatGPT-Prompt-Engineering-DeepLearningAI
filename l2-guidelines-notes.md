# Lesson2: Guidelines


## Principles of Prompting

- `Principle 1` : write clear and specific instructions
- `Principle 2` : give the model time to "think"     

### Pinciple 1 - Tactics :  

#### Tactic 1: Use delimiters to clearly indicate distinct parts of the input
- Delimiters can be anything like: 
  - Triple backticks : ```, 
  - Triple quotes: """,
  - Triple dashes:  ---,  
  - Angle brackets : < >, 
  - XML Tags : `<tag> </tag>`, 
  - colons `:` 

- Using delimiters is also a helpful technique to try and avoid `prompt injections`

- Check the example in the guideline [notebook](./lab/l2-guidelines.ipynb)

#### Tactic 2: Ask for a structured output
- JSON, HTML

- Check the example in the guideline [notebook](./lab/l2-guidelines.ipynb)

#### Tactic 3: Ask the model to check whether conditions are satisfied
- Check the example in the guideline [notebook](./lab/l2-guidelines.ipynb)

#### Tactic 4: "Few-shot" prompting
- Check the example in the guideline [notebook](./lab/l2-guidelines.ipynb)

### Pinciple 2 - Tactics :  
- Check the example in the guideline [notebook](./lab/l2-guidelines.ipynb)

#### Tactic 1: Specify the steps required to complete a task
- Check the example in the guideline [notebook](./lab/l2-guidelines.ipynb)

#### Tactic 2: Instruct the model to work out its own solution before rushing to a conclusion
- Check the example in the guideline [notebook](./lab/l2-guidelines.ipynb)


## Model Limitations: Hallucinations
- Boie is a real company, the product name is not real.

```python
prompt = f"""
Tell me about AeroGlide UltraSlim Smart Toothbrush by Boie
"""
response = get_completion(prompt)
print(response)
```

`Completion`:

```text
The AeroGlide UltraSlim Smart Toothbrush by Boie is a high-tech toothbrush that uses advanced sonic technology to provide a deep and thorough clean. It features a slim and sleek design that makes it easy to hold and maneuver, and it comes with a range of smart features that help you optimize your brushing routine.
```


## References

Main Course : 
- https://learn.deeplearning.ai/chatgpt-prompt-eng/lesson/2/guidelines

GPT Best Practices - openai : 
- https://platform.openai.com/docs/guides/gpt-best-practices 

API Reference :
- https://platform.openai.com/docs/api-reference/introduction



