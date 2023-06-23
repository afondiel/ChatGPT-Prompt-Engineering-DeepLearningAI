# Lesson8: Chatbot

## Overview

In this notebook, you will explore how you can utilize the chat format to have extended conversations with chatbots personalized or specialized for specific tasks or behaviors.

## OpenAI API call Architecture

- Getting response from a single message

<img src="./img/l8-api-call0.png" width="600" style="border:0px solid #FFFFFF; padding:1px; margin:1px">

- Chat model

<img src="./img/l8-api-call1.png" width="600" style="border:0px solid #FFFFFF; padding:1px; margin:1px">

### Set role

New function allowing to get mutltiple messages

```python
def get_completion_from_messages(messages, model="gpt-3.5-turbo", temperature=0):
    response = openai.ChatCompletion.create(
        model=model,
        messages=messages,
        temperature=temperature, # this is the degree of randomness of the model's output
    )
#     print(str(response.choices[0].message))
    return response.choices[0].message["content"]
```
<img src="./img/l8-api-call2.png" width="600" style="border:0px solid #FFFFFF; padding:1px; margin:1px">

- The `system` message is a high-level instruction which sets the behavior of the assistant 
- The `user` message give the user instruction
- The `Assistant` the model completion

<img src="./img/l8-api-call3.png" width="600" style="border:0px solid #FFFFFF; padding:1px; margin:1px">


## References

Main course : 
- https://learn.deeplearning.ai/chatgpt-prompt-eng/lesson/8/chatbot


