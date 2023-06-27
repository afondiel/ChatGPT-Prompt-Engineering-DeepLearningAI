# ChatGPT Prompt Engineering by DeepLearning.AI


## Overview

This crash & free course on ChatGPT Prompt Engineering is offered by [DeepLearning.AI](https://learn.deeplearning.ai/chatgpt-prompt-eng/lesson/1/introduction) and lectured by `Andrew Ng` and `Isa Fulford` from [openai](openai.com).

## Course Plan

- [Lesson1: Introduction](./l1-intro-notes.md)
- [Lesson2: Guidelines](./l2-guidelines-notes.md)
- [Lesson3: Iterative](./l3-iterative-prompt-dev.md)
- [Lesson4: Summarizing](./l4-summarizing.md)
- [Lesson5: Inferring](./l5-inferring.md)
- [Lesson6: Transforming](./l6-transforming.md)
- [Lesson7: Expanding](./l7-expanding.md)
- [Lesson8: Chatbot](./l8-chatbot.md)
- [Lesson9: Conclusion](./l9-conclusion.md)

> All notebook examples are available in the [lab](./lab/) folder.
## Setup

Load the API key and relevant Python libaries


```python
import openai
import os

from dotenv import load_dotenv, find_dotenv
_ = load_dotenv(find_dotenv())

openai.api_key  = os.getenv('OPENAI_API_KEY')
```

**Helper function**

- This function will make it easier to use prompts and look at the generated outputs:

It uses OpenAI's `gpt-3.5-turbo` model and the [chat completions endpoint](https://platform.openai.com/docs/guides/chat).


```python

def get_completion(prompt, model="gpt-3.5-turbo"):
    messages = [{"role": "user", "content": prompt}]
    response = openai.ChatCompletion.create(
        model=model,
        messages=messages,
        temperature=0, # this is the degree of randomness of the model's output
    )
    return response.choices[0].message["content"]
```
### Usage

```python
text = f"""
You should express what you want a model to do by \ 
providing instructions that are as clear and \ 
specific as you can possibly make them. \ 
This will guide the model towards the desired output, \ 
and reduce the chances of receiving irrelevant \ 
or incorrect responses. Don't confuse writing a \ 
clear prompt with writing a short prompt. \ 
In many cases, longer prompts provide more clarity \ 
and context for the model, which can lead to \ 
more detailed and relevant outputs.
"""
prompt = f"""
Summarize the text delimited by triple backticks \ 
into a single sentence.
```{text}```
"""
response = get_completion(prompt)
print(response)
```
#### Completion : 

```
Clear and specific instructions should be provided to guide a model towards the desired output, and longer prompts can provide more clarity and context for the model, leading to more detailed and relevant outputs.
```


## References

Main Course : 
- https://learn.deeplearning.ai/chatgpt-prompt-eng/lesson/1/introduction

Others short Free Courses available on DeepLearning.AI : 
- https://learn.deeplearning.ai/





